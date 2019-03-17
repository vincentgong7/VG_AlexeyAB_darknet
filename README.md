Updated: Mar 17, 2019
As AlexeyAB updates frequently, hereby I added a stable version of AlexeyAB Darknet with batch images detecting.

Usage:

./darknet detector batch cfg/coco.data cfg/yolov3.cfg weights/yolov3.weights batch exp/in_images/ exp/out_images/ > result/results.txt

Parameter explain:
The input images are: in_images/
The output images are: out_images/
The detection classes with percentage is saved in: results.txt


Make the project with command in darknet/ folder:
make

If you have already did the make, you may do re-make with commands:
make clean


Any questions please let me know.
vincent.gong7[at]gmail.com

Best Regards,
Vincent
