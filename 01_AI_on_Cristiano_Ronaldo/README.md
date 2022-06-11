# AI on Cristiano Ronaldo
**Wonder how AI could help us to reveal the secret of Cristiano Ronaldo?!**
|   |   |   |
|---|---|---|
|<img src="https://user-images.githubusercontent.com/40123599/172683240-c60f2fb1-c80e-4d6b-bcd5-eea9358f5045.jpg" width="250" height="250">|<img src="https://user-images.githubusercontent.com/40123599/172683871-5922b438-cf00-4658-b4cc-2a26c0c140d3.gif" width="250" height="250">|<img src="https://user-images.githubusercontent.com/40123599/172684491-43e42457-8976-4fdf-8ecf-1318b10debf3.png" width="250" height="250">|


# Human Pose Estimation
### Network comparsion
|Network|2D/3D|Single/Multiple Pose|Key-points|Method|
|---|---|---|---|---|
|MoveNet.SinglePose|2D|Single Pose|17|Bottom-up|
|MoveNet.MultiPose|2D|Multiple Pose|17|Bottom-up|
|BlazePose|2D|Single Pose|33| |
|BlazePose GHUM|3D|Single Pose|33| |
|PoseNet|2D|Multiple Pose|17|Bottom-up|
|OpenPose| |Multiple Pose|137|Top-down|


### **MoveNet** 
- GitHub: 
  - https://github.com/tensorflow/tfjs-models/tree/master/pose-detection/src/movenet
- Tensorflow Hub
  - [MoveNet.SinglePose.Lightning](https://tfhub.dev/google/movenet/singlepose/lightning/4)
  - [MoveNet.SinglePose.Thunder](https://tfhub.dev/google/movenet/singlepose/thunder/4)
  - [MoveNet.Mulitpose.Lightning](https://tfhub.dev/google/movenet/multipose/lightning/1)
- Tutorial:
  - https://www.youtube.com/watch?v=KC7nJtBHBqg  

- Useful References
  - Articles - [Next-Generation Pose Detection with MoveNet and TensorFlow.js](https://blog.tensorflow.org/2021/05/next-generation-pose-detection-with-movenet-and-tensorflowjs.html)
  - MoveNet Post-Processing Steps 
    ![image](https://user-images.githubusercontent.com/40123599/173198162-249b5545-4fe3-42f7-9430-797103c02384.png)

### **BlazePose GHUM** 
- Useful References
  - Articles - [3D Pose Detection with MediaPipe BlazePose GHUM and TensorFlow.js](https://blog.tensorflow.org/2021/08/3d-pose-detection-with-mediapipe-blazepose-ghum-tfjs.html)

![TF image 2](https://user-images.githubusercontent.com/40123599/173200278-6eade188-2f43-4c21-8ec6-855ebed1f2c4.gif)

**Other:**  
- Network
  - [MoveNet Vs BlazePose vs PoseNet](https://github.com/tensorflow/tfjs-models/tree/master/pose-detection)
  - [CenterNet](https://github.com/xingyizhou/CenterNet)  
    Object detection, 3D detection, and pose estimation using center point detection:
  - [TensorFlow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection)
  
 
# Bottom-up vs. Top-down methods
All approaches for pose estimation can be grouped into bottom-up and top-down methods.

- Bottom-up methods estimate each body joint first and then group them to form a unique pose.
- Top-down methods run a person detector first and estimate body joints within the detected bounding boxes.

