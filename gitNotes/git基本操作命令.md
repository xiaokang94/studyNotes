# git 基本操作命令 #
## 初始化git仓库 ##
1. 初始化一个空的仓库

	``` shell
	git init
	``` 
2. 远程克隆一个仓库

	```shell
		## rename 存放克隆文件的目录
		git clone https://github.com/xiaokang94/studyNotes.git rename 
	```
3. 跟踪一个文件并添加到暂存区域
	
	```linux
		git add *
	``` 
4. 将暂存区域的文件 添加到本地仓库
	```shell
		git commit -m '日志记录'	
	```
5. 上传时忽略文件
	- git控制根目录下创建.gitignore文件


