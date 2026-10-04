# 本机开发环境清单

> 扫描时间: 2026-06-23 20:25 (开始时间)
> 系统: Windows 11 Pro 10.0.26100
> Shell: Git Bash (GNU bash, bundled with Git for Windows)
> PowerShell: 5.1.26100.4202
> PowerShell 执行策略: RemoteSigned

---

## 摘要

| 分类 | 已安装 | 正常 ✅ | 异常 ⚠️ | 未检测到 ❌ |
|------|--------|---------|---------|------------|
| 编程语言 SDK | 8 | 7 | 1 | 3 |
| 包管理器 | 8 | 8 | 0 | 6 |
| 容器与虚拟化 | 3 | 3 | 0 | 3 |
| 数据库与中间件 | 0 | 0 | 0 | 6 |
| IDE 与编辑器 | 7 | 7 | 0 | 4 |
| 版本控制 | 2 | 2 | 0 | 2 |
| 终端与 Shell | 4 | 4 | 0 | 2 |
| AI/LLM 工具 | 3 | 2 | 1 | 1 |
| 网络工具 | 2 | 2 | 0 | 3 |
| 其他工具 | 12 | 12 | 0 | 5 |
| **合计** | **49** | **47** | **2** | **35** |

---

## 详细清单

### 1. 编程语言 SDK / 运行时

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| Node.js | v22.18.0 | D:\ProgramFiles\nodejs | ✅ | |
| npm | 10.9.3 | D:\ProgramFiles\nodejs\npm | ✅ | |
| pnpm | 11.4.0 | C:\Users\Swcmb\AppData\Roaming\npm\pnpm | ✅ | 全局安装 |
| yarn | 1.22.22 | C:\Users\Swcmb\AppData\Roaming\npm\yarn | ✅ | 全局安装 |
| Python | 3.13.9 | D:\ProgramFiles\anaconda3\envs\default\python.exe | ✅ | Anaconda 环境 |
| pip | 26.0.1 | D:\ProgramFiles\anaconda3\envs\default\Scripts\pip.exe | ✅ | |
| Java (JDK) | 21.0.8 LTS | D:\ProgramFiles\Java\jdk-21\bin | ✅ | 2025-07-15 发布 |
| javac | 21.0.8 | D:\ProgramFiles\Java\jdk-21\bin | ✅ | |
| Go | 1.25.4 | D:\ProgramFiles\Go\bin | ✅ | windows/amd64 |
| Rust (rustc) | 未检测到 | — | ❌ | |
| Cargo | 未检测到 | — | ❌ | |
| .NET SDK | 5.0.408 | C:\Program Files\dotnet\sdk | ⚠️ | 仅 SDK 5.0，较旧；运行时有 5.0/6.0/7.0/8.0 |
| .NET Runtime | 5.0.17 / 6.0.26 / 7.0.20 / 8.0.15 | C:\Program Files\dotnet\shared | ✅ | 多版本共存 |
| Ruby | 未检测到 | — | ❌ | |
| PHP | 未检测到 | — | ❌ | |
| Deno | 未检测到 | — | ❌ | |
| Bun | 1.2.17 | D:\ProgramFiles\bun_uv\bun.exe | ✅ | |

### 2. 包管理器 / 构建工具

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| npm | 10.9.3 | D:\ProgramFiles\nodejs\npm | ✅ | |
| pnpm | 11.4.0 | C:\Users\Swcmb\AppData\Roaming\npm\pnpm | ✅ | |
| yarn | 1.22.22 | C:\Users\Swcmb\AppData\Roaming\npm\yarn | ✅ | |
| Bun | 1.2.17 | D:\ProgramFiles\bun_uv\bun.exe | ✅ | 含 bun install |
| uv | — | D:\ProgramFiles\bun_uv\uv.exe | ✅ | Python 包管理器 |
| pip | 26.0.1 | D:\ProgramFiles\anaconda3\envs\default\Scripts\pip.exe | ✅ | |
| conda | — | D:\ProgramFiles\anaconda3\envs\default\Library\bin\conda.bat | ✅ | Anaconda 环境内 |
| Maven (mvn) | — | D:\ProgramFiles\JetBrains\IntelliJ IDEA 2024.3.6\plugins\maven\lib\maven3\bin\mvn | ✅ | IDEA 内置 |
| poetry | 未检测到 | — | ❌ | |
| Gradle | 未检测到 | — | ❌ | |
| Cargo | 未检测到 | — | ❌ | |
| vcpkg | 未检测到 | — | ❌ | |
| scoop | 未检测到 | — | ❌ | |
| chocolatey | 未检测到 | — | ❌ | |

