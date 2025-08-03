# CODECRAFT_ML_03
# 🐱🐶 Cat vs Dog Image Classifier (SVM)

This project implements an image classification pipeline using **Support Vector Machines (SVM)** to distinguish between **cats and dogs** based on grayscale image features.

## 📁 Dataset

The dataset consists of two folders:
- `cat/` - images of cats
- `dog/` - images of dogs

The dataset should be structured like this after unzipping:

dataset/
└── archieve/
└── animals/
├── cat/
└── dog/

yaml
Copy
Edit

✅ Each folder should contain `.png` image files.

> **Note:** Only a small number of images are used for demonstration (~25 per class), but this can be extended easily.

---

## 🛠️ How to Run

1. Open the provided Colab notebook (`Cat_Dog_SVM.ipynb`)
2. Upload your `archive.zip` (contains `animals/` folder) to the Colab session
3. Unzip using:

```python
!unzip -q archive.zip -d dataset
Update the image paths in code:

python
Copy
Edit
cat_dir = 'dataset/archieve/animals/cat'
dog_dir = 'dataset/archieve/animals/dog'
Run all cells to:

Load and preprocess images

Train an SVM classifier

Evaluate performance

Predict a new image

🧠 Model Used
SVM (Support Vector Machine) classifier from sklearn.svm

Images converted to grayscale and resized to 64x64

Optionally, you can add HOG features for better accuracy

🧪 Sample Output
yaml
Copy
Edit
Classification Report:
              precision    recall  f1-score   support
         Cat       0.72      0.80      0.76       25
         Dog       0.78      0.68      0.72       25
    Accuracy: 0.74
📌 Requirements
Python 3.7+

OpenCV

NumPy

scikit-learn

tqdm
