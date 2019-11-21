# 操作系统
- 操作系统分类
    - windows
    - MacOS
    - Unix
        - Minix,Linus-Linux
        - MacOS
- 虚拟机
    - 下载Virtualbox
- 自行安装
    - 安装套件anaconda+pycham www.jetbrains.com
    - 如果官网很慢，可以使用anaconda清华源网站上下

# GIT-起源
- 集中式：cvs,svn
- 分布式：github开源，bitbuckets私人
- 分享精神：blog+github

# Git安装
- windows:官网上下载安装即可
- Linux:原则上也可以从官网下载，但需要语句。启动终端：sudo su-输入密码-- 变为root@augs:/home/tlxy#-- 输入apt-get install git--输入aptitude search git(搜索名字里面带git的)--aptitude show git--aptitude install git（安装git）
- MacOS:

- 在git文件夹里选git-brash
- pwd：显示当前用户名

# Git 基本使用
- 创建仓库命令 git init 
- 创建新的文件夹：mkdir 新文件夹的名称
- 进入文件夹：cd 文件夹名称
- 初始化一个仓库：git init
- 看git文件夹里的东西：ll -a ./.git
- 创建文件：touch one.txt
- 编辑文件：vi one.txt
- 进入编辑模式：i
- 编辑结束保存并退出：按ESC+大写ZZ
- 看文件中内容：cat one.txt
- 查看当前文件夹中的文件：ls
- 将文件放在暂存区：git add one.txt
- 用 git config --global user.email"我的email"
- 用 git config --global user.name"gty"初始化git
- 将暂存区的内容上传到仓库： git commit
- 进入编辑窗口：写上这一次的注释，以便下一次查找
- 退出编辑：ESC+:wq
- 存入仓库成功
- 或直接用 git commit -m"message for desc":向仓库提交内容
- 每次的版本是通过[master 3cfb2fa]那一串版本号确定的，相当于ID
- git status 看仓库目前的状态
- git rm:删除信息
- git log:查看日志 head表示当前的版本
- git reset --hard 版本号（commit后面跟的那个很长的版本号，不是上面的那个）：回滚
- 其余的看廖雪峰的教程:www.liaoxuefeng.com

# Github and Bitbuckets 远程仓库
- https://github.com
- start project创建一个仓库
