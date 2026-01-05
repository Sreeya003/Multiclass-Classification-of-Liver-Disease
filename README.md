🧪 **_Multiclass Classification of Liver Disease_**

🩺 **Project Overview**
This repository contains a clinical analytics pipeline built in R to classify patients into one of four diagnostic categories based on biochemical and demographic markers. The project focuses on transforming raw clinical data into a high-precision diagnostic tool by combining traditional statistical modeling with advanced dimensionality reduction.

The final pipeline utilizes Linear Discriminant Analysis (LDA) on PCA-transformed features to achieve high classification accuracy across diverse liver disease stages.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🚀 **Key Features & Methodology**

1. 🧹 Clinical Data Engineering
   
   Preprocessing: Cleaned and encoded mixed-type demographic and biochemical data.

   Outlier Management: Implemented 99th percentile capping to handle extreme clinical values without losing data integrity.

   Feature Scaling: Applied Z-score normalization to standardize features for distance-based and variance-based algorithms.

2. 📉 Feature Selection & Noise Reduction

   Multicollinearity Control: Applied Principal Component Analysis (PCA) to handle highly correlated biochemical markers.

   Biomarker Identification: Used ANOVA and effect-size analysis to validate high-signal biomarkers, identifying AST, BIL, and GGT as the most significant drivers of patient segmentation.

3. 🤖 Multiclass Modeling & Performance

   Models Evaluated: Compared Multinomial Logistic Regression (MLR), Linear Discriminant Analysis (LDA), and Quadratic Discriminant Analysis (QDA).

   Champion Model: The LDA model (using PCA features) outperformed others with:

✅ Accuracy: 94.91%

🎯 Macro F1-Score: 0.79

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🛠️ Technical Stack
Language: R

Libraries: tidyverse, caret, MASS (LDA/QDA), FactoMineR (PCA)

Techniques: PCA, ANOVA, Outlier Capping, Z-score Scaling, Multiclass Classification

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📂 Repository Structure
scripts/: R scripts for preprocessing, PCA, and model training.

analysis/: ANOVA results and biomarker effect-size reports.

results/: Confusion matrices and accuracy benchmarks.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🏁 How to Use
📥 Load your liver disease dataset into the R environment.

⚙️ Run the preprocessing script to handle outliers and scaling.

📉 Execute the PCA script to generate principal components.

🏆 Run the modeling script to train the LDA classifier and view performance metrics.
