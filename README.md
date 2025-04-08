Image Similarity & Object Detection 🧠📸

This project was developed as part of an academic assignment focused on computer vision techniques, specifically image similarity metrics and object detection using deep learning.

## 📁 Contents

- `Homework6_Combined_Image_Similarity_Object_Detection.ipynb` – Jupyter Notebook containing all code and visualizations.
- `Homework6_Report.pdf` – Written summary of methodology, models used, and results.
- `Bright_Tree.png`, `Dark_Tree.png` – Images used for similarity comparison.
- `Kitchen.jpg`, `StreetView.jpg`, `Zebra.jpg` – Images used for object detection.

## 🧪 Task Overview

### 🔹 Part A: Image Similarity
- **Objective:** Compare two images – *Bright_Tree* and *Dark_Tree* – using:
  - MSE (Mean Squared Error)
  - PSNR (Peak Signal-to-Noise Ratio)
  - SSIM (Structural Similarity Index)
- **Techniques:**
  - Histogram matching
  - Grayscale conversion for SSIM
  - Evaluation before and after enhancement

### 🔹 Part B: Object Detection
- **Objective:** Detect and label objects in three images using a pre-trained Faster R-CNN model.
- **Images:** `Kitchen.jpg`, `StreetView.jpg`, `Zebra.jpg`
- **Model:** `fasterrcnn_resnet50_fpn` from PyTorch
- **Confidence Threshold:** 0.7
- **Output:** Bounding boxes with labels on detected objects

## 📊 Key Results

### Image Similarity
| Metric | Original | After Histogram Matching |
|--------|----------|---------------------------|
| MSE    | 0.0209   | 0.0131                    |
| PSNR   | 16.81 dB | 18.83 dB                  |
| SSIM   | 0.7371   | 0.7720                    |

### Object Detection
| Image       | Detected Objects (Confidence ≥ 0.7)         |
|-------------|----------------------------------------------|
| Kitchen     | bottle, cup, potted plant, dining table, chair |
| StreetView  | car, person, bus                            |
| Zebra       | zebra ×2 (100% confidence)                  |

## 🛠️ Libraries Used

- Python 3.x
- NumPy
- OpenCV
- scikit-image
- Matplotlib
- PyTorch & torchvision

## 📄 License

This project is for academic purposes only.

---

Feel free to fork or star the repo if you find it helpful! ✨
