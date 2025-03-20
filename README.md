# Hand Gesture Recognition using OpenCV and MediaPipe

##  Project Overview
This project is a **real-time hand gesture recognition system** that uses **OpenCV** and **MediaPipe Hands** to detect and recognize various hand gestures via a webcam feed. The system detects 21 key hand landmarks from the processed video frames and can recognize hand gestures from predefined gestures while labeling key parts of the hand.

##  Features
- It processes gestures in **real-time** with a webcam.
- Detects **hand landmarks** (21 key points on the hand).
- Recognizes gestures for a few common hand gestures.
- Supports **many hands**, labeling each of them independently.
- Identifies key parts of the hand: thumb, fingers, wrist, etc.
- Displays the recognized gesture on the screen in **real-time**.

##  Recognized Gestures
| Gesture | Description |
|---------|------------|
|  **Thumbs Up** | In this gesture, only the thumb points up, showing approval. |
|  **Victory Sign** | Both the index finger and middle finger are extended. |
|  **Open Palm** | All fingers except for the thumb are extended. |
|  **Unknown Gesture** | Any gesture that does not correspond with the above. |

##  Project Structure
```
├── hand_gesture_recognition.py  # Main script
├── README.md                    # Documentation
├── requirements.txt              # Dependencies
```

##  Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repo/hand-gesture-recognition.git
   cd hand-gesture-recognition
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On macOS/Linux
   venv\Scripts\activate      # On Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

##  Usage
1. **Run the script:**
   ```bash
   python hand_gesture_recognition.py
   ```
2. A webcam window will pop up, which will detect your hand and recognize gestures.
3. Press the key **'q'** to exit.

## 🔬 How It Works
1. Captures frames from a **webcam.**
2. **Converts frames from BGR to RGB** for processing through **MediaPipe Hands**. 
3. Detects **hand landmarks** and infers the **positions of fingers**.
4. Classifies the hand into a **predefined gesture** (Thumbs Up, Victory Sign, Open Palm, or Unknown).
5. **Displays** the label of the recognized gesture and key parts of the hand in real-time.
6. Processes the frames as long as the user has not pressed **'q'**.

##  Future Improvements
- Add more gestures (fist, pointing, OK sign).
- Add commands on gestures (volume control, scrolling, etc.).
- Improve accuracy with deep learning models.
- Support **mobile** as well.

##  License
The project is licensed under the **MIT License**; feel free to modify and make improvements from there!


