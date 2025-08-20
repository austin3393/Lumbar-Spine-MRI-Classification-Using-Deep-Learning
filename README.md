# 🧠 Lumbar Spine MRI Classification Using Deep Learning  

## 📌 Project Overview  
This project tackles the **RSNA 2024 Lumbar Spine Degenerative Classification Challenge**, which aims to classify the severity of five degenerative spine conditions using **lumbar spine MRI scans**. The work leverages **deep learning** techniques to automate grading of spinal stenosis and related pathologies, improving diagnostic efficiency and reducing variability in radiology assessments.  

## 🎯 Objectives  
- Develop a **deep learning model** to classify degenerative spine conditions.  
- Preprocess MRI DICOM images into structured datasets suitable for training.  
- Compare **2D CNN** approaches on sagittal and axial slices.  
- Evaluate performance on severity classification tasks (normal, mild, moderate, severe).  

## 🛠️ Methods  
- **Data Preprocessing**  
  - Filtered MRI DICOMs for **T2 sagittal and axial series**.  
  - Generated **slice-based datasets** with metadata (study ID, level, condition, severity).  
  - Applied resizing, normalization, and mini-stack approaches.  

- **Modeling**  
  - Implemented a **2D CNN classifier** in PyTorch.  
  - Designed experiments for **sagittal vs axial views** across conditions.  
  - Used cross-entropy loss and Adam optimizer for training.  

- **Evaluation**  
  - Metrics: Accuracy, F1-score, AUROC.  
  - Compared results across different anatomical views and conditions.  

## 📊 Key Findings  
- Sagittal views were more effective for **neural foraminal stenosis**, while axial views worked better for **subarticular and canal stenosis**.  
- The CNN achieved reasonable accuracy in classifying severity levels, though performance varied by condition.  
- Identified opportunities to expand toward **3D CNNs, transfer learning, and multimodal ensembles** for future work.  

## 🚀 Future Directions  
- Incorporate **3D volumetric modeling** for better anatomical context.  
- Leverage **transformer-based architectures** (Vision Transformers).  
- Improve **data augmentation** and class balancing strategies.  
- Conduct **external validation** on independent MRI datasets.  

## 🧰 Tech Stack  
- **Python, PyTorch**  
- **NumPy, pandas, matplotlib**  
- **pydicom** for medical imaging preprocessing  
- **scikit-learn** for evaluation metrics  

## 📂 Repository Structure  
