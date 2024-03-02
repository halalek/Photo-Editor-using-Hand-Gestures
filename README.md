# Photo Editor using Hand Gestures

The project aims to build a desktop application that uses hand gestures to modify images, with the aim of dispensing as much as possible with the current traditional means. 

Through the program, the image is opened, modified, and then saved.

This is done using image processing techniques, taking into account different lighting conditions, so that the user enters a Live Stream video in real time through the computer camera, and hand gestures and hand positions are recognized as needed.

## The project was built in several stages:
starting with recognizing the hand and its movement, 

then moving on to tracking the position of the hand, 

and finally implementing some transformations on the image based on specific movements of the hand.

![image](https://github.com/halalek/Photo-Editor-using-Hand-Gestures/assets/112726630/26de4333-1da2-4b19-8772-a163691759ba)


## The method of work:
### 1-On the user side:
• A video is entered via the computer camera that includes hand movement

• The possibility of performing some geometric transformations on an image through hand movements

That is (Translate - Rotate - Scale - Warp - Skew)

• The ability to draw on the image and modify it through specific movements

(Erase the drawing with the Eraser Tool - Change the size of the Brush Tool/Eraser Tool - Change the color of the Brush Tool/Eraser Tool)

• Possibility of saving the image

               




   ### 2-From the algorithm side:
• Identify the shape of the hand from the video

• Recognizing hand movement

• The ability to draw a group of dots that express the process of recognizing a position or gesture.

• Possibility of tracking hand position.

• Executing user commands such as geometry and drawing transformations and applying them to the image


## Algorithms used :
### 1-Hand recognition :
SkinMask is applied to the hand by detecting skin within the range of lower and upper pixel values in the color space
Then, to discover and draw the convexity of the hand, and to identify the fingers and their number, the law of cosines is used by measuring the angle between each two fingers.
Where the bottom of the gamma is less than 90 the identification is made on the keyboard
![image](https://github.com/halalek/Photo-Editor-using-Hand-Gestures/assets/112726630/99a0684d-e027-49f0-8f0a-1613dabdd120)


### 2-Back projection :
We explained in the previous step how the hand was identified by recognizing skin color, but the hand and face will also be recognized. This procedure is incorrect, so we have several solutions, including: The Back Projection algorithm will be used.
   It is one of the applications that relies on Histogram technology
It is used to segment the image or search for objects of interest in the image. It creates an image of the same size (for each channel) as our input image, where each pixel corresponds to the probability that this pixel belongs to our object. The resulting image will have more white interest compared to the remaining part. Back projection is a way to record how well pixels in a given image fit the distribution of pixels in a histogram model. We can calculate a histogram model for a feature in back projection and then use it to find this feature in an image.

![image](https://github.com/halalek/Photo-Editor-using-Hand-Gestures/assets/112726630/56320a9e-cdd5-4274-aa41-527c485364c6)

### 3-Tracking :
The movement of the hand is tracked by drawing certain points on the hand, such as the red dots shown in the picture, and by tracking these points, the movement of the hand is tracked

## Ex:

![image](https://github.com/halalek/Photo-Editor-using-Hand-Gestures/assets/112726630/34e54203-2d53-4332-aa5e-c87c4a94f85b)

![image](https://github.com/halalek/Photo-Editor-using-Hand-Gestures/assets/112726630/1bef1a07-cc9a-498e-9730-5a4939fbd46c)





