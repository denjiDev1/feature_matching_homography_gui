# 🛰️ Satellite Image Matcher & Coordinate Projector

An interactive visual tool for aligning aerial reference and satellite-captured images using feature detection and homography estimation. Designed to assist in coordinate mapping, drone targeting, or change detection across geospatial imagery.

---

## 📸 Project Overview

This project leverages computer vision techniques (like **SIFT** and **homography**) to automatically detect matching features between two satellite or drone-captured images. It provides an intuitive **graphical user interface (GUI)** to display matching points and allows projection of real-world coordinates.

---

## ✨ Core Features

- 🔍 **SIFT-based Feature Extraction** for robust keypoint matching
- 🔗 **FLANN-based Matcher** for efficient and scalable point correspondence
- 🧠 **RANSAC-based Homography Estimation** to handle outliers and transformations
- 🖼️ **GUI-based Interactive Display** for image alignment visualization
- 🌐 **Real-world Coordinate Projection** using known reference markers
- 📷 **Dual Image Selection & Overlay** in a checkerboard-style or side-by-side mode

---

## 🧰 Tech Stack

- **Language:** Python 3.x
- **Libraries:** OpenCV, NumPy, Tkinter
- **Algorithm:** SIFT + FLANN + RANSAC
- **Platform:** Cross-platform (Tested on Windows & Linux)

---

## 🖱️ GUI Interaction

| Action                    | Description                                 |
|---------------------------|---------------------------------------------|
| 📂 Load Reference Image    | Load base aerial/satellite image            |
| 📂 Load Target Image       | Load comparison image (e.g., drone footage) |
| 🧮 Match Features          | Detect and match features automatically     |
| 🛰️ Project Coordinates     | Enter known world coordinates for projection |
| 💾 Export Homography Matrix| Save or reuse the transformation matrix     |

---

## 📂 File Structure

```
.
├── main.py                  # GUI runner
├── matcher.py               # Feature detection & FLANN matcher
├── homography.py            # RANSAC homography computation
├── coordinate_mapper.py     # World coordinate transformation logic
├── ui/                      # GUI assets and layout files
├── assets/                  # Sample satellite and drone images
├── README.md
```

---

## 🏁 How to Run

### 🛠 Requirements

- Python 3.x
- OpenCV: `pip install opencv-python opencv-contrib-python`
- NumPy
- Tkinter (included with most Python distributions)

### ▶️ Launch App

```bash
python main.py
```

Use the GUI to load images and visualize feature matching and projection results.

---

## 🌍 Use Cases

- Satellite-to-Drone Imagery Alignment
- Target Detection & Localization
- Real-Time Mapping and Navigation Systems
- Change Detection for Environmental Monitoring
- Ground Control Point (GCP) Calibration

---

## 🔍 Sample Workflow

1. Load a reference map or satellite image.
2. Load a real-time drone or alternate angle image.
3. Perform feature matching.
4. Homography is computed automatically and applied.
5. Project known coordinates (e.g., from landmarks) into the other image frame.
6. Visualize or export result.

---


## 🚀 Future Enhancements

- 🧭 GPS-integrated coordinate retrieval
- 📐 Zoomable map overlay for fine-tuning
- 📊 Error heatmap for match confidence
- 🌐 Georeferencing module for exporting to GIS systems

---

## 🧠 Learning Outcomes

- Deepened understanding of feature detectors and descriptors (SIFT)
- Practical implementation of geometric transformations
- GUI integration of real-time image processing
- Application of homography for projection and alignment

---

## 📜 License

MIT License. Feel free to use and modify the tool for academic or commercial purposes.

---

🔬 Bridging the gap between vision and geography — one image at a time.
