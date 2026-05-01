# AI Job Market Salary Prediction

This repository contains the code for a supervised machine learning assignment using the AI and Data Science Job Market Dataset from Kaggle.

The main objective is to predict salary based on job, company, location, skill, education, and experience related features. The project is organized around seven research questions, each implemented in a separate Jupyter notebook.

## Dataset

Dataset source: Kaggle AI and Data Science Job Market Dataset 2020 to 2026 (https://www.kaggle.com/datasets/shree0910/ai-and-data-science-job-market-dataset-20202026?utm_source=chatgpt.com)

The dataset is not included in this repository. It should be downloaded from Kaggle and placed in the working environment before running the notebooks.

## Research Questions

1. Baseline model performance
2. Comparative model performance
3. Effect of preprocessing
4. Feature importance and interpretability
5. Sensitivity to evaluation metrics
6. Robustness and generalization
7. Practical usefulness and final recommendation

## Repository Structure

notebooks/ contains one notebook for each research question.

outputs/tables/ stores generated CSV result tables.

outputs/figures/ stores generated PDF figures.

## How to Run

Open each notebook in Kaggle or Jupyter Notebook and run all cells. Each notebook automatically saves its result table as a CSV file and its figure as a PDF file.

## Target Variable

The target variable is salary. Therefore, the task is treated as a supervised regression problem.

## Evaluation Metrics

The models are evaluated using MAE, RMSE, and R².
