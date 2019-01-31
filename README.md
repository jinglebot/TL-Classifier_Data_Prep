# Traffic Light Detection Data Preparation Sub-Project

### Project Description:

* Data exploration and analysis of a set of traffic light images taken from
* LISA Traffic Light Database by MarkP.Philipsen, MortenB.Jensen, AndreasMøgelmose, ThomasB.Moeslund and MohanM.Trivedi
* for training  on Faster RCNN Inception v2 Coco
* Image folder dayClip3. 643 frames 1280 x 960
* Tensorflow 1.12, CUDA 9.0, CuDNN 7.3.1, Anaconda environment
* Intel Core i7, Nvidia GeForce 845M 

### Tidbits to take note:
- Cannot use filename as image name because it's not unique. I used the file index number to make a new name instead.
- Images are small when converted to JPG. ~ < 200 KB

### Goals:
- Convert images in a folder from PNG to JPG
- Give each image a unique identifier as filename
- Split the image list - 80% for training, 20% for testing
- Transfer the images to their respective folders 
- Create a new list with the corresponding data required by the RCNN classifier:
- 	file_name, width, height, class, xmin, ymin, xmax, ymax
- Transfer list to CSV files 


