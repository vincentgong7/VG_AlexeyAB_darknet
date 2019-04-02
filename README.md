#  Convenient functions for AexeyAB Darknet.

As **AlexeyAB updates** frequently, hereby I added a stable version of AlexeyAB Darknet with extra convenient functions.

Licensed with [![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)


## Batch images detector
Github link: [https://github.com/vincentgong7/VG_AlexeyAB_darknet](https://github.com/vincentgong7/VG_AlexeyAB_darknet)

The **detector** function in AlexeyAB Darknet only support single image. Therefore I added this function into this forked repo. Hope you like it. Please also refer to this post for detail:

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

[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)

