# Object detection(YOLO) on Nvidia jetson TX2

<br />Tensorflow and keras implementation of YOLO algorithm using the on-board camera of TX2.

![alt text](https://github.com/siddharthbhonge/YOLO_with_Nvidia_jetson_TX2/blob/master/demo.png)

##### Demo Link:https://youtu.be/rHyBtfIDGOc

## Getting Started

The neural network was trained on Nvidia Titan X  GPU.This model was later used with nvidia Jetson TX2 Board.
Opencv was used to capture images .

## Prerequisites

1.Python 3.5 <br />
2.Tensorflow 1.5<br />
3.Keras <br />
4.Scikit Learn<br />
5.Open CV 3.4.1<br />


## Theory

##### I.A YOLO algorithm
```
							  Broad Overview
								|
						    Reduce Dimesions of image
								|
		                 probablity of box | box co-rdinates | Probability of each class
								|
							  hard threshold
								|	
							Non max-suppression
								|
							      output



 ```
![alt text](https://github.com/siddharthbhonge/YOLO_with_Nvidia_jetson_TX2/blob/master/yolo.png)


##### I.B  Non-max Supression


![alt text](https://github.com/siddharthbhonge/YOLO_with_Nvidia_jetson_TX2/blob/master/nonmax.png)



##### II. Open CV<br />

1.Open CV installation for ubuntu is pretty standard and done in same way as shown on their website.<br />
2.Installation of Open CV on Jetson TX2 is a bit diffrent.Jetson Hacks has a pretty cool script on his Git repo.This enable open CV on GPU on the Jetson.<br />


##### III.Running on Jetson TX2

This was done using pre-trained model by darknet.Follow the instruction as follows.<br />

![alt text](https://github.com/siddharthbhonge/YOLO_with_Nvidia_jetson_TX2/blob/master/instructions.png)

Then run the test_on_cam.py file.<br />
Uncomment if needed to run on Video.Add video to data folder in .avi format.<br  />

 Download the dataset: https://www.dropbox.com/s/nli1ne8hzkzsyt6/NFPAdataset.zip?dl=0


## Results

Yolo-tiny is a lightweight option with pretty descent accuracy and does not require huge computation resources.Athough a correct and accurate implementation is th YOLO designed above. 

## Authors

* **Siddharth Bhonge** - *Parser /Model* - https://github.com/siddharthbhonge


## Acknowledgments

* Andrew Ng  | Deeplearning.ai<br />

*    Joseph Redmon, Santosh Divvala, Ross Girshick, Ali Farhadi - You Only Look Once: Unified, Real-Time Object Detection (2015)<br />
*    Joseph Redmon, Ali Farhadi - YOLO9000: Better, Faster, Stronger (2016)<br />
*    Allan Zelener - YAD2K: Yet Another Darknet 2 Keras<br />
*    The official YOLO website (https://pjreddie.com/darknet/yolo/)<br />

