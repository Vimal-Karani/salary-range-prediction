# NYC Job Salary Range Prediction

A machine learning regression project that predicts the **minimum and maximum annual salary** for New York City government job postings.

## Project Overview

The project uses job-posting information such as agency, job title, employment details, career level, and location to estimate salary ranges.

The workflow includes:

- Data cleaning and exploratory analysis
- Salary annualization
- Text feature extraction
- Sentence Transformer embeddings using `all-MiniLM-L6-v2`
- Categorical feature encoding
- LightGBM regression
- Separate models for minimum and maximum salary
- RMSE and R² evaluation

## Models

Two LightGBM regression models are trained:

- Minimum salary prediction
- Maximum salary prediction

The project focuses on building a practical salary-estimation model from publicly available job-posting information.

## Files

- `NYC_Job_Salary_Range_Prediction_Polished.ipynb` — Google Colab notebook
- `README.md` — project documentation
- `requirements.txt` — Python dependencies

## Running the Notebook

The notebook is designed for **Google Colab**.

1. Open the notebook in Google Colab.
2. Mount Google Drive when prompted.
3. Update the dataset path if necessary.
4. Run the notebook from top to bottom.
5. Review the model evaluation and prediction results.

## Key Learning Outcomes

This project demonstrates:

- Regression modelling
- Salary data preprocessing
- Text embeddings
- Categorical feature handling
- LightGBM
- Model evaluation using RMSE and R²
- Feature engineering for real-world tabular data

## Note

Salary predictions are estimates based on the information available in the dataset. Actual compensation can vary depending on experience, qualifications, responsibilities, and other factors.
