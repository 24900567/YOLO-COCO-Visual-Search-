# YOLOv11 COCO Visual Search

A Streamlit-powered application for object detection and visual search using YOLOv11 on COCO dataset images.

## Features
- YOLOv11 object detection inference on image directories
- Metadata generation and storage (JSON)
- Advanced search: OR/AND class logic, count thresholds
- Interactive Streamlit UI with bounding boxes
- Grid results view with hover effects
- Export search results

## Quick Start

### CPU
```bash
conda create -n yolo_image_search python=3.11 -y
conda activate yolo_image_search
pip install -r requirements.txt
streamlit run app.py
```

### GPU
```bash
conda create -n yolo_image_search_gpu python=3.11 -y
conda activate yolo_image_search_gpu
conda install pytorch==2.5.1 torchvision==0.20.1 pytorch-cuda=12.4 -c pytorch -c nvidia
pip install -r requirements.txt
streamlit run app.py
```

## Usage
1. **Process images**: Point to image directory + yolo11m.pt model
2. **Load metadata**: From existing JSON
3. **Search**: Select classes, mode (OR/AND), optional count thresholds
4. **Results**: Grid with BBs, highlights, export JSON

## Dataset
- COCO 2017 val subset (500 images) gitignored - download separately
- Place in `coco-val-2017-500/`

## Files
- `app.py`: Main Streamlit app
- `src/`: Inference, utils, config
- `configs/default.yaml`
- `yolo11m.pt`: YOLOv11 medium model

## CUDA Guide
- [Linux](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/)
- [Windows](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/)
