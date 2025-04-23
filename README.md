
# 🦷 Dental Image Classification using CNN & Transfer Learning

##  Project Overview

This project focuses on the automatic classification of dental X-ray images into the following four categories:

- **Cavity**
- **Fillings**
- **Impacted Tooth**
- **Implant**

I have trained both **custom CNN models** and applied **Transfer Learning (VGG16)** to compare performance. After improvements and fine-tuning, the best accuracy was achieved with the VGG16 model: **83%+** on test data.

---

##  How to Run the Project

### 1️⃣ Train a Custom CNN Model
```bash
python src/custom_cnn_v4.py
```

### 2️⃣ Train with VGG16 Transfer Learning
```bash
python src/vgg16_transfer.py
```

### 3️⃣  Run the Image Prediction GUI
```bash
python src/app_gui.py
```

---


## Dataset Information

- All images have been resized to **224x224 pixels**
- Dataset split into `train`, `valid`, and `test`
- Images are normalized (pixel values scaled between 0 and 1)
- Augmentation is applied to training set because of inconsistency in number of images across the categories:
  - Rotation, shift, zoom, flip, shear

Here is the link to access the Dataset
https://www.kaggle.com/code/banddaniel/dental-x-rays-classification-test-f1-score-0-72


---

## GUI Application

- Load any `.h5` model
- Upload a dental X-ray image
- Predict class and show confidence
- Easy to use, built with `tkinter`

---

To use this Project:
1. Clone the repo
2. Organize data into `data/train`, `data/valid`, `data/test`
3. Run any training or evaluation script from `src/`
4. Use `app_gui.py` to interactively test models

---

