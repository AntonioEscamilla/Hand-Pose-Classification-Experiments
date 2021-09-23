# Hand Pose Classification Experiments

Machine learning experiments to train different models to classify hand poses. The training datasets are based on the [mediapipe solution](https://google.github.io/mediapipe/solutions/hands.html) along with the [Handy Interaction App](https://github.com/AntonioEscamilla/HandyInteraction) to record the instances for training.

## Hand Landmark Model
The mediapipe hand landmark model performs precise keypoint localization of 21 3D hand-knuckle coordinates inside the detected hand regions via regression, that is direct coordinate prediction. The model learns a consistent internal hand pose representation and is robust even to partially visible hands and self-occlusions.

![alt text](image.jpg)

## Training Set
To build a good classifier appropriate pose instances should be collected for training (e.g., “open_hand” and “close_hand”). It’s important that different instances in the dataset cover different camera angles, camera proximity, hand shapes, and pose variations.

![alt text](HandPoseClassifier/labels and poses.png)
