# DSUA301_Final-Project

### Description
Human Action Recognition is essential in machine learning development, and can be applied on various fields including VR technologies. In this project, we perform human action recognition on images and evaluate the results. Through our implementations, we are able to recognize human’s actions in images and assign labels to each action. We use a top-down approach by first identifying bounding boxes for humans in an image and then analyzing actions in the bounding boxes. 

Therefore, we first implement [YOLOv5](https://github.com/ultralytics/yolov5) for object recognition and crop the person object to improve estimation accuracy. Then, we use hyperband to find a good configuration of hyperparameters and fine-tune on pretrained Resnet-50 and VGG16 to classify human actions by optimized hyperparameters. Besides human actions, the model can also be adjusted and applied on gesture recognition.


### Repository Structure

