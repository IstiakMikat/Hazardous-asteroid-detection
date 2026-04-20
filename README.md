# 🚀 Potentially Hazardous Asteroid Detection

## 📌 Overview

This project uses supervised machine learning to classify asteroids as **hazardous** or **non-hazardous** based on NASA Near-Earth Object (NEO) data. It analyzes asteroid characteristics such as size, velocity, orbit, and distance to build accurate prediction models.

---

## 🎯 Objective

To develop a reliable classification system that can help in the **early detection of potentially dangerous asteroids**, supporting planetary defense research.

---

## 📂 Dataset

* Source: NASA NEO dataset (via Kaggle)
* Samples: 4687
* Features: 40 (reduced to 15 after preprocessing)
* Target: `Hazardous` (0 = No, 1 = Yes)

---

## ⚙️ Workflow

1. Data Cleaning
2. Feature Engineering
3. Correlation-based Feature Selection
4. Outlier Handling
5. Feature Scaling (Robust Scaler)
6. Model Training
7. Model Evaluation

---

## 🤖 Models Used

* 🌳 Random Forest Classifier
* 📍 K-Nearest Neighbors (KNN)
* 📈 Support Vector Machine (SVM)

---

## 📊 Results

| Model             | Accuracy   | Precision | Recall | F1 Score |
| ----------------- | ---------- | --------- | ------ | -------- |
| **Random Forest** | **99.72%** | 99.14%    | 99.14% | 0.9914   |
| KNN               | 94.67%     | 93.86%    | 92.24% | 0.826    |
| SVM               | 97.73%     | 89.45%    | 76.72% | 0.9304   |

🏆 **Best Model: Random Forest Classifier**

---

## 📁 Project Structure

```
hazardous-asteroid-detection/
│
├── README.md
├── requirements.txt
│
├── data/
│   └── nasa.csv
│
├── notebooks/
│   └── hazardous_asteroid_detection.ipynb
│
├── reports/
│   └── hazardous_asteroid_detection_report.pdf
│
└── images/
```

---

## ▶️ How to Run

### 1. Clone Repository

```bash
git clone https://github.com/your-username/hazardous-asteroid-detection.git
cd hazardous-asteroid-detection
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run Notebook

```bash
jupyter notebook
```

Open:

```
notebooks/hazardous_asteroid_detection.ipynb
```

---

## 📸 Visualizations

* Correlation Heatmap
* Boxplots (Outlier Detection)
* Pairplots
* Confusion Matrices

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Jupyter Notebook

---

## 💡 Key Highlights

* End-to-end ML pipeline implementation
* Feature selection improved model performance
* Random Forest achieved highest accuracy
* Real-world application in space safety

---

## 👩‍💻 Author

**MD Istiak Haque**

BSc in Computer Science

BRAC University

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
