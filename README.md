
#  Convenient functions for YOLO v4 based on AlexeyAB Darknet Yolo.

[![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)
[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)


**You only look once (YOLO)** is a state-of-the-art, real-time object detection system. It is implemented based on the Darknet, an Open Source Neural Networks in C. In this project, I improved the YOLO by adding several convenient functions for detecting objects for research and the development community.


<img src="https://raw.githubusercontent.com/vincentgong7/VG_AlexeyAB_darknet/master/output/1.jpg" alt="" width="600"/> <img src="https://raw.githubusercontent.com/vincentgong7/VG_AlexeyAB_darknet/master/output/2.jpg" alt="" width="600"/>

Figure 1. Example of Object Detection using Yolo based on the Darknet.


The added functions are implemented based on **AlexeyAB**  version of **Darknet**. As it is updated frequently, hereby I publish a stable version of AlexeyAB Darknet Yolo with those convenient functions. This repo will also be updated regularly.


## Batch images detector

<img src="https://raw.githubusercontent.com/vincentgong7/VG_AlexeyAB_darknet/yolo_v3/exp/example/vg_darknet_batch_detector.png" alt="" width="60%" />

Figure. The process of batch detecting images in a folder using Yolo based on the Darknet.


The **detector** function in AlexeyAB Darknet only supports a single image at a time. Therefore I added the batch function into this forked repo, which supports detecting images in a folder in one time. In the meantime, it exports information including the name of the image, the detected classes, the confidence and the <span style="color:blue"> **bounding box coordinates** </span> in **JSON** and **TXT** files.
Hope you like it. 

### Github link: [https://github.com/vincentgong7/VG_AlexeyAB_darknet](https://github.com/vincentgong7/VG_AlexeyAB_darknet)

Please also refer to the post for more information:

[https://github.com/pjreddie/darknet/issues/723](https://github.com/pjreddie/darknet/issues/723)

## Update May 07, 2020
1. The new version based on AlexeyAB Yolo v4.
2. Compile without change anything on Linux and Windows. Both are tested.
3. Export the bounding box of detected objects in images to JSON.
4. Export the bounding box of detected objects in images to TXT. 

## Usage

### Command
>./darknet detector batch cfg/coco.data cfg/yolov4.cfg weights/yolov4.weights io_folder sample_imgs/ output/ -out output/result.json -ext_output > output/result.txt

Parameter explain:
1. The input images are: **sample_imgs/**
2. The output images are: **output/**
3. The image name, detected classes, the confidence and the **bounding box coordinates** is saved in: **output/result.txt** and in **output/result.json**

### Installation
1. Clone this project.
2. Download pre-trained weights file into folder **./weights/**. Such as:
[https://bit.ly/yolo_v4](https://bit.ly/yolo_v4)
It is a ZIP file. Unzip it using the password: **jj113.io**


3. Build the project. No need to modify the code either in Linux or in Windows.

	3.1 For linux: Make the project with command in darknet/ folder: 
	>make
	
	3.2 For windows.	
	It can be successfully built on Visual Studio.
	
5. Use the command described above to batch process images.

## Contact
Any questions please let me know.

If you like it, please also let me know.

vincent.gong7[at]gmail.com



<!-- <img src="https://github.com/vincentgong7/VG_AlexeyAB_darknet/blob/master/exp/example/icon_link.png?raw=true" alt="" width="15" valign = "middle"/> [Gong.im](http://gong.im) -->

:palm_tree: [*Gong.im*](http://gong.im)

:floppy_disk: [Guestbook](https://github.com/vincentgong7/VG_AlexeyAB_darknet/issues/7)

<script type="text/javascript" src="//counter.websiteout.net/js/5/4/69/0"></script>
<br>
<div style="float: left;"><script type="text/javascript" id="clustrmaps" src="//cdn.clustrmaps.com/map_v2.js?cl=ffffff&w=600&t=m&d=hUfpL0e-tBg_zcx45xNWS0tq1zo_Jj5POALETOYreCY&co=2d78ad&cmo=3acc3a&cmn=ff5353&ct=ffffff"></script></div>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
