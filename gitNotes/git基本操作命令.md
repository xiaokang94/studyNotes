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

6. 查看已暂存和未暂存区域的修改(当前文件夹和暂存区域之间的差异)
	```shell
		git diff
	```
7. 查看已暂存区域和本地仓库最新版本之间的更改

	```shell
		git diff --cached
	```
8. 移除文件
	```shell
	git rm test.md
	```
9. 文件改名
	```shell
		git mv test.md test2.md
	```
10. 查看日志

	- 查看所有的日志记录

		```shell
		git log
		```
	- 查看最近三次提交的内容差异
		```shell
			git log -p -3	
		```
	- 每次提交的简略统计信息
		```shell
			git log --stat
		```
11. 撤销操作	
	
	- 重新提交
		```shell
			git commit --amend
		```
	- 取消暂存的文件
		```shell
			git reset HEAD test.md
		```
	- 撤销对文件的修改
		```shell
			git checkout -- test.md
		```

  

