# U-Net-Convolutional-Networks-for-Biomedical-Image-Segmentation


# Biomedical Image Segmentation using U-Net

Deep learning project for biomedical image segmentation using a U-Net based architecture.  
The model predicts pixel-wise masks from medical / microscopy images.

---

## 📌 Project Overview
This repository contains training and inference code for performing semantic segmentation on biomedical images.

Segmentation means assigning every pixel to either:
- foreground (object of interest)
- background

The project is suitable for learning medical imaging pipelines and experimenting with encoder–decoder CNNs.

---

## 🧠 Model Architecture
We use the **U-Net** convolutional neural network.

U-Net consists of:

- Encoder (downsampling path) → captures context
- Bottleneck → deepest features
- Decoder (upsampling path) → precise localization
- Skip connections → help recover fine details

It is widely used in:
- cell segmentation  
- organ detection  
- tumor localization  

---

## 📂 Dataset
Dataset is available on Google Drive.

👉 Images & masks are paired for supervised training.

Expected format:
dataset/
images/
masks/



### Download
Dataset folder:  
<https://drive.google.com/drive/folders/1nczFqDpCEHPVwvEwVDEcMp4DJa1Oh5XO?usp=drive_link>

---

## 💾 Pretrained Model Weights
You can download trained weights from:

<https://drive.google.com/file/d/1xPPObKf9ogjKL4tjux7MUrIBtDU7xHca/view?usp=drive_link>


---

## ⚙️ Installation

1️⃣ Clone the repository

git clone https://github.com/ADITYA-SUNKAVALLI/U-Net-Convolutional-Networks-for-Biomedical-Image-Segmentation.git
cd U-Net-Convolutional-Networks-for-Biomedical-Image-Segmentation

2️⃣ Create virtual environment

Windows
python -m venv venv
venv\Scripts\activate

Linux / Mac
python -m venv venv
source venv/bin/activate

3️⃣ Install dependencies

If requirements.txt is available:
pip install -r requirements.txt

If not, install the main libraries manually:

pip install torch torchvision numpy matplotlib opencv-python tqdm

▶️ Training

Example:

python train.py


Inference / Prediction
python predict.py

🧩 Tech Stack

Python

PyTorch

OpenCV

NumPy

Matplotlib





