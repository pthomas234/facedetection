# FaceDetection utilizing Python and OpenCV library to detect and evaluate faces using Haar-cascade algorithms.

Detecting faces from webcam:
The first section, we connect the webcam to Colab and capture an image of our face. We then use Haar cascade algorithms to draw a box around the detected faces. 

Source:  
Haar-cascade: https://medium.com/analytics-vidhya/haar-cascades-explained-38210e57970d 


Evaluating the Haar cascade classifier using the IOU metric:
Next section, we download the Wiki dataset, we then use the mat file from the Wiki dataset to locate the face and find the ground truth box of the face in the image. Since some images in the dataset are not valid, we skip them.

We run a loop to detect the face box in the images from the Wiki dataset and evaluate the IOU metric for each image in the dataset. Finally, we generate the average IOU metric over all the images in the dataset.


Sources: 
Image dataset: https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/
Measuring the accuracy of bounding box image: https://blog.mturk.com/tutorial-measuring-the-accuracy-of-bounding-box-image-annotations-from-mturk-ad3dfcdf8aa0
