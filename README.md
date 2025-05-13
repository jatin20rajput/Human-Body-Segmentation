Full Body and Brain Tumor Segmentation using U-Net
This project focuses on semantic segmentation of two distinct domains:

Full-body human segmentation from real-world images using the MADS dataset

Brain tumor segmentation from MRI scans using the LGG dataset

Both tasks are implemented using a U-Net-based deep learning architecture in Python (TensorFlow/Keras), aiming to automate complex image segmentation processes for medical and real-world applications.

🚀 Project Goals
Automate full-body human figure segmentation for tasks like background removal and pose estimation.

Accurately identify brain tumor regions in MRI images to support medical diagnosis and treatment planning.

Leverage U-Net architecture to achieve pixel-level precision in image segmentation.

📂 Datasets Used
1. MADS (Human Segmentation) Dataset
Contains 1,192 high-resolution full-body images.

Binary masks for foreground (human) and background.

Used for applications like virtual try-ons, live video editing, and pose detection.

2. LGG Brain MRI Dataset
Contains 2D slices of brain MRIs with labeled tumor regions.

Images preprocessed and resized for model training.

Focused on detecting Low-Grade Glioma tumors.

🧠 Model Architecture
U-Net is used for both segmentation tasks.

Encoder-Decoder structure with skip connections for precise localization.

Binary cross-entropy loss with accuracy as evaluation metric.

Augmentation applied using Keras ImageDataGenerator. 

├── datasets/
│   ├── MADS/                # Full-body images and masks
│   └── BrainMRI/            # MRI images and tumor masks
├
├── train_body_segmentation.py
├── train_brain_segmentation.py

