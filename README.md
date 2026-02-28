## Predictive Intelligence for Resource Risk Management: Rainfall Forecasting Pipeline 🌧️

<img width="1722" height="826" alt="Print Screen" src="https://github.com/user-attachments/assets/e2aa0b5c-e163-438b-a6f0-4a2471d1ec4d" />
________________________________________

## 🔍 Project Overview:
This project implements an end-to-end Data Science Engineering lifecycle to predict next-day rainfall (target variable: Rain_Tomorrow), leveraging 8.5 years of historical meteorological data from Australia. The analysis is based on a real-world dataset sourced from Kaggle. The core objective was to engineer a robust classification pipeline, spanning from data profiling to advanced modeling. A primary focus was placed on optimizing recall - a critical metric in scenarios where minimizing false negatives is vital to mitigate risks in sectors such as agriculture, public safety, and event management.
________________________________________

## 💡Project Highlights:
- KNN Model (k=23, Euclidean Distance): Achieved peak performance with a 0.82 recall score, while maintaining high accuracy and AUC. This configuration effectively mitigates operational risk by maximizing rainfall detection.
- Multi-Layer Perceptron, MLP (Hyperparameters: Inverse Scaling, Learning Rate = 0.05, 500 Iterations): Reached a 0.76 recall score, with high accuracy and AUC, demonstrating a strong generalization and zero evidence of overfitting.
- Most relevant feature: Humidity_3pm, showing a strong correlation with the target variable RainTomorrow.
- Conclusion: KNN and MLP models proved to be the most effective for this use case, maximizing the detection of rainy days. This approach is ideal for sectors such as agriculture or event management, where the cost of a false negative (failing to predict rain when it occurs) significantly outweighs a false positive.
________________________________________

## ⚙️ Project Structure:
1.	Data Profiling: Exploratory data analysis, missing values, outliers, and correlation analysis.
2.	Data Preprocessing: Missing value imputation, outliers management, feature scaling, and class balancing.
3.	Feature Engineering: Implementation of advanced feature encoding and transformation techniques.
4.	Model Benchmarking: Training and validation of 6 classification models.
5.	Performance Evaluation: Evaluation metrics (Accuracy, Recall, Precision, AUC, and F1-Score), confusion matrix, and overfitting study.
6.	Critical Analysis: Evaluation of results against operational risk objectives.
________________________________________

## 🛠️ Tech Stack:
- Language: Python
- Environment: Jupyter Notebook, Visual Studio Code
- Libraries: Pandas, NumPy, Scikit-learn, SciPy, Matplotlib, Seaborn
________________________________________

## 📂 Repository Structure:
- `Engenharia_Ciencia_Dados_Previsao_Chuva.ipynb`: Full source code and implementation.
- `Engenharia_Ciencia_Dados_Previsao_Chuva.pdf`: Detailed technical PDF report.
________________________________________

## 📦 Quick Start:
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Open the `.ipynb` file in Jupyter Notebook.
4. Execute cells sequentially to reproduce the analysis and visualizations.
________________________________________

## 📩 Contacts:
- Alexandre Vasconcelos
- Email: alex.vasconcelos.2057@gmail.com
- LinkedIn: [linkedin.com/in/alexandre-vasconcelos-396227167/](https://www.linkedin.com/in/alexandre-vasconcelos-396227167/)
