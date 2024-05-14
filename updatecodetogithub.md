# 如何安装 TortoiseGit 并配置 GitHub

这篇文章将会帮助你理解如何在 Windows 系统上安装 TortoiseGit 并链接你的 GitHub 账户，使得你可以同步你的代码记录。

## 安装TortoiseGit

1. 访问[TortoiseGit下载页面](https://tortoisegit.org/download/)并根据你的操作系统的位数（32位或64位）下载合适的安装包。
2. 双击下载的安装文件开始安装，点击`Next`接受许可协议。
3. 选择你的安装路径并点击`Next`。
4. 然后你可以选择需要安装的额外功能并点击`Next`。
5. 选择你的 git.exe 路径。如果你已经安装了 Git，则 TortoiseGit 会自动检测到。如果没有，则你需要先下载并安装 Git。
6. 接下来进行一些额外设置，然后点击`Install`开始安装。
7. 安装完成后点击`Finish`结束安装。

## 配置 GitHub

1. 首先，你需要一个 GitHub 账户。如果你还没有，请访问 [GitHub官网](https://github.com/) 注册一个新账户。
2. 在你的电脑上生成 SSH 公私钥对。打开 Git bash，运行以下命令：

    ```bash
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```

    按提示操作，最后会在你的用户目录下生成 .ssh 文件夹，里面的 id_rsa 是私钥，id_rsa.pub 是公钥。
3. 登录 GitHub，点击头像 -> Settings -> SSH and GPG keys -> New SSH key。标题随意填写，然后打开你的 id_rsa.pub 文件，复制里面的内容粘贴到 Key 栏。
4. 回到 TortoiseGit，右键你的项目文件夹，选择 TortoiseGit -> Settings -> Git -> Remote。在 Remote 邨存库处填入你需要同步的 GitHub 仓库地址，然后点击 Add New/Save。

至此，你已经成功安装并配置了 TortoiseGit，并将其与 GitHub 账户关联。你现在可以提交你的代码，并同步到 GitHub 上。
