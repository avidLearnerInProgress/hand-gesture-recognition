Hand Gesture Recognition  
============================

## Detects finger movements of hands and shows appropriate output. Uses **OpenCV** and **Python** for image processing tasks  
  
#### Steps:  

+ *Segment hand region from a real-time video sequence*  
  - Background Subtraction  
  - Motion Detection and Thresholding  
  - Contour Extraction
  
+ *Count fingers*  
  - Get convex hull of the segmented hand region and compute the most extreme points in the convex hull  
  - Get center of palm using extremes points  
  - Using center of palm, construct a circle with the maximum Euclidean distance as radius  
  - Perform bitwise AND operation on thresholded hand image and the circular ROI  
  - Compute count of fingers using the finger slices obtained in previous step  

##### To run the file use:  _**python sudo.py**_  
##### ```diff - *Note: **(Memory Intensive Operation)** This script creates screenshot for every frame captured and stores it in directory 'screenshots'. Hence, there is a little delay during frame capture*````  

#### Screenshots:  
#### ![Screenshot1](https://rawgit.com/avidLearnerInProgress/hand-gesture-recognition/master/screenshots/screenshot_1.png)  
#### ![Screenshot2](https://rawgit.com/avidLearnerInProgress/hand-gesture-recognition/master/screenshots/screenshot_2.png)  
#### ![Screenshot3](https://rawgit.com/avidLearnerInProgress/hand-gesture-recognition/master/screenshots/screenshot_3.png)  
#### ![Screenshot4](https://rawgit.com/avidLearnerInProgress/hand-gesture-recognition/master/screenshots/screenshot_4.png)  
#### ![Screenshot5](https://rawgit.com/avidLearnerInProgress/hand-gesture-recognition/master/screenshots/screenshot_5.png)  









  
