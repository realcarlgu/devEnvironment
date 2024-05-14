在 Ubuntu 系统中，你可以通过如下步骤来保留所有的历史记录：

bash
# 打开.bashrc文件
nano ~/.bashrc

# 在文件最后添加如下四行代码
HISTSIZE=-1
HISTFILESIZE=-1
shopt -s histappend
PROMPT_COMMAND='history -a'

# 使用下面的命令保存并退出nano编辑器
ctrl+o 
enter
ctrl+x

# 让刚才的改动立即生效
source ~/.bashrc
其中：

HISTSIZE=-1 和 HISTFILESIZE=-1 允许bash shell 保存无线的命令到内存和硬盘中。
shopt -s histappend 确保在每次打开一个新的 shell 时，新的命令添加到history文件的尾部。
PROMPT_COMMAND='history -a' 使每一次命令都会立即写入历史记录。
