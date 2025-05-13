# **Full Body and Brain Tumor Segmentation using U-Net**

This project focuses on semantic segmentation of two distinct domains:

- **Full-body human segmentation** from real-world images using the **MADS dataset**
- **Brain tumor segmentation** from MRI scans using the **LGG dataset**

Both tasks are implemented using a **U-Net-based deep learning architecture** in Python (TensorFlow/Keras), aiming to automate complex image segmentation processes for medical and real-world applications.

---

## 🚀 **Project Goals**

- Automate full-body human figure segmentation for tasks like background removal and pose estimation.  
- Accurately identify brain tumor regions in MRI images to support medical diagnosis and treatment planning.  
- Leverage U-Net architecture to achieve pixel-level precision in image segmentation.

---

## 📂 **Datasets Used**

### 1. **MADS (Human Segmentation) Dataset**

- Contains 1,192 high-resolution full-body images.  
- Binary masks for foreground (human) and background.  
- Used for applications like virtual try-ons, live video editing, and pose detection.

### 2. **LGG Brain MRI Dataset**

- Contains 2D slices of brain MRIs with labeled tumor regions.  
- Images preprocessed and resized for model training.  
- Focused on detecting Low-Grade Glioma tumors.

---

## 🧠 **Model Architecture**

- **U-Net** is used for both segmentation tasks.  
- Encoder-Decoder structure with skip connections for precise localization.  
- Binary cross-entropy loss with `accuracy` as the evaluation metric.  
- Augmentation applied using Keras `ImageDataGenerator`.

---

## 📁 **Project Structure**

├── datasets/
│ ├── MADS/ # Full-body images and masks
│ └── BrainMRI/ # MRI images and tumor masks
├── train_body_segmentation.py
├── train_brain_segmentation.py 


## 🖼️ **Visualizations**

- Comparison of **ground truth** and **model-predicted masks** for both datasets.
- Visual results demonstrate **sharp boundaries**, **clear region segmentation**, and **minimal false positives**.
- Displayed side-by-side to effectively evaluate qualitative performance.

---

## 📌 **Future Improvements**

- Incorporate advanced evaluation metrics like **Dice Score**, **IoU**, **F1-Score**, and **Precision/Recall**.
- Use hybrid loss functions such as **Dice Loss**, **Focal Loss**, or **Tversky Loss** to better handle class imbalance and small region detection.
- Explore architectural variants like **U-Net++**, **Attention U-Net**, and **TransUNet** for improved feature extraction and contextual learning.
- Extend the model to handle **multi-class segmentation** and **3D volumetric data** for detailed medical analysis.

---

## 💡 **Real-World Applications**

### 🏥 **Medical Imaging**
- Tumor localization and segmentation for **early diagnosis**.
- Support in **surgical navigation** and **radiotherapy planning** by accurately mapping tumor boundaries.

### 👕 **Fashion & Retail**
- Enable **virtual try-on experiences** through full-body segmentation.
- Automate **background removal** for e-commerce catalogs and product listings.

### 🧍‍♂️ **Fitness, Gaming & Augmented Reality**
- Real-time **pose estimation** and **gesture tracking** for fitness and rehabilitation apps.
- Creation of **personalized avatars** in AR/VR environments using human body segmentation.
