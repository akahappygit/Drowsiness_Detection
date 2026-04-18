
# 🛑 Driver Drowsiness Detection System

A real-time safety application to detect **driver drowsiness** using computer vision techniques. The system analyzes **eye movements**, **mouth activity**, and **head posture** from webcam input and triggers an alert when signs of fatigue are detected.

---

## 🔍 Overview

This project uses facial landmarks to determine:
- **Drowsiness** based on Eye Aspect Ratio (EAR)
- **Yawning** based on Mouth Aspect Ratio (MAR)
- **Head tilt** using geometric calculations

When drowsiness or inattention is detected, an alert sound is immediately played to regain the driver’s focus.

---

## 🚦 Key Features

- 👁️ **Eye Aspect Ratio (EAR)** – Detects prolonged eye closure
- 👄 **Mouth Aspect Ratio (MAR)** – Detects yawning
- 🧠 **Head Tilt Detection** – Measures unsafe head posture
- 🔊 **Real-time Audio Alerts** – Warns the driver with a beep sound

---

## 🧠 Model Details

- The model is trained using `scikit-learn`
- Facial landmarks are extracted using **MediaPipe FaceMesh**
- Features like EAR, MAR, and head angle are passed to a trained classifier
- The trained `.pkl` model is loaded via `joblib` during runtime

---

## 📁 Dataset

You can access the dataset used for training here:  
🔗 [Google Drive Dataset](https://drive.google.com/drive/folders/1hjdPerTAgYc2ONyXyTWdg-dXamZI0MXS)

---

## ⚙️ How It Works

1. **Webcam Capture** – Continuously captures frames from the webcam
2. **Face & Landmark Detection** – Uses MediaPipe FaceMesh to identify key facial points
3. **Feature Extraction** – Calculates EAR, MAR, and head tilt
4. **Prediction** – The model predicts the driver’s status based on extracted features
5. **Warning System** – Plays an alert sound if driver shows signs of fatigue

---

## 📦 Requirements

Make sure you have the following Python packages installed:

```bash
pip install opencv-python mediapipe scikit-learn joblib numpy
```

---

## ▶️ Run the App

```bash
python main.py
```

> Ensure your webcam is connected and accessible.

---

## 🙏 Acknowledgments

- **MediaPipe** – for real-time face mesh detection  
- **scikit-learn** – for training and evaluating the ML model  
- **Face 5,000 Images Dataset** – used for training and testing

---

## 📄 License

This project is intended for educational and research purposes only.

---

## 🙋‍♂️ Author

**Dhruv Agarwal**  

E-mail: dhruv.agarwal433@gmail.com  

[LinkedIn](https://www.linkedin.com/in/dhruvagrawal433)

**Ayush Kumar Anand**

E-mail: work.ayushkumaranand@gmail.com

[LinkedIn](https://www.linkedin.com/in/ayush-kumar-anand11/)



---

⭐ If you found this project useful, please give it a star and share it!
