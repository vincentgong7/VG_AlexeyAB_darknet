# Extra functions for a forked AexeyAB Darknet repo.

As **AlexeyAB updates** frequently, hereby I added a stable version of AlexeyAB Darknet with extra convenient functions.


## Batch images detector

The **detector** function in AlexeyAB Darknet only support single image. Therefore I added this function into this forked repo. Hope you like it. Please also refer to this post for detail:
https://github.com/pjreddie/darknet/issues/723

### Command
>./darknet detector batch cfg/coco.data cfg/yolov3.cfg weights/yolov3.weights batch exp/in_images/ exp/out_images/ > result/results.txt

### Usage
1. Clone this project.
2. Download pre-trained weights file into foder **./weights/**. Such as: 
https://pjreddie.com/media/files/yolov3-openimages.weights
3. Make the project with command in darknet/ folder: 
>make
4. Use the command described above to perform batch detecting images.

## Contact
Any questions please let me know.  
vincent.gong7[at]gmail.com  
vincentgong.net
