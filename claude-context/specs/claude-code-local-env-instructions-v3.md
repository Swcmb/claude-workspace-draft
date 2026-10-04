# Claude Code 本机环境适配指令集 v3.0

## 一、全局行为准则

### 1.1 语言规范
| 场景 | 语言 |
|:---|:---|
| 文档、说明、交互响应、计划 | 中文 |
| 代码注释、技术文档 | 中文 |
| 变量名、函数名、类名、提交信息 | 英文 |
| 内部推理过程 | 英文 |
| 编写规则、自定义命令、CLAUDE.md、Agent 提示词 | **英文** |

### 1.2 容器化隔离
- 数据库、消息队列、缓存、搜索引擎等**仅限 Docker 容器**运行
- 执行依赖 Docker 的命令前，**必须**提示用户启动 Docker 服务并等待确认

### 1.3 规则引用
代码质量规范 → `.claude/rules/code-quality.md`
特殊响应规则 → `.claude/rules/special-responses.md`

---

## 二、输出路径规范

### 2.1 根目录（强制）
所有规范、文档、计划、研究笔记、ADR 等产出物**仅限**存放于：
```
./claude-context/
```

### 2.2 子目录分类
| 目录 | 用途 |
|:---|:---|
| `specs/` | PRD、需求文档、用户故事、验收标准 |
| `plans/` | 开发计划、WBS、里程碑、迭代规划 |
| `docs/` | 项目描述、API 手册、部署指南 |
| `designs/` | 架构图、ER 图、接口设计 |
| `research/` | 技术选型、竞品分析、风险评估 |
| `artifacts/` | JSON Schema、SQL、配置模板等代码产出物 |

### 2.3 约束
- 写前确保目标子目录存在，否则 `mkdir -p` 自动创建
- 禁止保存至工作区根目录或临时目录
- 引用时使用相对路径 `./claude-context/...`
- 用户未指定路径时默认遵循以上规则，无需再次确认

---

## 三、环境清单权威机制

《本机开发环境清单》指明了当前报告输出时有什么开发环境


## 六、包管理器决策树

按优先级逐层判断，命中即停：

### 第一层：CUDA / GPU 生态
**触发词**：`torch` `torchvision` `torchaudio` `cudatoolkit` `cudnn` `tensorflow-gpu` `jax`（GPU 场景）

→ **仅允许 conda**，禁用 uv/pip：
```bash
conda activate default
conda install -c pytorch -c nvidia -n default pytorch torchvision torchaudio cudatoolkit=12.4 --yes
```
→ 禁止 `--index-url https://download.pytorch.org/whl/cu124` 及 `uv pip install torch` 等效指令
→ 预检 `~/.condarc`，缺少国内镜像则执行 `chsrc set conda`

### 第二层：普通 Python 依赖
→ 优先 `uv pip install --python $(which python) <package>`

### 第三层：Node.js / 前端
| 锁文件 | 包管理器 |
|:---|:---|
| `bun.lockb` | `bun install` / `bun run` |
| `pnpm-lock.yaml` | `pnpm` |
| `package-lock.json` | `npm` |
| 空项目 | 默认 `bun`（除非用户指定旧版兼容） |

---

## 七、编译链参数

### 7.1 C/C++（MinGW GCC 15.2.0）
识别到 `winlibs-x86_64-posix-seh` 后，编译命令必须包含：
```
-std=c++23 -static-libgcc -static-libstdc++ -O2
```

### 7.2 CUDA 一致性校验
GPU 验证代码不得仅写 `print(torch.cuda.is_available())`，必须同时输出：
```bash
conda list | grep cudatoolkit  # 确认 Conda Toolkit 版本
nvidia-smi                     # 确认驱动最高支持版本
```
若 `cudatoolkit` > 12.5 且 PyTorch 2.x 对 12.4 最稳定，必须警告并建议降级。

---

