# 常用命令之apache篇 #

1. 如何查看当前apache 服务的版本及虚拟主机的配置信息 

    ````
        1. 查看apache当前的版本
        
            httpd -v
            
        2. 查看当前apache 所配置的虚拟主机的信息
        
            httpd -h // 命令记不住时通过帮助命令查找
            httpd -t -D DUMP_VHOSTS 
        
            
    ````
