# Smart-Traffic-Mangement-system-

A multi-threaded, algorithm-driven simulation project that replicates real-time traffic behavior at a four-way intersection. The system uses adaptive signal logic, vision-based vehicle detection, and prioritization for emergency vehicles to reduce wait time, fuel usage, and improve urban mobility.

---

## 📌 Features

- ✅ **Adaptive Signal Control**: Uses weighted waiting time to dynamically manage signal changes.
- 🚨 **Emergency Vehicle Priority**: Ambulances and fire trucks are detected and prioritized immediately.
- 🔁 **Real-Time Simulation**: Vehicle movement, signal switching, and turning behavior modeled using `Pygame`.
- 🎥 **YOLO-Based Vehicle Detection**: Detects vehicles from real video frames using `YOLOv11`.
- 📉 **Performance Logging**: Tracks wait times, throughput, fuel savings, and more.

---

## 🖼️ Screenshots & Output Samples

- ![Simulation Interface]
- ![Screenshot 2025-06-15 230840](https://github.com/user-attachments/assets/fe7bb22e-3723-44e7-8f82-83b7506541c3)
- ![YOLO Detection Sample]
- ![Screenshot 2025-06-19 213925](https://github.com/user-attachments/assets/08bcf0fc-4f2e-489c-8848-160e0ab8bb48)
- ![Screenshot 2025-06-19 213851](https://github.com/user-attachments/assets/8f3e5479-b51a-491c-b96f-2e8915b584d3)

---

## 📂 File Structure

```
├── opencv.py                  # YOLO video processing and vehicle detection
├── simulation_engine/         # (If applicable) Pygame-based traffic simulator
├── images/                    # Includes icons, vehicle images
├── stats/                     # Simulation logs, graphs
├── traffic2.mp4               # Input traffic video (replaceable)
└── README.md                  # Project description and instructions
```

---

## ⚙️ How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/smart-traffic-signal
cd smart-traffic-signal
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```
> Or manually install:
```bash
pip install ultralytics opencv-python pygame
```

### 3. Run the Detection Code
Ensure you have a traffic video named `traffic2.mp4` in the root folder, then run:
```bash
python opencv.py
```

### 4. Output
- Annotated video will be saved as `processed_video.mp4`.
- Console will display detection and performance metrics.

---

## 🧠 Algorithm Logic (Summary)

1. Detect vehicles using YOLO.
2. Track wait time per vehicle.
3. Calculate weighted wait time per lane.
4. Select green lane based on max weight.
5. Prioritize emergency vehicles when detected.
6. Log simulation stats for analysis.

---

## 🏙️ Use Cases

- Urban traffic signal automation
- Emergency routing optimization
- Smart city development and planning
- AI-based traffic pattern research

---

## 🙌 Acknowledgment

Developed by:  
**Soufik Aktar**  

---