### 3. 容器与虚拟化

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| Docker | 29.2.1 | C:\Program Files\Docker\Docker\resources\bin | ✅ | build a5c7197 |
| Docker Compose | v5.0.2 | C:\Program Files\Docker\Docker\resources\bin | ✅ | |
| WSL2 | — | — | ✅ | Ubuntu-24.04 (Running), docker-desktop (Running) |
| kubectl | — | C:\Program Files\Docker\Docker\resources\bin\kubectl.exe | ✅ | Docker Desktop 附带 |
| Podman | 未检测到 | — | ❌ | |
| Vagrant | 未检测到 | — | ❌ | |
| VirtualBox | 未检测到 | — | ❌ | |

### 4. 数据库与中间件

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| MySQL | 未检测到 | — | ❌ | 无服务、无客户端 |
| PostgreSQL | 未检测到 | — | ❌ | |
| MongoDB | 未检测到 | — | ❌ | |
| Redis | 未检测到 | — | ❌ | |
| RabbitMQ | 未检测到 | — | ❌ | |
| Elasticsearch | 未检测到 | — | ❌ | |

> **注**: 数据库可能运行在 WSL Ubuntu-24.04 或 Docker 容器中，本次扫描仅覆盖 Windows 原生安装。

### 5. IDE 与编辑器

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| VS Code | 1.125.1 | D:\ProgramFiles\Microsoft VS Code | ✅ | |
| IntelliJ IDEA | 2024.3.6 | D:\ProgramFiles\JetBrains\IntelliJ IDEA 2024.3.6 | ✅ | |
| PyCharm | 2024.3.6 | D:\ProgramFiles\JetBrains\PyCharm 2024.3.6 | ✅ | |
| CLion | 2025.3.3 | D:\ProgramFiles\JetBrains\CLion 2025.3.3 | ✅ | |
| DataGrip | 2026.1.2 | D:\ProgramFiles\JetBrains\DataGrip 2026.1.2 | ✅ | 仅路径检测 |
| Trae CN | — | D:\ProgramFiles\Trae CN | ✅ | AI IDE |
| Vim | 9.1 | D:\ProgramFiles\Git\usr\bin\vim.exe | ✅ | Git Bash 内置 (2024-01-02) |
| Cursor | 未检测到 | — | ❌ | |
| WebStorm | 未检测到 | — | ❌ | |
| GoLand | 未检测到 | — | ❌ | |
| Rider | 未检测到 | — | ❌ | |
| Visual Studio | 未检测到 | — | ❌ | D:\ProgramFiles\Microsoft Visual Studio 目录存在但 devenv 不可用 |
| Neovim | 未检测到 | — | ❌ | |

### 6. 版本控制工具

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| Git | 2.51.0.windows.1 | D:\ProgramFiles\Git\mingw64\bin\git.exe | ✅ | |
| GitHub CLI | 2.95.0 | C:\Program Files\GitHub CLI | ✅ | 2026-06-17 发布 |
| GitKraken | 未检测到 | — | ❌ | |
| SourceTree | 未检测到 | — | ❌ | |

### 7. 终端与 Shell 工具

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| PowerShell | 5.1.26100.4202 | 内置 | ✅ | Windows 自带 |
| Git Bash | — | D:\ProgramFiles\Git\usr\bin\bash.exe | ✅ | 当前主 Shell |
| Oh My Posh | — | C:\Users\Swcmb\AppData\Local\Microsoft\WindowsApps | ✅ | |
| Windows Terminal | — | C:\Users\Swcmb\AppData\Local\Microsoft\WindowsApps\wt.exe | ✅ | |
| PowerShell 7 (pwsh) | 未检测到 | — | ❌ | 仅检测到内置 PS 5.1 |
| zsh | 未检测到 | — | ❌ | |

