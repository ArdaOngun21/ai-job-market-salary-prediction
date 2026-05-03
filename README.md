\# AI Job Market Salary Prediction



This repository contains the code for a supervised machine learning assignment using the AI and Data Science Job Market Dataset from Kaggle.



The main objective of this project is to predict salary based on job, company, location, skill, education, experience, and work arrangement related features. The project is organized around seven research questions, with each research question implemented in a separate Jupyter notebook.



\## Dataset



Dataset source:



https://www.kaggle.com/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026



The dataset is not included in this repository. It should be attached to the Kaggle notebook environment before running the notebooks.



Expected Kaggle dataset directory:



```text

/kaggle/input/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026

```



The notebooks automatically search this directory for the dataset file.



\## Target Variable



The target variable is:



```text

salary

```



Since salary is a numerical variable, the task is treated as a supervised regression problem.



\## Research Questions



1\. How effectively can baseline supervised learning models predict salary in the AI Job Market Dataset?

2\. Which supervised learning model achieves the best salary prediction performance?

3\. How do preprocessing strategies affect salary prediction performance?

4\. Which features contribute most to salary prediction?

5\. How does model ranking change when different evaluation metrics are used?

6\. How robust is the selected salary prediction model under different validation and perturbation conditions?

7\. Which model provides the best balance between predictive performance, interpretability, robustness, computational cost, and deployment suitability?



\## Repository Structure



```text

notebooks/

&#x20; RQ1\_Baseline\_Performance.ipynb

&#x20; RQ2\_Model\_Comparison.ipynb

&#x20; RQ3\_Preprocessing\_Impact.ipynb

&#x20; RQ4\_Feature\_Importance.ipynb

&#x20; RQ5\_Metric\_Sensitivity.ipynb

&#x20; RQ6\_Robustness\_Generalization.ipynb

&#x20; RQ7\_Final\_Recommendation.ipynb



outputs/

&#x20; tables/

&#x20;   RQ1\_Baseline\_Model\_Performance.csv

&#x20;   RQ2\_Model\_Comparison.csv

&#x20;   RQ3\_Preprocessing\_Impact.csv

&#x20;   RQ4\_Feature\_Importance.csv

&#x20;   RQ5\_Metric\_Sensitivity.csv

&#x20;   RQ6\_Robustness\_Generalization.csv

&#x20;   RQ7\_Final\_Recommendation.csv



&#x20; figures/

&#x20;   RQ1\_Baseline\_Model\_Performance.pdf

&#x20;   RQ2\_Model\_Comparison.pdf

&#x20;   RQ3\_Preprocessing\_Impact.pdf

&#x20;   RQ4\_Feature\_Importance.pdf

&#x20;   RQ5\_Metric\_Sensitivity.pdf

&#x20;   RQ6\_Robustness\_Generalization.pdf

&#x20;   RQ7\_Final\_Recommendation.pdf

```



\## Methodology



The dataset is loaded from the Kaggle input directory. The salary column is used as the target variable, while job, company, location, education, experience, skill, remote work, and posting related columns are used as predictors.



The preprocessing pipeline handles numerical and categorical variables separately. Numerical variables are imputed and scaled where required. Categorical variables are imputed and transformed using one hot encoding. The dataset is split into training and testing subsets, and supervised regression models are trained and evaluated.



\## Models Used



The project uses the following supervised regression models:



```text

Linear Regression

Ridge Regression

Decision Tree Regressor

k-NN Regressor

Random Forest Regressor

Gradient Boosting Regressor

Extra Trees Regressor

```



Different models are used depending on the purpose of each research question.



\## Evaluation Metrics



The models are evaluated using the following regression metrics:



```text

MAE

RMSE

R²

```



MAE and RMSE measure prediction error. Lower values indicate better performance.



R² measures the proportion of salary variation explained by the model. Higher values indicate better performance.



\## Outputs



Each notebook saves one result table and one publication ready figure.



Generated tables are saved as CSV files under:



```text

/kaggle/working/ai\_job\_market\_outputs/tables/

```



Generated figures are saved as PDF files under:



```text

/kaggle/working/ai\_job\_market\_outputs/figures/

```



The final generated outputs are also included in this repository under:



```text

outputs/tables/

outputs/figures/

```



\## How to Run on Kaggle



1\. Open the required notebook in Kaggle.

2\. Attach the dataset from Kaggle:



```text

https://www.kaggle.com/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026

```



3\. Make sure the dataset is available under the expected Kaggle input directory:



```text

/kaggle/input/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026

```



4\. Run the notebook cells from top to bottom.

5\. The notebook will generate and save the corresponding CSV table and PDF figure.



\## Notes



The dataset appears to contain strong structured relationships between salary and predictors such as experience level, job title, company size, and technical skills, some models may achieve very high R² scores. These results should be interpreted carefully when discussing real world generalization.



\## Author



Arda Ongun

