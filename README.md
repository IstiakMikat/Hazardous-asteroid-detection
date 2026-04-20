# Hazardous-asteroid-detection
Classifies asteroids as hazardous or non-hazardous using supervised ML on NASA NEO data. Uses features like size, velocity, orbit, and distance to build accurate models for early detection of potentially dangerous asteroids, supporting planetary defense research.

🎯 Problem Statement

Asteroids frequently pass near Earth, and some pose potential threats. Manual analysis of such large datasets is inefficient.
This project aims to:

Automate asteroid classification using ML
Compare multiple models
Identify the best-performing classifier
📂 Dataset
Source: NASA NEO dataset (via Kaggle)
Total Samples: 4687
Total Features: 40
Final Features after preprocessing: 15
Target Variable: Hazardous (Boolean → Converted to 0/1)
⚙️ Methodology
1. Data Preprocessing
Removed irrelevant features:
ID, Name, Date fields
Features with single unique values
Handled:
No missing values
No duplicate values
2. Feature Engineering
Applied correlation analysis
Removed highly correlated features (|r| ≥ 0.9)
Reduced dimensionality significantly
3. Feature Scaling
Used Robust Scaler (handles outliers effectively)
4. Outlier Handling
Identified using boxplots
Removed features with extreme outlier influence
🤖 Machine Learning Models Used
🌳 Random Forest
Ensemble learning method
Uses multiple decision trees
Robust to outliers and non-linear data
📍 K-Nearest Neighbors (KNN)
Distance-based classification
Simple and intuitive model
📈 Support Vector Machine (SVM)
Uses hyperplanes for classification
RBF kernel applied for non-linear separation
📊 Results Comparison
Model	Accuracy	Precision	Recall	F1 Score
Random Forest	99.72%	99.14%	99.14%	0.9914
KNN	94.67%	93.86%	92.24%	0.826
SVM	97.73%	89.45%	76.72%	0.9304
🏆 Best Model: Random Forest Classifier
Highest accuracy and F1 score
Lowest false positives & false negatives
📸 Visualizations

The project includes:

Correlation heatmap
Boxplots (outlier detection)
Pairplots (feature relationships)
Confusion matrices for all models
🗂️ Project Structure
hazardous-asteroid-detection/
│
├── README.md
├── requirements.txt
├── data/
│   └── nasa.csv
│
├── notebooks/
│   └── hazardous_asteroid_detection.ipynb
│
├── reports/
│   └── hazardous_asteroid_detection_report.pdf
│
├── images/
│   ├── correlation_heatmap.png
│   ├── boxplot.png
│   ├── pairplot.png
│   └── confusion_matrices.png
▶️ How to Run the Project
1. Clone the Repository
git clone https://github.com/your-username/hazardous-asteroid-detection.git
cd hazardous-asteroid-detection
2. Install Dependencies
pip install -r requirements.txt
3. Run Jupyter Notebook
jupyter notebook

Open:

notebooks/hazardous_asteroid_detection.ipynb
💡 Key Learnings
Feature selection significantly improves model performance
Random Forest handles real-world noisy data effectively
Proper preprocessing is as important as model selection
Visualization helps understand dataset behavior deeply
🌍 Real-World Impact
Helps automate asteroid risk classification
Supports space research & planetary defense
Demonstrates real-world ML pipeline:
Data cleaning
Feature engineering
Model training
Evaluation
🛠️ Tech Stack
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
Jupyter Notebook
👩‍💻 Author

MD Istiak Haque
BSc in Computer Science
BRAC University