### 8. AI / LLM 开发工具

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| Ollama | 0.30.8 | C:\Users\Swcmb\AppData\Local\Programs\Ollama | ⚠️ | 已安装但服务未运行 |
| NVIDIA GPU | RTX 5060 | — | ✅ | Driver 581.29, CUDA 13.0 |
| CUDA Toolkit | 12.9 (V12.9.41) | C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.9 | ✅ | nvcc 可用 |
| NVIDIA Nsight Compute | 2025.3.0 | C:\Program Files\NVIDIA Corporation\Nsight Compute 2025.3.0 | ✅ | PATH 中 |
| LM Studio | — | C:\Users\Swcmb\.lmstudio | ✅ | 仅配置目录检测到 |
| PyTorch | 未检测到 | — | ❌ | Python 环境中未安装 |
| TensorFlow | 未检测到 | — | ❌ | |

### 9. 网络与 API 工具

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| curl | 8.15.0 | D:\ProgramFiles\Git\mingw64\bin\curl.exe | ✅ | 多处安装：Git Bash、anaconda、Windows System32、独立版 |
| curl (独立版) | 8.20.0 | D:\ProgramFiles\curl-8.20.0_1-win64-mingw\bin | ✅ | PATH 中有独立版本 |
| Postman | — | C:\Users\Swcmb\AppData\Local\Postman | ✅ | 安装目录存在 |
| wget | 未检测到 | — | ❌ | |
| HTTPie | 未检测到 | — | ❌ | |
| Insomnia | 未检测到 | — | ❌ | |

### 10. 其他开发工具

| 工具 | 版本 | 安装路径 | 状态 | 备注 |
|------|------|---------|------|------|
| SSH (OpenSSH) | 10.0p2 | 内置 | ✅ | OpenSSL 3.2.4 |
| OpenSSL | 3.2.4 | 内置 | ✅ | |
| cmake | — | D:\ProgramFiles\winlibs-x86_64-posix-seh-gcc-15.2.0-mingw-w64ucrt-14.0.0-r7\mingw64\bin | ✅ | MinGW 工具链附带 |
| GCC (MinGW) | 15.2.0 | D:\ProgramFiles\winlibs-x86_64-posix-seh-gcc-15.2.0-mingw-w64ucrt-14.0.0-r7\mingw64\bin | ✅ | POSIX SEH, MinGW-w64 UCrt 14.0.0-r7 |
| TeX Live | 2026 | D:\ProgramFiles\texlive\2026\bin\windows | ✅ | LaTeX 排版系统 |
| Tesseract OCR | — | D:\ProgramFiles\Tesseract-OCR | ✅ | OCR 引擎 |
| ffmpeg | — | E:\Program Files\ffmpeg-master-latest-win64-gpl-shared\bin | ✅ | E 盘 |
| Wireshark | — | D:\ProgramFiles\Wireshark | ✅ | 网络抓包 |
| Vim | 9.1 | D:\ProgramFiles\Vim\vim91 | ✅ | |
| draw.io | — | D:\ProgramFiles\draw.io | ✅ | 流程图工具 |
| Zotero | — | D:\ProgramFiles\Zotero | ✅ | 文献管理 |
| XshellPlus | — | D:\ProgramFiles\XshellPlus | ✅ | SSH 客户端（绿化版） |
| SPSS | — | D:\ProgramFiles\SPSS\Statistics | ✅ | 统计分析 |
| RedPanda C++ | — | D:\ProgramFiles\RedPanda-Cpp | ✅ | C++ IDE |
| reqable | — | D:\ProgramFiles\reqable | ✅ | API 调试 |
| atomcode | v4.15.3 | D:\ProgramFiles\atomcode | ✅ | |
| chsrc | — | C:\Users\Swcmb\AppData\Local\Microsoft\WinGet\Packages\RubyMetric.chsrc... | ✅ | 换源工具 |
| VMware Workstation | — | C:\Program Files (x86)\VMware\VMware Workstation\bin | ✅ | PATH 中 |
| DeepLX | — | E:\Program Files\DeepLX | ✅ | 翻译工具 |
| msys64 | — | D:\ProgramFiles\msys64\ucrt64\bin | ✅ | UCrt64 环境 |
| PowerToys | — | C:\Program Files\PowerToys | ✅ | DSCModules 在 PATH 中 |
| .NET Tools | — | C:\Users\Swcmb\.dotnet\tools | ✅ | 用户级工具 |
| Terraform | 未检测到 | — | ❌ | |
| Ansible | 未检测到 | — | ❌ | |
| AWS CLI | 未检测到 | — | ❌ | |
| Azure CLI | 未检测到 | — | ❌ | |
| GCP CLI | 未检测到 | — | ❌ | |
| helm | 未检测到 | — | ❌ | |
| make | 未检测到 | — | ❌ | |

