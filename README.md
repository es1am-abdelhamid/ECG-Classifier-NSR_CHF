# 🫀 ECG Signal Classification (NSR vs CHF)
**Author:** Eslam Abdelhamid OR Eslam A.Abd El-Razek  
**Author Contact:** eslamelshick@gmail.com 

[![Python](https://img.shields.io/badge/Python-3.13%2B-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange.svg)](https://www.tensorflow.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-green.svg)](https://scikit-learn.org/)

## 📊 Project Overview
This project focuses on the automated classification of ECG signals into two categories: **Normal Sinus Rhythm (NSR)** and **Congestive Heart Failure (CHF)**. [cite_start]By leveraging extracted physiological features, we implemented a full data science pipeline—from preprocessing to deep learning—to identify the most accurate diagnostic model[cite: 3, 14].

## 🧠 Models & Architecture
[cite_start]We implemented and compared three different models to evaluate their effectiveness in biomedical signal classification[cite: 14]:

1. **Support Vector Machine (SVM):** Utilized an **RBF kernel** to handle non-linear relationships in the feature space.
2. **Decision Tree:** A baseline interpretable model with `max_depth=5` to prevent overfitting.
3. [cite_start]**Artificial Neural Network (ANN):** A multi-layer feedforward architecture designed for binary classification[cite: 19, 28].
   * **Input Layer:** Matches the number of extracted features.
   * **Hidden Layers:** Dense(16, ReLu) → Dropout(0.2) → Dense(8, ReLu).
   * **Output Layer:** Dense(1, Sigmoid).

## 📊 Visualizations & Project Assets
The project includes several key visual insights and files as shown in the project directory:

* **`accs_bar_graph.png`**: A bar chart comparing the accuracy scores of SVM, Decision Tree, and ANN.
* **`confusion_matrices_for_our_models.png`**: Visual representation of the performance for each classifier, showing true vs. predicted labels.
* **`Distribution_of_Target_Classes.png`**: A count plot showing the balance between NSR and CHF cases in the dataset.
* **`features_heatmap.png`**: A correlation matrix used to identify relationships between numerical features and assist in feature selection.
* **`KDE_plots_for_our_selected_features.png`**: Density plots illustrating the distribution and overlap of key features for both classes.
* **`ECG_Data.xlsx`**: The primary dataset containing the extracted ECG signal features used for training.

## 📈 Performance Results
[cite_start]The models were evaluated using Accuracy and other key metrics[cite: 14]. The **ANN** outperformed traditional machine learning models:

| Rank | Model | Accuracy |
| :--- | :--- | :--- |
| **1** | **Artificial Neural Network (ANN)** | **96.39%** |
| 2 | SVM (RBF Kernel) | 94.17% |
| 3 | Decision Tree | 93.33% |

🏆 **Best Model:** The ANN achieved the highest accuracy due to its superior ability to learn complex, non-linear patterns within the ECG features.

## 🧪 Workflow & Methodology
1. **Data Collection:** Loading the `ECG_Data.xlsx` into a pandas DataFrame.
2. [cite_start]**Preprocessing:** Handling missing values via mean imputation and scaling features using `StandardScaler`[cite: 14].
3. **Exploratory Data Analysis (EDA):** Visualizing distributions using KDE plots and analyzing dependencies via Heatmaps.
4. **Feature Selection:** Reducing multicollinearity to improve model stability.
5. [cite_start]**Modeling & Evaluation:** Comparing performance metrics across the three models[cite: 14, 16].

## ⚙️ Tech Stack
* **Language:** Python 3[cite: 21].
* [cite_start]**Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `tensorflow/keras`[cite: 22, 24, 26, 28].

## 👨‍💻 Author
**Author:** Eslam Abdelhamid OR Eslam A.Abd El-Razek  
**Author Contact:** eslamelshick@gmail.com 

*Mechatronics Engineering Student | AI , ML ,& DL Researcher*
