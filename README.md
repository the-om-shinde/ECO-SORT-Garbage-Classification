# ♻️ ECO-SORT: Real-Time Waste Detection and Classification

A **Machine Learning-based garbage classification system** using YOLO for real-time detection and classification of waste items such as plastic, metal, glass, paper, shoes, and more.

This project provides an **interactive desktop application** with real-time webcam detection and image-based analysis using a modern GUI.

---

## 🚀 Key Features

### 🔍 Real-time Detection

High-speed object detection using YOLO, optimized for low-latency inference.

### 🖼️ Garbage Classification System (GUI - CustomTkinter)

* **Static Image Analysis**

  * Upload and analyze images
  * Display bounding boxes with confidence scores

* **Live Camera Mode**

  * Real-time detection via webcam
  * Continuous frame-by-frame classification

---

### 🧠 Advanced Features

* **Hazard Detection**

  * Identifies potentially dangerous waste (e.g., batteries)

* **Object Tracking**

  * Maintains object identity across frames

* **Noise Filtering**

  * Reduces background interference for better accuracy

---

### 🎨 Modern UI

* Dark theme interface
* User-friendly navigation
* Real-time detection results

---

## 📦 Supported Categories

The model is trained to recognize **10 classes**:

| Class ID | Category   | Type           |
| -------- | ---------- | -------------- |
| 0        | Battery    | Hazardous      |
| 1        | Biological | Organic Waste  |
| 2        | Cardboard  | Recyclable     |
| 3        | Clothes    | Recyclable     |
| 4        | Glass      | Recyclable     |
| 5        | Metal      | Recyclable     |
| 6        | Paper      | Recyclable     |
| 7        | Plastic    | Recyclable     |
| 8        | Shoes      | Recyclable     |
| 9        | Trash      | Non-recyclable |

---

## ⚙️ Installation

### 📌 Prerequisites

* Python 3.8+

---

### 🔧 Setup

```bash
git clone https://github.com/the-om-shinde/ECO-SORT-Garbage-Classification.git
cd ECO-SORT-Garbage-Classification
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the application:

```bash
python main.py
```

---

## 🖥️ Application Features

* Upload images for detection
* Real-time webcam-based classification
* Confidence score visualization
* Bounding box detection

---

## 📊 Sample Output

<p align="center">
  <img src="images/output.png" width="700"><br>
  <b>Real-time garbage detection using YOLO (Paper detected with 89% confidence)</b>
</p>

---

## 📁 Project Structure

```
ECO-SORT-Garbage-Classification/
│
├── assets/              # UI elements
├── images/              # Sample outputs
├── model/               # Model folder (weights not included)
├── experiments/         # Training notebooks
│
├── main.py              # GUI application
├── data.yaml            # Dataset configuration
├── requirements.txt     # Dependencies
└── README.md
```

---

## ⚠️ Important Notes

* Model file (`best.pt`) is **not included** due to GitHub size limitations
* To run the project, place your trained model at:

  ```
  model/best.pt
  ```
* Notebooks are included for experimentation and training purposes

---

## 🧠 Technical Details

* Model: YOLO (Ultralytics)
* Framework: PyTorch
* GUI: CustomTkinter
* Image Processing: OpenCV

---

## 📈 Performance Notes

* GPU significantly improves detection speed
* CPU-only mode works with reduced performance
* Lower confidence thresholds improve tracking stability

---

## 🚀 Future Improvements

* Web-based dashboard (Flask / FastAPI)
* Cloud deployment
* Multi-camera support
* Mobile integration
* Smart waste segregation system

---

## 👤 Author

Om Shinde

---

## 📌 Credits

This project uses open-source tools and pretrained models including YOLO (Ultralytics).
The main implementation, integration, and application development were done by the author.

---
