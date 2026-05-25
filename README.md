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

## 初始化 Git 仓库

安装 Git 后，可以将一个普通项目文件夹初始化为 Git 仓库，使 Git 开始记录该项目的修改历史。

### 1. 进入项目文件夹

首先打开终端，并进入需要管理的项目目录。

例如：

```bash
cd your-project-folder
```

其中，`your-project-folder` 需要替换成自己的项目文件夹路径。

### 2. 初始化 Git 仓库

在项目文件夹中执行：

```bash
git init
```

执行成功后，当前文件夹会被初始化为一个 Git 仓库。

Git 会在该目录下创建一个隐藏文件夹：

```bash
.git
```

这个 `.git` 文件夹用于保存 Git 的版本记录和配置信息，一般不需要手动修改。

### 3. 查看仓库状态

可以使用以下命令查看当前 Git 仓库的状态：

```bash
git status
```

如果看到文件显示为 `Untracked files`，说明这些文件还没有被 Git 跟踪。

### 4. 添加文件到 Git 暂存区

执行：

```bash
git add .
```

该命令会将当前目录下的所有文件添加到 Git 暂存区。

### 5. 提交第一个版本

执行：

```bash
git commit -m "Initial commit"
```

其中，`Initial commit` 表示第一次提交的说明。

提交完成后，Git 就已经开始记录该项目的版本历史。

### 6. 查看提交记录

可以使用以下命令查看提交历史：

```bash
git log
```

如果能够看到刚才的提交信息，说明项目已经成功交由 Git 管理。
