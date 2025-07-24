# Typing Tutor with Hand Gesture Recognition

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Made with](https://img.shields.io/badge/Built%20With-OpenCV%20%7C%20cvzone%20%7C%20Pygame-blue)

A real-time AI-based typing tutor that uses **hand gesture recognition via webcam** to help users practice proper 10-finger typing. The system detects finger positions on a virtual keyboard, tracks accuracy, and provides instant visual feedback — making it ideal for learning touch-typing interactively.

---

## 🧠 Why This Project?

Traditional typing tutors rely on physical keyboards. This project introduces an **innovative learning experience** using:
- Real-time **hand tracking**
- **Gesture-based input validation**
- A gamified, camera-driven interface for faster muscle memory development

---

## 🚀 Features

- 🧠 Detects correct finger usage for each key
- ⌨️ Virtual keyboard with live overlay
- 🔡 Randomized character prompts to practice
- 📷 Real-time webcam tracking using `cvzone` (built on MediaPipe)
- ✅ Green/red highlights for correct/incorrect inputs
- 📊 Score tracking for typing accuracy

---

## 🛠️ Tech Stack

| Component      | Library / Tool         |
|----------------|------------------------|
| Hand Tracking  | cvzone, OpenCV         |
| GUI Overlay    | Pygame                 |
| Image Handling | OpenCV, NumPy          |
| Language       | Python 3.8+            |

---

## 💻 Installation

### ✅ Requirements

Make sure you have **Python 3.8+** and install the following dependencies:

```bash
pip install -r requirements.txt
```

### `requirements.txt` contents:

```
opencv-python
cvzone
pygame
numpy
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/typing-tutor-hand-gesture.git
cd typing-tutor-hand-gesture
```

### 2. Make Sure This File Exists:

- `Background.png` → The UI layout image (keyboard + score zones)

### 3. Run the App

```bash
python typingTutor.py
```

The webcam will activate and the system will prompt you to type characters using the correct finger.

---

## 🔍 How It Works

1. A **background image** is loaded with a virtual keyboard.
2. **Webcam feed** overlays your hand using OpenCV.
3. **Hand landmarks** are detected using `cvzone` (powered by MediaPipe).
4. The program checks:
   - Finger tip location
   - Key being touched
   - If the correct finger is used
5. Feedback is given instantly:
   - ✅ Correct → Green highlight
   - ❌ Incorrect → Red highlight
6. Scores are updated and displayed in real-time.

---

## 📁 File Structure

```
typing-tutor/
├── typingTutor.py           # Main script with hand tracking + logic
├── Background.png           # Background image with keyboard UI
├── requirements.txt         # Dependencies list
└── README.md                # Project documentation
```

---

## 📌 To-Do / Enhancements

- Add leaderboard or session logs
- Support full words and timed tests
- Add sound feedback (key click / error sound)
- Add left/right hand view toggle

---

## 👤 Author

**Hridey Dalal**  
📧 [hrideydalal1@gmail.com](mailto:hrideydalal1@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/hridey-/)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
