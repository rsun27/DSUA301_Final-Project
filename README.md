# DSUA301_Final-Project


In this project, we perform human action recognition on images and evaluate the results. Through our implementations, we are able to recognize human’s actions in images and assign labels to each action. We use a top-down approach by first identifying bounding boxes for humans in an image and then analyzing actions in the bounding boxes. 

Therefore, we first implement YOLOv5 for object recognition and crop the human object to improve estimation accuracy. Then, we are going to fine-tune on pretrained Resnet-50 and VGG16 to classify human actions by optimized hyperparameters adjusted by Hyperband. Human Action Recognition is essential in machine learning development, and can be applied on various fields including VR technologies. Besides human actions, the model can also be adjusted and applied on gesture recognition.



https://github.com/ultralytics/yolov5
