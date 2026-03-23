## **1. 🏷️ Project Title**

**Computer-Vision-Powered Image Search & Object Detection using YOLOv11**

---

## **2. 📝 Abstract / Introduction**

This project implements a **YOLOv11-based real-time object detection and visual search system**.
Users can upload an image, and the system identifies objects using the **COCO dataset** and retrieves visually similar images using **feature extraction + similarity matching**.

The project includes:

* YOLOv11 inference on CPU/GPU
* Streamlit web deployment
* Conda-based environment setup
* Image search pipeline
* User-friendly UI

---

## **3. 📂 Dataset & YOLO Model Details (COCO)**

### **Dataset: COCO 2017**

* 118K training images
* 5K validation images
* 80 object categories
* Common classes: person, car, dog, cup, laptop, etc.

### **YOLOv11 Model**

* Model Used: **yolo11m.pt**
* Pretrained on COCO dataset
* Supports bounding box detection
* Fast and efficient for real-time inference

---

## **4. 🛠️ Environment Setup**

Install Conda (Anaconda/Miniconda)

```bash
conda create -n yolosearch python=3.10 -y
conda activate yolosearch
```

Install dependencies:

```bash
pip install ultralytics
pip install streamlit
pip install opencv-python
pip install numpy
pip install pillow
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

---

## **5. ⚙️ GPU Installation Steps OR CPU Installation Steps**

### **GPU Setup**

(If you have NVIDIA GPU)

1. Install NVIDIA CUDA Toolkit (11.8 recommended)
2. Install cuDNN
3. Install PyTorch with GPU support:

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

### **CPU Setup**

If no GPU available:

```bash
pip install torch torchvision torchaudio
pip install ultralytics
```

---

## **6. 🖥️ How to Run in VS Code using Conda**

### **Step 1 — Activate Environment**

```bash
conda activate yolosearch
```

### **Step 2 — Run YOLO Inference Script**

```bash
python src/inference.py
```

### **Step 3 — VS Code Tips**

* Select Interpreter → your conda env
* Open integrated terminal
* Run Streamlit or Python scripts

---

## **7. 🌐 How to Deploy using Streamlit**

Run Streamlit app:

```bash
streamlit run app.py
```

Main Features:

* Upload image
* Detect objects using YOLOv11
* Show bounding boxes
* Perform visual similarity search
* Responsive UI

---

## **8. 🖼️ Output Screenshots**

Include these images inside your GitHub repo:

* **UI Screenshot (Streamlit home page)**
* **Detection Output (Image + bounding boxes)**
* **VS Code Terminal showing YOLO inference logs**
* **Similarity search results**



<img width="1813" height="1092" alt="Screenshot 2026-03-19 160346" src="https://github.com/user-attachments/assets/386a2519-d579-4dcf-a978-605c08859ab8" />
<img width="1807" height="1067" alt="Screenshot 2026-03-19 160356" src="https://github.com/user-attachments/assets/32a3fa4e-6f7b-40da-a3f3-de933521118c" />
<img width="1834" height="1081" alt="Screenshot 2026-03-19 160409" src="https://github.com/user-attachments/assets/afd77eaa-9b27-49be-a6d7-4856d1d00bf6" />

---


## **9. 🚀 Enhancements / Innovations Added**

Examples (Edit according to your project):

* Added **visual similarity search** using embedding vectors
* Implemented **GPU-accelerated YOLO inference**
* Built a **Streamlit UI**
* Added **search-by-object-name** feature
* Built **logging + exception handling** system
* Supports **multiple image formats**

---

## **10. 📊 Results & Conclusion**

### **Results**

* Average detection accuracy: **High**
* Response time: **Fast (approx 20–40 ms on GPU)**
* Works on 80 COCO classes
* UI is easy to use and deploy

### **Conclusion**

This project successfully demonstrates a **real-time object detection + image search system** using **YOLOv11**.
The application is optimized for both CPU and GPU and includes a deployable **Streamlit interface** suitable for real-world use.

---
