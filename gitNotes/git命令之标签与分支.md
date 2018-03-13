# git标签与分支 #

### git标签 ###
 - 创建标签

	 1. 轻量标签

 		- 指一个特定提交的引用

 	2. 附注标签

		 - 存储在git数据库中的一个完整的对象；

 	 	- 特征

  	 	- 可以被校验

	 	- 包含打标签者的名字，电子邮件地址,日期时间；

 	3. 打标签

		```linux
		git tag -a v1.0 -m '第一次打标签测试'
		```
 	4. 显示标签的信息与对应的提交信息

		 ```shell
			git show v1.0 
		 ```
	5. 显示过去的提交及给过去版本打标签
		
		 ```shell
			git log --pretty=online # 显示过去的提交历史
			git tag -a v1.1 key值 # 给过去提交的某一项目打标签
		 ```
	6. 远程共享标签
		
		```shell
			git push remote_name [tagename|--tags]
		```
	7. 检出标签 
		
		```shell
			git checkout -b v1.0	
		```

