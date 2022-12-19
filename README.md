# DSUA301_Final-Project

### Description
Human Action Recognition is essential in machine learning development, and can be applied on various fields including VR technologies. In this project, we perform human action recognition on images and evaluate the results. Through our implementations, we are able to recognize human’s actions in images and assign labels to each action. We use a top-down approach by first identifying bounding boxes for humans in an image and then analyzing actions in the bounding boxes. 

Therefore, we first implement [YOLOv5](https://github.com/ultralytics/yolov5) for object recognition and crop the person object to improve estimation accuracy. Then, we use hyperband to find a good configuration of hyperparameters and fine-tune on pretrained Resnet-50 and VGG16 to classify human actions by optimized hyperparameters. Besides human actions, the model can also be adjusted and applied on gesture recognition.


### Repository Structure

`Object_Detection.ipynb` contains trained models of yolov5 for person detection. The models are trained on [COCO 2017](https://cocodataset.org/#download) dataset. The trained models are in the `yolov5_models` folder. `Action_Recognition.ipynb` includes the code and process for training *ResNet-50* and *VGG16* to classify humans' actions. You can find full images and cropped images in `Dataset`.


### How to execute the code

We recommend executing this code on Google Colab. If you are interested in using trained models to detect **person** object and crop images, you can load the trained YOLOv5 models in the `yolov5_models` folder and follow the code in `Object_Detection.ipynb` to achieve the goal. If you are interested in recognizing human actions, you can run the code in `Action_Recognition.ipynb`.


### Results evaluation

##### ResNet-50
Validation AUC: 0.8658

![alt text](https://github.com/rsun27/DSUA301_Final-Project/blob/main/images/resnet50.png "Logo Title Text 1")

##### VGG16
Validation AUC: 0.8661

![alt text](https://github.com/rsun27/DSUA301_Final-Project/blob/main/images/vgg.png "Logo Title Text 1")

##### Object Detection Result
YOLOv5l: 

![alt text](https://github.com/rsun27/DSUA301_Final-Project/blob/main/images/yolov5l.png "Logo Title Text 1")



##### Full images vs Cropped images (prediction)
Full image:

![alt text](https://github.com/rsun27/DSUA301_Final-Project/blob/main/images/full_image.jpg "Logo Title Text 1")

Crop:

![alt text](https://github.com/rsun27/DSUA301_Final-Project/blob/main/images/cropped_image.jpg "Logo Title Text 1")

Prediction:

![alt text](https://github.com/rsun27/DSUA301_Final-Project/blob/main/images/crop_pred.png "Logo Title Text 1")




