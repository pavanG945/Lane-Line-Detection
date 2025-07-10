
# 🚗 Lane Line Detection System

This project detects lane lines in road videos using computer vision techniques with OpenCV and MoviePy. It features a user-friendly GUI built with Tkinter that plays both input and processed video streams simultaneously, showcasing real-time lane detection.

## 📌 Features

- Lane detection using color filtering, edge detection, and Hough Transform.
- Video processing and smoothing to improve detection accuracy.
- GUI display with real-time comparison (input vs output).
- Supports video file input and displays processed output side by side.

## 🧠 Techniques Used

- **Color Space Masking**: HSV thresholding to isolate yellow and white lanes.
- **Edge Detection**: Canny edge detector to identify edges.
- **ROI Filtering**: Region of Interest (polygon masking).
- **Hough Transform**: To detect lines in edge map.
- **Smoothing Algorithm**: Frame-by-frame averaging to stabilize lines.

## 📂 Project Structure

```
📁 LaneLineDetection/
├── lanelinedetection.ipynb      # Development notebook
├── main.py                      # Core lane detection logic
├── gui.py                       # GUI for video visualization
├── input2.mp4                   # Input road video (add your file)
├── output2.mp4                  # Output with detected lanes
├── logo.png                     # Logo used in GUI (optional)
```

## 🚀 How to Run

1. **Install Dependencies**:

```bash
pip install opencv-python numpy matplotlib moviepy Pillow
```

2. **Place your input video** in the project directory as `input2.mp4`.

3. **Run the Application**:

```bash
python gui.py
```

The GUI will open and display two video windows: the original video on the left and the processed output with detected lane lines on the right.

## 🛠️ Customization

- Adjust color thresholds in `main.py` to fine-tune yellow/white detection.
- Modify Hough Transform parameters for different road environments.
- Update smoothing factor `α` for more/less stable line rendering.

## 📽️ Demo Preview

<img src="output2.mp4" alt="Lane Detection Output Video" width="500"/>

> (Ensure you upload the demo video on GitHub or embed a link via YouTube/GIF)

## 👤 Author

- **Pavan Gembali** – [LinkedIn](#) | [GitHub](#)

---

Feel free to fork, improve, and adapt for your autonomous driving or video analysis projects!
