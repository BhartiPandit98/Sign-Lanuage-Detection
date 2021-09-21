# Sign-Lanuage-Detection
## Introduction
A custom object detection model is built to predict 4 different sign language gestures, built using Tensorflow Object Detection API.

## Dataset and Model
* Images was generated using web cam using OpenCV VideoCapture method. Four different sign hand gestures were captured and bounding boxes around them were created using LabelImg.
* Transfer learning was performed on a MobileNet V2 model from Tensorflow Model Zoo. The model was trained using self generated images. The checkpoints were generated and used to store the final model.
* NVIDIA CUDA and cuDNN was used to be able to use GPU to train the model. Tensorflow GPU was also used.
* The model was tested on the training images. Along with this the testing was also done in real time through webcam using OpenCV. 
* The model gave an accuracy of 0.75 on the testing images. Alongside, It was also able to detect accurately and fastly in real time.
* The model gave a precision of 0.7 and recall of 0.71 on the testing data.

## Deployment of the model
* The model was deployed using Tensorflow JS.
* IBM cloud was used to host the model. IBM Bucket was created and the model was host on the cloud
* The model was converted to Tensorflow JS and the json and other model files were uploaded in the Bucket.
* VS Code was used to manipulate the JavaScript file and make connection to the cloud. Finally VS Code was used to start the server.
