## TASK-1 Color detection 
This code allows you to detect the color of any pixel in an image by selecting it with a double click of the mouse. The program displays the name of the color, as well as its RGB values, in a rectangle on the image. The color names are obtained from a dataset of color names stored in a CSV file.

The code uses the OpenCV library to load and manipulate the image, as well as to detect mouse events. Pandas library is used to read and parse the CSV file. Tkinter library is used to create a file dialog window to select the input image.

The main function in the code is 'draw_function', which is called every time the mouse is double-clicked on the image. This function obtains the RGB values of the selected pixel and sets the 'clicked' flag to True.

The color name and RGB values are then displayed on the image using the 'cv2.rectangle' and 'cv2.putText' functions from OpenCV library. The color name is obtained by comparing the RGB values of the selected pixel with the RGB values of each color in the CSV file and choosing the color with the minimum distance.

The program continues to display the image until the user hits the 'esc' key to close the window.

## Datasets:

Task1 :
https://github.com/codebrainz/color-names/blob/master/output/colors.csv
