# NYC Job Salary Range Prediction

Machine learning project that predicts the minimum and maximum annual salary of NYC government job postings.

## Model workflow

- Data cleaning and EDA
- Salary annualization
- Sentence Transformer embeddings (`all-MiniLM-L6-v2`)
- CatBoost target encoding for categorical variables
- Two LightGBM regression models
- RMSE and R² evaluation
- Streamlit deployment

## Running locally

1. Run the Colab notebook and save the model artifacts.
2. Copy the generated `artifacts` folder into this project folder.
3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Start Streamlit:

```bash
streamlit run app.py
```

The app will open in your browser.

## Google Colab

The notebook is written for Google Colab. It mounts Google Drive, loads the dataset from Drive, trains the models, and saves the artifacts.

## Deployment

For Streamlit Community Cloud, upload `app.py`, `requirements.txt`, and the `artifacts` folder to a GitHub repository. Set the main file to `app.py`.

The Sentence Transformer model is loaded by name when the app starts, so the local Hugging Face model files do not need to be committed to GitHub.
