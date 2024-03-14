# 添加路径
终端中zsh的可访问的程序一般放在`/bin, /usr/bin, /usr/local/bin，~/bin目录下`；而最新安装的Anaconda会默认安装在`/Users/username`下或者`/Users/username/opt`下，导致环境变量没有写入到终端配置文件。笔者的Anaconda默认被安装在了`~/opt`目录下，直接采用网络上的代码行不通，需要改一下路径。

1.先到/opt目录下查看是否有conda文件夹
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240314183400.png)

2.修改~/.zshrc 。添加路径
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240314183510.png)
```
export PATH="/opt/conda/bin:$PATH"
```
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240314183632.png)


3.source ~/.zshrc  追踪以下文件，即可使用conda
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240314183526.png)
