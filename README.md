If the above Jupyter Notebook does not work please try [this URL](https://nbviewer.jupyter.org/github/ajdev-1/garbage-detector/blob/master/garbage_detector.ipynb) which uses Jupyter Notebook Viewer. :blush:

# Garbage Object Detection

In this project, I trained an object detection model that classifies garbage into the different German garbage separation categories.
The data basis of this project consisted on the one hand of a data set created for scientific purposes ([Trashnet](https://github.com/garythung/trashnet)) and on the other hand of a small data set that I created and labeled myself.

# Objective
Incorrect waste separation and high rates of misdirected waste have a negative impact on different areas. On the one hand, this harms the environment and, on the other, it leads to increased costs for recycling companies.
<br/><br/>
Accordingly, this project trained an object detection model to help people in private households decide on which way to dispose an object.
<br/><br/>
The development of this app was not part of this project. This project only dealt with the implementation of a first object detection PoC.
For this first PoC I tried to classify objects into the following classes:

- Glass
- Yellow container (German waste system)
- Paper


# Technology
The pipeline (Jupyter Notebook), all data handling and training of the models was done in Google Colab. By connecting Google Colab with Google Drive, it was possible to perform the project from different computers, independent of the operating system. I only had to upload the required data to Google Drive.

Transfer Learning was used to train the model. Thus, I chose a MobileNet architecture ([TensorFlow 2 Detection Model Zoo](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md)), which is especially useful for use on mobile devices.

# Results
Due to the too small amount of data, I was not able to train a model that could be used in private households. Nevertheless, this PoC showed that a sufficiently large amount of data definitely offers the possibility for a usable model.

The below images show positive/ good results of my object detection model. But these objects were also likely to overfit during the training process...

![image](https://user-images.githubusercontent.com/38671044/119031418-5ca81e80-b9ab-11eb-9442-1ac5daea6cea.png)

![image](https://user-images.githubusercontent.com/38671044/119032243-3fc01b00-b9ac-11eb-8416-f2bd9f9bf689.png)




