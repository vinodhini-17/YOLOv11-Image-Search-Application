# 🔍 YOLOv11 Image Search Application

A Computer Vision powered image search application built using **YOLOv11**, **PyTorch**, and **Streamlit**.

This project allows users to process image datasets, generate metadata using object detection, and search images using detected object classes and count thresholds.

---

# 🚀 Features

- YOLOv11 object detection
- Metadata-based image search
- AND / OR search filtering
- Object count threshold filtering
- Bounding box visualization
- Highlight matching classes
- JSON metadata export
- Streamlit interactive UI
- GPU acceleration using CUDA

---

# 🖼️ Application Preview

## Search Engine

- Search images using object classes
- Apply count thresholds
- Choose AND / OR filtering logic

## Results View

- Display matching images
- Show bounding boxes
- Highlight selected classes
- Adjustable grid layout

---

# 🛠️ Tech Stack

- Python 3.11
- YOLOv11
- PyTorch
- Streamlit
- Pillow (PIL)
- CUDA 12.4
- Conda

---

# 📂 Project Structure

```bash
Yolov11_Image_search/
│
├── app.py
├── requirements.txt
├── instruction.txt
├── yolo11m.pt
│
├── src/
│   ├── inference.py
│   ├── utils.py
│
├── data/
├── test/
└── coco-val-2017-500/
```

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/yolov11-image-search.git

cd yolov11-image-search
```

---

# 💻 CPU Setup

```bash
conda create -n yolo_image_search python=3.11 -y

conda activate yolo_image_search

pip install -r requirements.txt
```

---

# 🚀 GPU Setup (Recommended)

```bash
conda create -n yolo_image_search_gpu python=3.11 -y

conda activate yolo_image_search_gpu

conda install pytorch==2.5.1 torchvision==0.20.1 pytorch-cuda=12.4 -c pytorch -c nvidia

pip install -r requirements.txt
```

---

# ▶️ Run Application

```bash
streamlit run app.py
```

Open in browser:

```text
http://localhost:8501
```

---

# 🔎 How It Works

## 1️⃣ Process New Images

- Provide image folder path
- Run YOLO inference
- Generate metadata.json

---

## 2️⃣ Load Existing Metadata

- Load previously generated metadata
- Skip inference step
- Faster searching

---

## 3️⃣ Search Engine

Users can:

- Search by object class
- Apply maximum object count thresholds
- Use:
  - OR mode → Any selected class
  - AND mode → All selected classes

---

## 4️⃣ Result Visualization

- View matching images
- Show bounding boxes
- Highlight matching objects
- Export results as JSON

---

# 📦 Export Results

Filtered results can be downloaded as:

```json
search_results.json
```

Useful for:
- Dataset analysis
- Annotation workflows
- Model retraining

---

# 🧪 Test GPU Support

```python
import torch

print(torch.cuda.is_available())
```

Expected output:

```python
True
```

---

# 📸 Sample Workflow

```text
Input Images
      ↓
YOLOv11 Inference
      ↓
Metadata Generation
      ↓
Search Engine
      ↓
Filtered Results
```

---

# 🎯 Future Improvements

- Semantic image search
- CLIP embedding support
- FAISS vector database integration
- Multi-model support
- Cloud deployment
- User authentication

---

# 👨‍💻 Author

### Vinodhini k

Computer Vision & AI Engineering Project using YOLOv11 and Streamlit.
