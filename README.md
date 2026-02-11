# Face Recognition System (Project #03)

The third project in my **AI/ML Learning Path**. This project steps into the domain of biometric identification by combining face detection and recognition algorithms.

## 📌 Overview
This system identifies individuals in a real-time video feed. It uses a two-stage process: first, locating a face within the frame, and second, classifying that face against a trained dataset using the Fisherface algorithm.

## 🛠️ Tech Stack
* **Language:** Python
* **Library:** OpenCV
* **Algorithms:** * **Haar Cascade (Frontal Face):** For real-time face detection.
    * **Fisherface (LDA-based):** For facial feature extraction and identification.

## ⚙️ How It Works
1. **Data Collection:** A script captures multiple grayscale images of a specific person to build a training dataset.
2. **Detection:** The Haar Cascade classifier scans the frame to find the coordinates of human faces.
3. **Training:** The Fisherface Recognizer trains on the dataset, using Linear Discriminant Analysis (LDA) to maximize the ratio of between-class scatter to within-class scatter.
4. **Recognition:** The model predicts the ID of the detected face and provides a confidence score.

## 🚀 Quick Start
1. **Prepare Data:** Run the data collection script to capture your face images.
2. **Train Model:** Run the training script to generate the `trainer.yml` file.
3. **Run Recognition:**
   ```bash
   python face_recognizer.py
4. The system will label the detected face with the trained name or "Unknown" if the confidence threshold isn't met.

*Progress: Successfully moved from feature detection to individual identification.*
