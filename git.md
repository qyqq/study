## git是什么
Git是目前世界上最先进的分布式版本控制系统（没有之一）。
#### 在Windows上安装Git
msysgit是Windows版的Git，点击下面这条链接下载到本地！

1. > [下载地址](http://dlsw.baidu.com/sw-search-sp/soft/4e/30195/Git_V2.5.1_64_bit_setup.1441791170.exe)

2. 下载安装后打开 Git Bash
3. 在命令行输入:

	$ git config --global user.name "Your Name"
	$ git config --global user.email "email@example.com"
> 注意git config命令的--global参数，用了这个参数，表示你这台机器上所有的Git仓库都会使用这个配置，当然也可以对某个仓库指定不同的用户名和Email地址
> 
例如如果你公司的项目是放在自建的gitlab上面, 如果你不进行配置用户名和邮箱的话, 则会使用全局的, 这个时候是错误的, 正确的做法是针对公司的项目, 在项目根目录下进行单独配置

	$ git config user.name "Your Name"
	$ git config user.email "email@example.com"
4. 查看配置

	$ git config --list
#### 操作使用
##### 创建版本库

什么是版本库呢？版本库又名仓库，英文名repository，你可以简单理解成一个目录，这个目录里面的所有文件都可以被Git管理起来，每个文件的修改、删除，Git都能跟踪，以便任何时刻都可以追踪历史，或者在将来某个时刻可以“还原”。

1.选择一个合适的地方，创建一个空目录：

若Windows系统，请确保目录名（包括父目录）不包含中文。

	$ mkdir learngit
	$ cd learngit
	$ pwd
	/Users/michael/learngit
2.git init初始化仓库：

	$ git init
	Initialized empty Git repository in /Users/michael/learngit/.git/
tips:可以发现当前目录下多了一个.git的目录，这个目录是Git来跟踪管理版本库的，不要手动修改这个目录里面的文件，不然改乱了，就把Git仓库给破坏了

使用 ls -ah可以查看到.git
#### 把文件添加到版本库

在当前目录下来创建一个文件:

	$ touch readme.md
	$ vi readme.md
参考地址1
[http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)

参考地址2
[http://justcoding.iteye.com/blog/1830388](http://justcoding.iteye.com/blog/1830388)

参考地址3
[https://github.com/cuijiji/study-and-grow-up/tree/master/git](https://github.com/cuijiji/study-and-grow-up/tree/master/git)