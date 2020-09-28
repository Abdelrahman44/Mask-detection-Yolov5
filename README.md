# Mask-detection-Yolov5

This repository uses Yolov5, the small version, to detect masked faces and unmasked faces with high accuracy and high throuput in real time.
the

## Accuracy
Average Precision is a metric used to measure the perfomrance of object detection models for one class. 
Below the mean Average Precision (mAP) is shown for the two classes (masked and unamsked) at 0.5 and 0.5:95 IoU thresholds.

![performance](https://github.com/Abdelrahman44/Mask-detection-Yolov5/blob/master/yolov5/runs/exp5/results.png)




Below are sample images and predictions:


![output1](https://github.com/Abdelrahman44/Mask-detection-Yolov5/blob/master/yolov5/inference/output/0_Concern-In-China-As-Mystery-Virus-Spreads_jpg.rf.3135dfc5feab288d76a4ccfd22dfc5bf.jpg)
![output1](https://github.com/Abdelrahman44/Mask-detection-Yolov5/blob/master/yolov5/inference/output/r1p00017o8171pnq407_jpg.rf.6fd25b7219a249e97f54fcabf2b52726.jpg)
![output1](https://github.com/Abdelrahman44/Mask-detection-Yolov5/blob/master/yolov5/inference/output/w1240-p16x9-0e48e0098f6e832f27d8b581b33bbc72b9967a63_jpg.rf.34ed1e8f70eebdabaf43ab9d40dc1c9b.jpg)
![output1](https://github.com/Abdelrahman44/Mask-detection-Yolov5/blob/master/yolov5/inference/output/RTX7CCFN_jpg.rf.66ed5c5054f30d933d19ab3d56ace004.jpg)
![output1](https://github.com/Abdelrahman44/Mask-detection-Yolov5/blob/master/yolov5/inference/output/r1p00017o8171pnq407_jpg.rf.6fd25b7219a249e97f54fcabf2b52726.jpg)
![output1](https://github.com/Abdelrahman44/Mask-detection-Yolov5/blob/master/yolov5/inference/output/1288126-10255706714jpg_jpg.rf.95f7324cbfd48e0386e0660b5e932223.jpg)
![output1](https://github.com/Abdelrahman44/Mask-detection-Yolov5/blob/master/yolov5/inference/output/shutterstock_1627199179_jpg.rf.8432d033a37b3d142ec4ffcede508c7d.jpg)


## Requirements
After cloning the repo do:
'pip install -r requirements.txt'


## How-to-use

To run inference execute below command

'python detect.py --source ../data/test/images --weights runs/exp6/weights/best.pt --img 640'
You can change --source to:
      * 0  # webcam
      * file.jpg  # image 
      * file.mp4  # video
      * path/  # directory
      * rtsp://170.93.143.139/rtplive/470011e600ef003a004ee33696235daa  # rtsp stream
      * rtmp://192.168.1.105/live/test  # rtmp stream
      * http://112.50.243.8/PLTV/88888888/224/3221225900/1.m3u8  # http stream
