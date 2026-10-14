# Ensemble Model Comparison: Decision Tree vs Random Forest vs Gradient Boosting

This beginner-friendly machine-learning project compares three classification models on the built-in Breast Cancer Wisconsin dataset from scikit-learn. The dataset is loaded directly from scikit-learn, so you do not need to download a separate CSV file.

## Models
1. Decision Tree Classifier (baseline)
2. Random Forest Classifier
3. Gradient Boosting Classifier

## Metrics
Accuracy, precision, recall, F1-score, and confusion matrix.

## Requirements
- Python 3.10 or newer recommended
- Jupyter Notebook or VS Code with the Jupyter extension

## Setup (Windows)
Open the extracted project folder in VS Code and open Terminal > New Terminal.

```powershell
py -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If PowerShell blocks activation, use Command Prompt and run:
```bat
.venv\Scripts\activate.bat
```

## Run the notebook
1. Open `notebooks/ensemble_exploration.ipynb` in VS Code.
2. Select the Python kernel for your `.venv` environment.
3. Run all cells from top to bottom.
4. The notebook prints metrics, displays a comparison chart and confusion matrices, and saves the comparison report to `reports/performance_comparison.md`.

## Dataset information
The notebook uses scikit-learn's Breast Cancer Wisconsin (Diagnostic) dataset, a standard tabular binary-classification dataset. It is loaded using `sklearn.datasets.load_breast_cancer(as_frame=True)`. Target 0 means malignant and target 1 means benign in this dataset. This is for learning model-comparison methods only, not for medical diagnosis.

## Files
- `notebooks/ensemble_exploration.ipynb`: preprocessing, training, evaluation, and visualizations
- `reports/performance_comparison.md`: report template/results (run the notebook to refresh results)
- `requirements.txt`: Python dependencies
- `data/raw_dataset_info.txt`: dataset source and schema notes

## Reproducibility
The notebook uses a fixed random seed. Model metrics may vary slightly with different library versions.

## GitHub
Do not upload `.venv/` or cache files. Upload the project files and the generated report after running the notebook.
