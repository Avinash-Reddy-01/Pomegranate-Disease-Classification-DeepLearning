# 🍎 Pomegranate Fruit Disease Classification using Transfer Learning

This project implements a deep learning approach for the classification of **pomegranate fruit diseases** using **transfer learning models**. The work is inspired by the published research article:

> *"Transfer learning models for classification of pomegranate fruit diseases using image dataset"*  
> [ScienceDirect Link](https://www.sciencedirect.com/science/article/pii/S2352340924002531)

Two core notebooks are included in this repository:
- `Image_Classification.ipynb` - Transfer learning model training and evaluation
- `K-Fold_Cross_Validation.ipynb` - Robust evaluation using K-Fold strategy

---

## 📂 Dataset

The dataset used in this project is publicly available via Data in Brief:

🔗 *[Pomegranate Fruit Diseases Dataset](https://doi.org/10.1016/j.dib.2024.110284)*

The dataset includes labeled images of:
- **Healthy** pomegranate
- **Anthracnose**
- **Bacterial Blight**
- **Cercospora Fruit Spot**
- **Alternaria Fruit Spot**

### 📊 Data Split
The dataset is split using `split-folders`:
- 60% Training
- 20% Validation
- 20% Testing

---

## 🧠 Transfer Learning Models Used

The following pretrained CNN architectures are utilized:
- `VGG19`
- `ResNet152V2`
- `InceptionV3`
- `EfficientNetV2L`
- `DenseNet169`
- `Xception`

These models are fine-tuned for multi-class classification with performance metrics including:
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- Classification Report

---

## 🧪 K-Fold Cross Validation

The second notebook uses **Stratified K-Fold Cross Validation** (k=5) to ensure robust generalization and avoid overfitting. Metrics are averaged across all folds for stable evaluation.

---

## 📸 Image Augmentation

To improve model robustness and reduce overfitting:
- Horizontal & vertical flip
- Rotation
- Brightness adjustments
- Zoom and shift transforms

Implemented using `ImageDataGenerator`.

---

## 🛠️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/Avinash-Reddy-01/Pomegranate-Disease-Classification-DeepLearning.git
cd pomegranate-disease-classification
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Add dataset to the root folder or modify paths in the notebooks.

4. Run notebooks in order:
   - `Image_Classification.ipynb`
   - `K-Fold_Cross_Validation.ipynb`

---

## 📦 Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn
- OpenCV
- Split-folders

---

## 📧 Contact

For questions or collaborations, reach out to:

**Avinash Reddy**  
📧 avinashreddykasireddy954@gmail.com

---

## 📝 License

This project is licensed under the MIT License.
