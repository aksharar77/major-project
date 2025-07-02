# major-project
# 🧘‍♀️ PoseMaster: Real-Time Yoga Pose Detection and Correction

**PoseMaster** is a deep learning-based yoga assistant designed to help users improve their yoga practice through real-time feedback and posture correction. By leveraging **MediaPipe** and **pre-trained deep learning models**, it detects and analyzes body postures through live video and compares them against reference yoga poses.

---

## 🎯 Objectives

- Develop a real-time yoga assistant using live video input.
- Detect and analyze body posture using **MediaPipe**.
- Compare user poses with ideal reference poses.
- Provide **instant feedback** via visual cues and audio instructions.
- Personalize feedback based on the **user's age group and experience level**.
- Make home-based yoga practice **safer, more effective, and accessible**.

---

## 🛠 Tools & Technologies

| Category               | Tools / Libraries                                      |
|------------------------|--------------------------------------------------------|
| Deep Learning          | TensorFlow, Keras                                      |
| Pose Detection         | MediaPipe, OpenCV (cv2)                                |
| Pre-trained Models     | Xception, VGG16, EfficientNet, DenseNet               |
| Visualization          | Matplotlib, Seaborn                                    |
| Development Environment| Google Colab, Visual Studio Code (VS Code)            |

---

## 🧠 Deep Learning Approach

- Adopted **transfer learning** by fine-tuning pre-trained models:
  - **Xception**
  - **VGG16**
  - **EfficientNet**
  - **DenseNet**
- Used **data augmentation** and **resizing** techniques to improve generalization.
- Training was performed on **Google Colab** using GPU acceleration.
- Evaluated each model using accuracy, precision, recall, and F1-score.
- Best-performing model used for real-time feedback.



## 🗂️ Dataset Overview

- **Total Images**: 
  - **Training**: 1,127
  - **Validation**: 268
- **Total Yoga Poses**: 52
- **Sample Classes**:
  - Bird of Paradise
  - Boat Pose
  - Bound Angle Twist
  - Bound Lotus
- All images were preprocessed with:
  - Resizing to uniform dimensions
  - Rotation, flipping, and zooming for augmentation



## 🔍 Model Training

- All four models were trained for **50 epochs** each.
- Accuracy and confusion matrices were used for performance evaluation.
- Xception model showed superior results and was used in the final system.



## 🎥 Real-Time Feedback System

- Implemented with **MediaPipe** for landmark detection.
- System compares user's posture with reference pose landmarks.
- Provides **live visual feedback**:
  - ✅ **Green**: Correct Pose
  - ❌ **Red**: Incorrect Pose
- Future versions include:
  - **Audio instructions**
  - More detailed feedback on individual joint corrections



## 🚀 Deployment

- Implemented using **Visual Studio Code (VS Code)**.
- Real-time inference integrated with webcam support.
- Frontend displays pose instructions, live feedback, and performance metrics.


## 💡 Future Enhancements

- Add multilingual audio feedback for broader accessibility.
- Improve pose accuracy using temporal smoothing.
- Include warm-up/cool-down sequences and tracking progress over time.
- Deploy as a cross-platform desktop/mobile application.


