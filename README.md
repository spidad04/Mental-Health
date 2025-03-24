# 😷 Key Identifiers of Depression Using Machine Learning

This repository contains an R-based analysis to identify key predictors of depression among university students using machine learning techniques. The project leverages various R packages to preprocess data, select important features, build multiple predictive models, and explain model predictions with explainable AI techniques.

---

## 🔍 Overview

Depression is a complex condition influenced by several psychological and behavioral factors. In this project, we:

- **Clean & Preprocess Data:**  
  Read a raw CSV dataset, rename variables, and convert character columns to factors.
  
- **Visualize Data:**  
  Plot the distribution of depression labels.
  
- **Feature Selection:**  
  Use the Boruta algorithm to identify the top 10 predictors for depression.
  
- **Data Splitting:**  
  Create training, testing, and validation sets with stratification.
  
- **Model Training:**  
  Build and tune multiple classification models including:  
  - Random Forest  
  - Neural Network (Multi-Layer Perceptron)  
  - k-Nearest Neighbors (kNN)  
  - XGBoost
  
- **Model Evaluation:**  
  Use metrics such as Precision-Recall AUC, accuracy, and F1 score.
  
- **Explainable AI:**  
  Employ techniques like Accumulated Local Effects (ALE) and interaction strength analysis with the `iml` package to interpret predictions.

---

## 🗂️ Repository Structure

. ├── data/ │   └── Raw Data.csv         # The raw dataset containing survey responses ├── scripts/ │   └── analysis.Rmd         # R Markdown document with complete code and analysis ├── README.md                # This file └── references/             # (Optional) Additional documentation and references

---

## 🚀 Installation & Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/spidad04/Mental-Health.git
   cd Mental-Health

2. Install R and RStudio:

Ensure you have R and RStudio installed.


3. Install Required Packages:

Open R or RStudio and install the necessary packages:

install.packages(c(
  "tidyverse", "rsample", "tune", "yardstick", "dials", "recipes",
  "workflows", "parsnip", "themis", "Boruta", "vip", "iml"
))


4. Data Setup:

Place your CSV file (e.g., Raw Data.csv) in the data/ folder. Adjust the file path in analysis.Rmd if needed.




---

📊 Usage

Run the Analysis:

Open the analysis.Rmd file in RStudio. The document contains code blocks that:

Load and clean the data.

Visualize the distribution of depression labels.

Perform feature selection using Boruta.

Split the data into training, testing, and cross-validation sets.

Build and tune machine learning models (Random Forest, Neural Network, kNN, and XGBoost).

Evaluate models using pr-AUC, accuracy, and F1 score.

Generate explainability plots (ALE and interaction effects) to interpret model predictions.


Customize & Extend:

Feel free to modify the code to experiment with different modeling approaches or add additional data visualizations.



---

👥 Contributing

Contributions are welcome! If you'd like to improve this project, please open an issue or submit a pull request. For major changes, discuss them first by opening an issue.


---

📝 Authors

Edwin Kumadoh

Gabriel Agbobli




For any inquiries, please contact the authors or open an issue in this repository.


---

Happy Coding! 🚀
