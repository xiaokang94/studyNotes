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
			git checkout brtesat
		 ```
	 - 项目分叉历史
		 
		```shell
			git log --oneline --decorate --graph --all
		```

