#  Convenient functions for YOLO based on AexeyAB Darknet.

[![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)
[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)


**You only look once (YOLO)** is a state-of-the-art, real-time object detection system. It is implemented based on the Darknet, an Open Source Neural Networks in C. In this project I improved the YOLO by adding several convenient functions for detecting objects for researches and the development community.

![enter image description here](https://raw.githubusercontent.com/vincentgong7/VG_AlexeyAB_darknet/master/exp/example/1.png | width=100)


![](https://raw.githubusercontent.com/vincentgong7/VG_AlexeyAB_darknet/master/exp/example/2.png)


![](https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png | width=100)



The added functions are implemented based on **AlexeyAB**  version of **Darknet**. As it is updated frequently, hereby I publish a stable version of AlexeyAB Darknet with those convenient functions. This repo will also be updated regularly.


## Batch images detector
Project link: [https://darknet.gong.im/](https://darknet.gong.im/)


Github link: [https://github.com/vincentgong7/VG_AlexeyAB_darknet](https://github.com/vincentgong7/VG_AlexeyAB_darknet)

The **detector** function in AlexeyAB Darknet only supports a single image at a time. Therefore I added the batch function into this forked repo, which support detecting images in a folder in one time. Hope you like it. Please also refer to the post for detail:

[https://github.com/pjreddie/darknet/issues/723](https://github.com/pjreddie/darknet/issues/723)

### Command
>./darknet detector batch cfg/coco.data cfg/yolov3.cfg weights/yolov3.weights batch exp/in_images/ exp/out_images/ > exp/results/results.txt

Parameter explain:
1. The input images are: **in_images/**
2. The output images are: **out_images/**
3. The detection classes with percentage is saved in: **exp/results/results.txt**

### Usage
1. Clone this project.
2. Download pre-trained weights file into foder **./weights/**. Such as: 

    [https://pjreddie.com/media/files/yolov3-openimages.weights](https://pjreddie.com/media/files/yolov3-openimages.weights)

3. Make the project with command in darknet/ folder: 
>make
4. Use the command described above to perform batch detecting images.

## Contact
Any questions please let me know.
vincent.gong7[at]gmail.com


[http://gong.im](http://gong.im)

