### 直接使用训练好的模型去水印项目

# 安装文件

```
# tensorflow-2.4.1
pip3 install tensorflow -i https://mirrors.aliyun.com/pypi/simple/

# numpy-1.19.5
pip3 install numpy -i https://mirrors.aliyun.com/pypi/simple/

# Successfully installed keras-2.4.3 pyyaml-5.4.1 scipy-1.6.0
pip3 install keras -i https://mirrors.aliyun.com/pypi/simple/

# Successfully installed opencv-python-4.5.1.48
pip3 install opencv-python -i https://mirrors.aliyun.com/pypi/simple/

# Successfully installed pillow-8.1.0
pip3 install pillow -i https://mirrors.aliyun.com/pypi/simple/
```

# pip install -h 就有说明了，就是 --upgrade，意思是如果已安装就升级到最新版 
# -U 升级到最新版本
pip3 install -U numpy -i https://mirrors.aliyun.com/pypi/simple/


# 执行清除水印

```
python3 test_model.py --weight_file Watermark.hdf5  --image_dir inputdir --output_dir outputdir
```


> 水印模型文件名.hdf5替换成实际的文件名，inputdir里放入有水印的图片，执行命令。去除水印后的图片会静静的躺在 outputdir目录里。
