<!--

 * @Description: YOLOX Deepstream
 * @Author: nanmi
 * @Date: 2021-07-21 16:23:35
 * @LastEditTime: 2021-07-21 16:23:35
 * @LastEditors: nanmi
 * @GitHub:github.com/nanmi
   -->

# YOLOX(Megvii-BaseDetection) Deploy DeepStream :two_hearts: :collision:

This project base on https://github.com/Megvii-BaseDetection/YOLOX  and https://zhuanlan.zhihu.com/p/391693130


# News

Adapt the new version of YOLOX original pre-training model, FPS > 100 - 2021-12-20

Deploy yolox to deep stream, FPS > 70 - 2021-7-21

# System Requirements

cuda 11.0+

TensorRT 8+

OpenCV 4.0+ (build with opencv-contrib module) [how to build](https://gist.github.com/nanmi/c5cc1753ed98d7e3482031fc379a3f3d#%E6%BA%90%E7%A0%81%E7%BC%96%E8%AF%91gpu%E7%89%88opencv)

OpenMP

DeepStream 6.0+

# Installation

Make sure you had install dependencies list above

```bash
# clone project and submodule
git clone {this repo}

cd {this repo}/nvdsinfer_custom_impl_yolox/

make
```

use to parse infer postprocess.

# Run

```shell
cd {this repo}

deepstream-app -c deepstream_app_config.txt
```

# How to build engine?

https://zhuanlan.zhihu.com/p/391693130

# About License

For the 3rd-party module and Deepstream, you need to follow their license

For the part I wrote, you can do anything you want

