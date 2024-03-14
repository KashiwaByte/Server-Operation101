![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240314194524.png)
## 1. 上传本地文件夹到远程服务器
```
scp 【本地要上传文件地址】  [用户名]@[ip地址]：远程地址
```

```
//例如我的本地要上传的文件地址是c://user/code/demo/dist,用户名是root，IP地址是192.168.9.25
scp -r c://user/code/demo/dist root@192.168.9.25:/home/root/demo/fe/ 
//如果我当前在c://user/code/demo/下(比如在vscode打开demo项目打开终端)，就可以执行以下命令直接上传
//-r代表上传的是文件夹以及文件夹里所有的东西
scp -r dist root@192.168.9.25:/home/root/demo/fe/ 
```

## 2. 上传本地文件压缩包到远程服务器
如果是上传本地文件压缩包到远程服务器，上传成功后要在服务器上对压缩包进行解压

```
scp 【本地要上传的压缩包地址】      [用户名]@[ip地址]：远程地址
```

```
//例如我的本地要上传的压缩包地址是c://user/code.zip,用户名是root，IP地址是192.168.9.25

scp c://user/code.zip  root@192.168.9.25:/home/lu/gisspace/ocr_0.0.1/ocr

```

