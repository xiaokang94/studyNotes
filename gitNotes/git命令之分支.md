# git 分支 #
 - 分支创建

	```shell
	git branch brtesat # 创建分支并不切换到创建的分支中去
	```
 - 查看各个分支当前所指的对象
		 
	 ```shell
	git log --oneline --decorate
	 ```

 - 分支切换
		 
	```shell
	git checkout brtesat # 切换到brtesat分支
	 ```
 - 项目分叉历史
		 
	```shell
	git log --oneline --decorate --graph --all # 查看提交日志
	```

 - 分支的新建与合并
	
	- 新建分支
		
	 	- 从当前提交的历史中新建一个分支(Head 指针从当前提交版本开始)
			 
			```shell
				git checkout -b branchname 
			```
		- 合并分支(当前所在的分支指向要合并的分支)
			
			```shell
				git checkout master # 切换到master分支
				git merge  brtesat # 将master 分支的指针指向brtesat
			```
 
 - 查看所有的分支
	
	```shell
	git branch -v # 查看所有分支的最后一次提交
	git branch --merged # 显示所有合并后的分支
	git branch --no-merged # 显示所有未合并的分支
	```

 - 删除分支(删除时 工作目录所在的分支不能是删除的分支)
      
	```shell
	git checkout master # 切换到主分支
	git branch -d brtesat # 删除合并后的分支
	git branch -D brtesat # 删除未合并的分支(强制删除)
	```	
 - 分支合并时冲突解决
	
	```shell
		git status # 使用该命令 查看详情

	```
	
 - 远程分支

	- 获取远程分支 标签信息
		
		```shell
		git ls-remote	# 显式获取远程引用的完整列表
		git remote show (remote) # 获取远程分支更多信息
		```
	- 推送/抓取远程分支

		```shell
			git push (remote) (branch) # 推送远程分支
			git fetch (remote) # 抓取远程分支
			git merge (remote)/(branch) # 合并分支
			git checkout -b (branch) (remote)/(branch) #新建一个分支
		```
	- 跟踪分支

		```shell
			git checkout --track (remote)/(branch)
		```
	- 查看所有的跟踪分支

		```shell
			git branch -vv
		```
	- 删除远程分支
		
		```shell 
			git push remote --delete branchname # git服务器只是删除指针
		```
	
