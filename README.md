# AI-based Crowd Density Detection for Event Management

## 📚 Overview
This project implements **AI-based crowd density detection** for event management using Python, OpenCV, and YOLOv8. The system detects and tracks people in a video, counts how many people enter and exit through two defined regions, and displays real-time visualization with updated statistics.

---

## 🚀 Key Features
- **YOLOv8 Object Detection:** Detects people in the video.
- **Custom Tracker:** Tracks each person using unique IDs and updates their positions.
- **Entry and Exit Count:** Counts the number of people entering and exiting defined areas.
- **Polygon Area Detection:** Detects movement between predefined areas using polygonal boundaries.
- **Real-time Visualization:** Displays bounding boxes, movement paths, and the entry/exit count dynamically.

---

## 📂 Project Structure
```
/AI-based-crowd-density-detection
├── /tracker.py           # Custom tracking logic
├── /peoplecount1.mp4     # Input video file
├── /coco.txt            # Class labels for YOLO model
├── /README.md           # Project documentation
└── /main.py             # Main script to run the system
```

---

## 📦 Requirements
- Python 3.8+
- Required Libraries:
  ```bash
  pip install ultralytics opencv-python-headless pandas numpy
  ```

---

## 📝 How It Works
1. **Load YOLOv8 Model:** Loads the pre-trained YOLOv8 model (`yolov8s.pt`) and the COCO dataset class names.
2. **Define Areas:** Two polygonal regions are defined to detect people entering and exiting.
3. **Object Detection & Tracking:**
   - YOLOv8 detects people in the frame.
   - The tracker assigns unique IDs to each person and maintains their movement.
4. **Count Entry and Exit:** The system monitors objects passing through the defined regions, and the counts are updated accordingly.

---

## ▶️ Usage
### Clone the repository:
```bash
git clone https://github.com/your-repo/AI-based-crowd-density-detection.git
cd AI-based-crowd-density-detection
```
### Run the project:
```bash
python main.py
```

---

## 📊 Results
- **Entry and Exit Counts:** Displayed on the video with real-time updates.
- **Bounding Boxes:** Show detected persons with unique IDs and movement.
- **Mouse Coordinates:** Get pixel coordinates using mouse movement.

---

## 📧 Contact
For any queries or contributions, contact:
**Raj M** - [kit26.aids45@email.com](mailto:kit26.aids45@email.com)
