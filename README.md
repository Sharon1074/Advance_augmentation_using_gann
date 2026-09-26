# AdvanceAugmentation – Rice Leaf Disease Classification

A deep-learning image augmentation project for **rice leaf disease classification** using a proposed **Advance GAN-based augmentation approach** combined with traditional image transformations.

The project focuses on addressing **limited training data** in agricultural image classification by generating additional training samples and evaluating their effect on CNN classification performance.

---

## 🎥 1. Project Demo

▶️ **[Watch the Complete Project Demo on YouTube](https://youtu.be/ykvGh5tc2_Y)**

---

## 📌 2. Project Overview

Deep learning models generally require sufficient training data to achieve reliable classification performance. In agricultural applications, collecting and labeling large datasets can be difficult.

This project investigates image augmentation techniques for **rice leaf disease classification** using a dataset containing three disease classes.

Three experiments are performed:

1. **Without Augmentation**
2. **Traditional Augmentation**
3. **Proposed Advance GAN Augmentation**

The resulting datasets are used to train CNN-based classifiers and evaluate their performance.

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 🎯 3. Objective

The main objective of this project is to investigate whether increasing training-data diversity through image augmentation can improve rice leaf disease classification.

The proposed approach combines:

- CNN-based feature extraction
- GAN-based image generation
- Traditional image transformations
- Rotation
- Flipping

The generated images are then used to train a CNN classifier.

---

## 🌾 4. Dataset

The project uses the **Rice Leaf Diseases / Rice Health Crop dataset**.

### Disease Classes

- Bacterial Leaf Blight
- Brown Spot
- Leaf Smut

### Dataset Details

- **3 disease classes**
- **40 images per class**
- **120 original images in total**

### Dataset Source

**Kaggle:**  
https://www.kaggle.com/datasets/vbookshelf/rice-leaf-diseases

---

## 💡 5. Proposed Approach

The proposed **Advance GAN augmentation approach** combines traditional image transformations with CNN and GAN-based image generation.

### Workflow

```text
Original Rice Leaf Images
          │
          ▼
Traditional Transformations
     Rotation / Flipping
          │
          ▼
CNN Feature Extraction
          │
          ▼
GAN-based Image Generation
          │
          ▼
Synthetic Image Samples
          │
          ▼
Advance Augmented Dataset
          │
          ▼
CNN Classifier
          │
          ▼
Disease Classification
```
📊 7. Results / Evaluation

The three experiments are evaluated using:

Metric	Purpose
Accuracy	Overall classification performance
Precision	Correctness of positive predictions
Recall	Ability to identify relevant samples
F1-Score	Balance between precision and recall
Confusion Matrix	Class-wise prediction analysis
Reported Results

The original project recorded the following results:

Experiment	Accuracy
Without Augmentation	83.33%
Traditional Augmentation	96.48%
Advance GAN Augmentation	98.21%

The original project documentation reports that the proposed Advance GAN approach achieved the highest recorded accuracy among the three experiments.

Note: Because the notebook uses randomized shuffling and train/test splitting without a fixed random seed, rerunning the notebook can produce different evaluation results. The values above represent the originally recorded project results.

🛠️ 8. Technology Stack
Programming Language
Python
Deep Learning
TensorFlow 1.14.0
Keras 2.3.1
Convolutional Neural Networks (CNN)
Generative Adversarial Networks (GAN)
Computer Vision
OpenCV
Pillow
Data Processing
NumPy
Pandas
Machine Learning
Scikit-learn

Used for:

Train/Test Split
Accuracy
Precision
Recall
F1-Score
Confusion Matrix
Data Visualization
Matplotlib
Seaborn
Development Environment
Jupyter Notebook
Jupyter HTML Export
📁 9. Project Structure
AdvanceAugmentation/
│
├── AdvanceAugmentation.ipynb
│   └── Complete Jupyter Notebook implementation
│
├── AdvanceAugmentation.html
│   └── Saved notebook with recorded outputs
│
├── README.md
│
├── requirements.txt
│
├── Gan/
│   ├── __init__.py
│   ├── layer_utils.py
│   ├── losses.py
│   ├── model.py
│   └── utils.py
│
├── Dataset/
│   ├── Bacterial leaf blight/
│   ├── Brown spot/
│   └── Leaf smut/
│
├── TraditionalAugmentation/
│   ├── Bacterial leaf blight/
│   ├── Brown spot/
│   └── Leaf smut/
│
├── AdvanceAugmentData/
│   ├── Bacterial leaf blight/
│   ├── Brown spot/
│   └── Leaf smut/
│
├── model/
│   ├── generator.h5
│   ├── without_gan_weights.hdf5
│   ├── traditional_gan_weights.hdf5
│   ├── advance_gan_weights.hdf5
│   ├── 22advance_gan_weights.hdf5
│   ├── advance_X.txt.npy
│   ├── advance_Y.txt.npy
│   ├── traditional_X.txt.npy
│   ├── traditional_Y.txt.npy
│   ├── X.txt.npy
│   └── Y.txt.npy
│
└── testImages/
    └── Test images
🚀 10. Installation & Setup
Step 1 – Clone the Repository
git clone YOUR_GITHUB_REPOSITORY_URL

Navigate to the project:

cd AdvanceAugmentation
Step 2 – Install Python

The original project uses an older TensorFlow/Keras environment.

For reproducibility, use the dependency versions specified in:

requirements.txt
Step 3 – Install Dependencies
pip install -r requirements.txt
Step 4 – Start Jupyter Notebook
jupyter notebook

Jupyter Notebook will open in your browser.

▶️ 11. How to Run
Step 1

Open:

AdvanceAugmentation.ipynb
Step 2

Make sure the following folders are present in the project directory:

Dataset/
Gan/
model/
TraditionalAugmentation/
AdvanceAugmentData/
testImages/
Step 3

Run the notebook cells sequentially from the beginning.

Step 4

The notebook loads the available preprocessed datasets and trained model weights when they are present.

Step 5

The project performs the three classification experiments:

Without Augmentation
        ↓
Traditional Augmentation
        ↓
Advance GAN Augmentation
Step 6

The classification performance can be evaluated using:

Accuracy
Precision
Recall
F1-Score
Confusion Matrix
📓 12. Notebook & Output

The project contains two versions of the implementation:

Jupyter Notebook
AdvanceAugmentation.ipynb

Contains the complete Python implementation and project workflow.

HTML Version
AdvanceAugmentation.html

Contains the saved notebook execution and recorded outputs.

The HTML version is useful for reviewing the original project results without rerunning the complete notebook.

👩‍💻 13. Author

Sharon Shamsthuthi

B.Tech – Computer Science and Engineering
CMR Engineering College, Hyderabad, Telangana

🔗 Project Links

🎥 Project Demo:
https://youtu.be/ykvGh5tc2_Y

🌾 Dataset:
https://www.kaggle.com/datasets/vbookshelf/rice-leaf-diseases
