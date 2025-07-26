# ResNet50v2_RK3588_Classification

1.项目代码介绍

src/main.cc ：主程序运行文件

src/resnet.cc：模型初始化、推理、反初始化等函数代码

include/resnet.h：各函数声明
include/rknn_api.h：rknn底层模型初始化和推理的库librknnrt.so对应的头文件

2.配置文件介绍

jpg2png.py是jpg图片转png格式的脚本，直接使用jpg图片读取会失败，所以先用该脚本转成png格式后再运行

3rdparty 中是第三方库

build 是编译位置

inputimage 是输入图片所在文件夹

model 是RKNN模型以及标签名txt文件所在文件夹

rknn_lib 是瑞芯微官方动态库librknnrt.so所在位置

3.编译运行

**①cd build**

**②cmake ..**

**③make**

**④./rknn_resnet50_demo ../model/xxx.rknn ../inputimage/xxx.png**





CSDN地址：[【ResNet50图像分类部署至RK3588】模型训练→转换RKNN→开发板部署](https://blog.csdn.net/A_l_b_ert/article/details/149648932?spm=1001.2014.3001.5501)

QQ咨询（not free，除非你点了小星星）：2506245294

此处统一说明：加QQ后直接说问题和小星星截图，对于常见的相同问题，很多都已在CSDN博客中提到了（RKNN转换流程是统一的，可去博主所有的RKNN相关博客下去翻评论），已在评论中详细解释过的问题，不予回复。
