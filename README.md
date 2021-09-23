# Hand Pose Classification Experiments

Machine learning experiments to train different models to classify hand poses. The experiments are based on the [mediapipe solution](https://google.github.io/mediapipe/solutions/hands.html) for hand landmark detection and the [Handy Interaction App](https://github.com/AntonioEscamilla/HandyInteraction) to record the instances for training.

## Hand Landmark Model
The mediapipe hand landmark model performs precise keypoint localization of 21 3D hand-knuckle coordinates inside the detected hand regions via regression, that is direct coordinate prediction. The model learns a consistent internal hand pose representation and is robust even to partially visible hands and self-occlusions.

![alt text](https://github.com/AntonioEscamilla/images-in-readMe/blob/master/HandPoseClassifier/mediapipe_hand_landmarks.png)

## Training Set
To build a good classifier appropriate pose instances should be collected for training (e.g., “open_hand” and “close_hand”). It’s important that different instances in the dataset cover different camera angles, camera proximities, hand shapes, and pose variations. For this purpose the [Handy Interaction App](https://github.com/AntonioEscamilla/HandyInteraction) runs the mediapipe model on frames comming from a camera connected to the computer and dump predicted pose landmarks to a CSV file.

![alt text](https://github.com/AntonioEscamilla/images-in-readMe/blob/master/HandPoseClassifier/labels_and_poses.png)
