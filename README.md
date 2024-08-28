Galaxy Distance Estimation Project

Project Overview

This project is focused on estimating galaxy distances using photometric redshift techniques. The project employs advanced machine learning models such as Random Forest, Gradient Boosting, Decision Trees, and XGBoost to predict spectroscopic redshift from photometric data. The work is primarily based on two meticulously constructed galaxy catalogs, Teddy and Happy, which simulate the biases and challenges typically encountered in large-scale astronomical surveys.

Objectives
	•	Model Performance Assessment: Evaluate the accuracy, robustness, and generalization capabilities of non-parametric regression models in estimating galaxy distances under varying data conditions.
	•	Model Comparison: Identify the best performing models among Decision Tree, Random Forest, Gradient Boosting, and XGBoost for photometric redshift estimation.
	•	Photometric Error Analysis: Assess the impact of photometric errors on model accuracy and reliability.
	•	Dataset Utilization: Utilize the Teddy and Happy catalogs to simulate real-world challenges in photometric redshift estimation.

Dataset Description

Happy Catalogue

The Happy catalogue consists of four distinct samples, each with known spectroscopic redshifts (spec-z):
	•	Happy A: Aligned with the SDSS DR12 spectroscopic sample, used for training and calibration.
	•	Happy B: Similar to Happy A, used for validation.
	•	Happy C: Reflects photometric sample characteristics with higher error distributions.
	•	Happy D: Represents the SDSS DR12 photometric sample for further validation.

Teddy Catalogue

The Teddy catalogue also comprises four samples, each with known spectroscopic redshifts (spec-z):	
        •       Teddy A: Used for training and calibration.
	•	Teddy B: Identical to Teddy A, used for validation.
	•	Teddy C: Similar coverage to A and B but follows a different underlying distribution.
	•	Teddy D: Extends beyond the coverage of Teddy A and B, simulating real-world conditions.


Model Description

Decision Trees (DT)

A foundational model offering a simple yet effective approach for regression tasks, used as a baseline for further model comparisons.

Random Forest (RF)

An ensemble learning method that constructs multiple decision trees to enhance prediction accuracy and reduce overfitting.

Gradient Boosting Machines (GBM)

A sequential ensemble method that builds models iteratively to correct errors made by previous models, improving accuracy over multiple iterations.

XGBoost

An advanced implementation of Gradient Boosting that includes regularization, parallel processing, and efficient handling of sparse data, making it the most robust model used in this project.

Hyperparameter Tuning

Hyperparameter tuning was performed using GridSearchCV to identify the optimal parameters for each model, ensuring the best performance.

Results

The models were evaluated based on several metrics:
	•	Mean Prediction
	•	Standard Deviation (Std)
	•	Median Absolute Deviation (MAD)
	•	Outlier Rate


Both weighted and unweighted approaches were explored to address data imbalances in the datasets.
stallation and Usage

Prerequisites
        •	Python 3.7+
	•	Required Python libraries: numpy, pandas, scikit-learn, xgboost, matplotlib

 Results Visualization
        •	The results are visualized using plots that compare the performance of different models across various subsets of the Happy and Teddy datasets.

	

Acknowledgments	
        •	This project is a part of the MSc Data Science program at the University of Hertfordshire.
	•	Special thanks to Rafael Dsouza for supervising this project.


