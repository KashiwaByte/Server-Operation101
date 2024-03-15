# jukemirlib
https://github.com/rodrigo-castellon/jukemirlib

### Installing

You can install via `pip`

```shell
pip install git+https://github.com/rodrigo-castellon/jukemirlib.git
```



# accelerate
```
pip install accelerate
```
# 缺乏sndfile
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240314204831.png)

```
sudo apt-get install libsndfile1-dev
```



# 缺乏pytorch3d

![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240314204952.png)


```
conda install -c bottler nvidiacub
```

```
conda install -c fvcore -c iopath -c conda-forge fvcore iopath
```

```
# Anaconda Cloud
conda install pytorch3d -c pytorch3d
```



# libffi.so.7
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240314215508.png)

```
wget http://es.archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi7_3.3-4_amd64.deb

sudo dpkg -i libffi7_3.3-4_amd64.deb
```


# torch.cuda.is_available() False



```
pip install torch==1.12.0+cu116 torchvision==0.13.0+cu116 torchaudio==0.12.0 --extra-index-url https://download.pytorch.org/whl/cu116
```


# Cuda
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240315104249.png)

# 生成选项错误
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240315114642.png)

安装完整版ffmpeg
```
sudo apt install ffmpeg

```


# FbxCommon报错
![image.png](https://kashiwa-pic.oss-cn-beijing.aliyuncs.com/20240315111220.png)

需要安装fbx的SDK




# SMPL-to-FBX解决方案
参照以下这个库，不过需要修改以下zip文件
https://github.com/softcat477/SMPL-to-FBX
把__init__.py文件第72行的 修改如下（去掉缩放属性）
```
"smpl_trans":data["smpl_trans"]}
```