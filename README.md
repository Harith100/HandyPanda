# 🐼 HandyPanda – Gesture-Controlled Mouse with MediaPipe

Control your computer with just your hand!  
**HandyPanda** lets you use real-time hand gestures to move the mouse, click, and scroll — no hardware, just a webcam.

---

## 🚀 Features

- ✋ **Hand Tracking** using MediaPipe Hands  
- 🖱️ **Cursor Movement** via index finger tracking  
- 🤏 **Left Click** – Thumb + Index pinch  
- 👉 **Right Click** – Thumb + Middle pinch  
- 📜 **Scroll Mode** – Fold all fingers and move your wrist up/down  
- 🎯 **Smoothing** and **calibration box** for stable control

---

## 🛠 Tech Stack

- **Python 3**  
- **OpenCV** – for webcam feed and frame processing  
- **MediaPipe** – hand landmark detection  
- **PyAutoGUI** – for controlling mouse actions  
- **NumPy** – for gesture logic and distance calculations

---

## 🎮 How It Works

1. Captures webcam feed in real-time.
2. Uses **MediaPipe** to detect 21 hand landmarks.
3. Interprets gestures:
   - ☝️ Index finger up → Move mouse  
   - 🤏 Thumb & Index pinch → Left Click  
   - 👉 Thumb & Middle pinch → Right Click  
   - ✊ All fingers folded → Scroll mode (wrist controls scroll)  
4. Sends commands using **PyAutoGUI**

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/handypanda.git
cd handypanda
pip install -r requirements.txt
