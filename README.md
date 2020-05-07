
#  Convenient functions for YOLO based on AexeyAB Darknet.

[![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)
[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)


**You only look once (YOLO)** is a state-of-the-art, real-time object detection system. It is implemented based on the Darknet, an Open Source Neural Networks in C. In this project I improved the YOLO by adding several convenient functions for detecting objects for researches and the development community.


<img src="https://raw.githubusercontent.com/vincentgong7/VG_AlexeyAB_darknet/yolo_v3/exp/example/1.png" alt="" width="400"/> <img src="https://raw.githubusercontent.com/vincentgong7/VG_AlexeyAB_darknet/yolo_v3/exp/example/2.png" alt="" width="400"/>

Figure. Example of Object Detection using Yolo based on the Darknet.


The added functions are implemented based on **AlexeyAB**  version of **Darknet**. As it is updated frequently, hereby I publish a stable version of AlexeyAB Darknet with those convenient functions. This repo will also be updated regularly.


## Batch images detector
Github link: [https://github.com/vincentgong7/VG_AlexeyAB_darknet](https://github.com/vincentgong7/VG_AlexeyAB_darknet)

<img src="https://raw.githubusercontent.com/vincentgong7/VG_AlexeyAB_darknet/master/exp/example/vg_darknet_batch_detector.png" alt="" width="60%" />

Figure. The process of batch detecting images in a folder using Yolo based on the Darknet.


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
2. Download pre-trained weights file into folder **./weights/**. Such as: 

    [https://pjreddie.com/media/files/yolov3-openimages.weights](https://pjreddie.com/media/files/yolov3-openimages.weights)

3. Build the project

	3.1 For linux: Make the project with command in darknet/ folder: 
	>make
	
	3.2 For windows, please modify one line in top in the detector.c, using the header file for Windows.
	
	//#include <dirent.h> //for linux, ubuntu, macos
	
	#include "dirent_win.h" //for windows
	
	Then it can be successfully built on Visual Studio.
	
5. Use the command described above to perform batch detecting images.

## Contact
Any questions please let me know.
vincent.gong7[at]gmail.com



<!-- <img src="https://github.com/vincentgong7/VG_AlexeyAB_darknet/blob/master/exp/example/icon_link.png?raw=true" alt="" width="15" valign = "middle"/> [Gong.im](http://gong.im) -->

:palm_tree: [*Gong.im*](http://gong.im)

:floppy_disk: [Guestbook](https://github.com/vincentgong7/VG_AlexeyAB_darknet/issues/7)

<script type="text/javascript" src="//counter.websiteout.net/js/5/4/69/0"></script>
<br>
<div style="float: left;"><script type="text/javascript" id="clustrmaps" src="//cdn.clustrmaps.com/map_v2.js?cl=ffffff&w=600&t=m&d=hUfpL0e-tBg_zcx45xNWS0tq1zo_Jj5POALETOYreCY&co=2d78ad&cmo=3acc3a&cmn=ff5353&ct=ffffff"></script></div>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
