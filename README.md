## 安装方式

在使用本项目之前，请先确保电脑中已经安装 Git。

---

### Windows 安装 Git

#### 1. 下载 Git

进入 Git 官方下载页面，下载 Windows 版本安装包：

```bash
https://git-scm.com/downloads
```

也可以直接进入 Windows 安装页面：

```bash
https://git-scm.com/install/windows
```

#### 2. 安装 Git

下载完成后，双击运行安装程序。

安装过程中一般保持默认选项即可。如果不确定每一步选什么，直接点击 `Next` 继续安装。

安装完成后，可以使用以下工具执行 Git 命令：

- Git Bash
- Windows Terminal
- VS Code 终端

#### 3. 检查是否安装成功

打开 Git Bash 或终端，输入：

```bash
git --version
```

如果能够看到 Git 的版本号，说明安装成功。

示例：

```bash
git version 2.54.0
```

---

### macOS 安装 Git

macOS 推荐使用 Homebrew 安装 Git。

#### 1. 安装 Homebrew

打开终端，执行 Homebrew 官方安装命令：

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

安装过程中根据终端提示输入电脑密码，并按提示继续。

#### 2. 配置 Homebrew 环境变量

Homebrew 安装完成后，终端通常会显示 `Next steps`。

请优先按照终端中 `Next steps` 给出的命令进行配置。

对于 Apple Silicon 芯片的 Mac，例如 M1、M2、M3、M4，一般需要执行：

```bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

#### 3. 检查 Homebrew 是否安装成功

```bash
brew --version
```

如果能够看到 Homebrew 的版本号，说明 Homebrew 安装成功。

#### 4. 使用 Homebrew 安装 Git

```bash
brew install git
```

#### 5. 检查 Git 是否安装成功

```bash
git --version
```

如果能够看到 Git 的版本号，说明 Git 安装成功。
