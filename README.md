# AI Job Market Salary Prediction

This repository contains the code for a supervised machine learning assignment using the AI and Data Science Job Market Dataset from Kaggle.

The main objective of this project is to predict salary based on job, company, location, skill, education, experience, and work arrangement related features. The project is organized around seven research questions, with each research question implemented in a separate Kaggle compatible Jupyter notebook.

## Dataset

**Dataset source:**  
https://www.kaggle.com/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026

The dataset is not included in this repository. It should be attached to the Kaggle notebook environment before running the notebooks.

**Expected Kaggle dataset directory:**  
`/kaggle/input/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026`

The notebooks automatically search this directory for the dataset file.

## Target Variable

**Target variable:** `salary`

Since salary is a numerical variable, the task is treated as a supervised regression problem.

## Research Questions

1. How effectively can baseline supervised learning models predict salary in the AI Job Market Dataset?
2. Which supervised learning model achieves the best salary prediction performance?
3. How do preprocessing strategies affect salary prediction performance?
4. Which features contribute most to salary prediction?
5. How does model ranking change when different evaluation metrics are used?
6. How robust is the selected salary prediction model under different validation and perturbation conditions?
7. Which model provides the best balance between predictive performance, interpretability, robustness, computational cost, and deployment suitability?

## Repository Structure

```text
notebooks/
  RQ1_Baseline_Performance.ipynb
  RQ2_Model_Comparison.ipynb
  RQ3_Preprocessing_Impact.ipynb
  RQ4_Feature_Importance.ipynb
  RQ5_Metric_Sensitivity.ipynb
  RQ6_Robustness_Generalization.ipynb
  RQ7_Final_Recommendation.ipynb

outputs/
  tables/
    RQ1_Baseline_Model_Performance.csv
    RQ2_Model_Comparison.csv
    RQ3_Preprocessing_Impact.csv
    RQ4_Feature_Importance.csv
    RQ5_Metric_Sensitivity.csv
    RQ6_Robustness_Generalization.csv
    RQ7_Final_Recommendation.csv

  figures/
    RQ1_Baseline_Model_Performance.pdf
    RQ2_Model_Comparison.pdf
    RQ3_Preprocessing_Impact.pdf
    RQ4_Feature_Importance.pdf
    RQ5_Metric_Sensitivity.pdf
    RQ6_Robustness_Generalization.pdf
    RQ7_Final_Recommendation.pdf
```

## Methodology

The dataset is loaded from the Kaggle input directory. The `salary` column is used as the target variable, while job, company, location, education, experience, skill, remote work, and posting related columns are used as predictors.

The preprocessing pipeline handles numerical and categorical variables separately. Numerical variables are imputed and scaled where required. Categorical variables are imputed and transformed using one hot encoding. The dataset is split into training and testing subsets, and supervised regression models are trained and evaluated.

## Models Used

The project uses the following supervised regression models:

- Linear Regression
- Ridge Regression
- Decision Tree Regressor
- k-NN Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Extra Trees Regressor

Different models are used depending on the purpose of each research question.

## Evaluation Metrics

The models are evaluated using the following regression metrics:

- MAE
- RMSE
- R²

MAE and RMSE measure prediction error. Lower values indicate better performance.

R² measures the proportion of salary variation explained by the model. Higher values indicate better performance.

## Outputs

Each notebook saves one result table and one publication ready figure.

Generated tables are saved as CSV files under:

`/kaggle/working/ai_job_market_outputs/tables/`

Generated figures are saved as PDF files under:

`/kaggle/working/ai_job_market_outputs/figures/`

The final generated outputs are also included in this repository under:

- `outputs/tables/`
- `outputs/figures/`

## How to Run on Kaggle

1. Open the required notebook in Kaggle.
2. Attach the dataset from Kaggle:  
   https://www.kaggle.com/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026
3. Make sure the dataset is available under the expected Kaggle input directory:  
   `/kaggle/input/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026`
4. Run the notebook cells from top to bottom.
5. The notebook will generate and save the corresponding CSV table and PDF figure.

## Notes

The initial dummy tables and figures were used only as templates. The final notebooks generate actual results from the dataset. Since the dataset appears to contain strong structured relationships between salary and predictors such as experience level, job title, company size, and technical skills, some models may achieve very high R² scores. These results should be interpreted carefully when discussing real world generalization.

## Author

Arda Ongun
