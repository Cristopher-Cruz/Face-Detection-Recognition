# Face-Detection-Recognition

### File 1 : faceDetection.py - face detection on loaded image
How to run : open file and run on IDE that supports python

How to quit : press 'q' on pop-up frame to close window and exit program

### How it works : 
1. Loads specified image into the program
2. Converts image to grayscale  
3. Uses haar cascades algorithm to detect faces
4. Window will open with frame around the face detected

The script uses **openCV** and the **haarcascade** algorithm

### Issues you might encounter : 
- Make sure the image file is in the same directory as the faceDetection.py script
- If the image file is corrupted or not in the correct format, the program will be unable to read it
- Even if the file extension is valid, the image itself might not be. You might need to convert it again (try : [image.online-convert.com](https://image.online-convert.com))

![image 1](res1.png)




### File 2 : faceRecognition.py - real time face recognition
How to run : open file and run on IDE that supports python

How to quit : press 'q' on live webcam window to close window and exit program

How it works : 
1. Loads images from a specified directory
2. Encodes images from step 1
3. Opens webcam and encodes the current live feed
4. Checks if there is a match between the encoded images and the live frames encoded

The script uses **openCV** and the **face_recognition** api 
### Issues you might encounter : 
- Make sure the images loaded to train the program are in the correct folder specified by the script. In this script, the image path is set to a folder named 'faces', in the same directory where the 'faceRecognition.py' script resides
- Do not remove code lines that remove '.DS_Store' from image path. See the following [post](https://stackoverflow.com/questions/47645115/oserror-cannot-identify-image-file-dataset-ds-store) on stackoverflow for reference

![image 1](res3.png)
