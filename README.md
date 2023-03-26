# CC-MAR-DATA_SCIENCE


## Project description
This project consists of two tasks completed as part of a project work assignment for Code Clause. The first task is an image color detection application that allows users to select an image and identify the color of any portion of the image using OpenCV. The second task is a brain tumor detection model that uses a convolutional neural network (CNN) to classify brain MRI images as either benign or malignant tumors, achieving an accuracy of around 89%.

## Technologies Used
1.  OpenCV (cv2): an open source computer vision and machine learning software library.
2.  Pandas: a data manipulation library used for data analysis and manipulation.
3.  Tkinter: a Python GUI toolkit used for creating graphical user interfaces.
4.  TensorFlow: an open source machine learning framework developed by Google.
5.  Scikit-learn: a machine learning library for Python.
6.  NumPy: a library for working with arrays.
7.  Matplotlib: a plotting library for Python.
8.  Keras: an open source deep learning library written in Python.
9.  Imutils: a library for performing image processing tasks in OpenCV.
10. OS: a Python module that provides a way of interacting with the operating system.
11. ImageDataGenerator: a class in Keras that generates batches of augmented data from image files.



## TASK-1 Color detection 
This code allows you to detect the color of any pixel in an image by selecting it with a double click of the mouse. The program displays the name of the color, as well as its RGB values, in a rectangle on the image. The color names are obtained from a dataset of color names stored in a CSV file.

The code uses the OpenCV library to load and manipulate the image, as well as to detect mouse events. Pandas library is used to read and parse the CSV file. Tkinter library is used to create a file dialog window to select the input image.

The main function in the code is 'draw_function', which is called every time the mouse is double-clicked on the image. This function obtains the RGB values of the selected pixel and sets the 'clicked' flag to True.

The color name and RGB values are then displayed on the image using the 'cv2.rectangle' and 'cv2.putText' functions from OpenCV library. The color name is obtained by comparing the RGB values of the selected pixel with the RGB values of each color in the CSV file and choosing the color with the minimum distance.

The program continues to display the image until the user hits the 'esc' key to close the window.


## TASK-2 Brain Tumor Detection using CNN :
this is the project which allows the user to detect whether the brain tumor is present in the MRI scan or not. Firstly the MRI images with labels are taken from the kaggle. There are in total of 250 images which are then passed for data augmentation so that data can be increased. so, after data augmentation the total images are around 2000.

Now, the images are been cropped and stored and finally trained in the CNN model. this is the architecture of the mode:
![Model_architecture](https://user-images.githubusercontent.com/111417300/227766242-e46a5086-d27e-4940-933f-1faf5f8cd5ef.jpg)

and finally we are getting the accuracy to be around 89%


## Contributors 
https://github.com/pratham180702


## Datasets:

Task1 :
https://github.com/codebrainz/color-names/blob/master/output/colors.csv

Task2 :
https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection
