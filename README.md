# Typing Tutor with Hand Gesture Recognition

This project is a webcam-based AI typing tutor that helps users improve their 10-finger typing skills using real-time hand gesture tracking. The system evaluates whether the user is pressing the correct key with the correct finger based on standard typing rules, providing immediate visual feedback and maintaining score tracking.

## Project Overview

Typing Tutor uses computer vision techniques to overlay a virtual keyboard and detect finger positions through a webcam. When the program prompts a character, the user must use the correct finger and gesture to press it. The system highlights whether the attempt was correct or incorrect based on both position and finger usage.

This project is useful for:
- Teaching correct finger-to-key mappings
- Practicing typing without a physical keyboard
- Enhancing motor memory using visual learning

## Features

- Virtual keyboard rendered on screen
- Random character prompts for the user to type
- Real-time hand tracking using a webcam
- Finger identification and location mapping
- Visual indicators for correct and incorrect attempts
- Real-time score tracking for correct and wrong responses

## Requirements

To run the project, you must have Python 3.8 or higher and the following Python packages installed:

- opencv-python
- numpy
- pygame
- cvzone

You can install all dependencies using the command:

```bash
pip install -r requirements.txt
````

## Getting Started

1. Clone the repository or download the project files.
2. Ensure `Background.png` is in the root directory. This image contains the UI layout with the virtual keyboard and score areas.
3. Run the script using:

```bash
python typingTutor.py
```

4. Follow the prompts on the screen and place your hands in the webcam view.

## File Structure

```
typing-tutor/
├── typingTutor.py           # Main script with application logic
├── Background.png           # Background layout with keyboard and score zones
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

## How It Works

* The webcam feed is projected onto a background image containing the keyboard layout.
* Hand landmarks are detected using `cvzone` (built on MediaPipe).
* Finger tips are tracked and mapped to the warped keyboard image.
* The program evaluates whether the right finger is placed over the prompted key using bounding boxes.
* Based on the detection, a green or red overlay indicates success or failure.
* Scores are updated in real-time and displayed on the interface.

## License

This project is licensed under the MIT License.
