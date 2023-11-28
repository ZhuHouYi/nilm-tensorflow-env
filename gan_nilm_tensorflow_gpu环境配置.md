python豆瓣源：https://pypi.douban.com/simple/



# gan_nilm_tensorflow_gpu环境配置

1.驱动版本

![image-20231127194848481](.\image\image-20231127194848481.png)

2.cuda选择：11.2

3.cudnn选择：8.1

4.python版本：3.8

5.tensorflow-gpu版本：2.6.0：`pip install tensorflow-gpu==2.6.0 -i https://pypi.douban.com/simple/`

![image-20231127195318281](.\image\image-20231127195318281.png)

6.将以下环境变量添加：

![image-20231127205249109](C.\image\image-20231127205249109.png)

# 成功.



额外注意事项：

1.本次配置环境前电脑已经有cuda11.8版本了，安装cuda11.2时会报错：![image-20231127211215625](.\image\image-20231127211215625.png)

此时卸载以下软件

- NVIDIA Frameview SDK
- NVIDIA PhysX

之后能正常安装，但是环境目录中出现CUDA_PATH和两个路径，如果后面想重新使用11.8，可能还需要将CUDA_PATH改回来。

![image-20231127211316210](.\image\image-20231127211316210.png)

2.使用pip安装tensorflow-gpu==2.6.0后运行可能会报安装包不兼容的错误，此时继续pip安装所需的包即可，例如protobuf、keras(对应版本为2.6.0)、tables(使用pip安装，默认为3.8.0)。

3.如果cuda和cudnn环境报错：zlibwapi.dll文件找不到，那么就去zlib官网下载zlib123dllx64.zip压缩包，解压后将zlibwapi.dll放到cuda 11.2或cuda 11.8的bin目录下，zlibwapi.lib放到lib目录下即可。

