# DSCI 552 Homework 6

Hongwei Xiao (Ga9a)

Open `notebooks/Xiao_Hongwei_HW6.ipynb` for the code, saved outputs, figures, and answers to Questions 1–5. `Xiao_Hongwei_HW6.pdf` is the reading copy.

## Run

Use Python 3.12. Install the packages in `requirements.txt`, then select that environment as the notebook kernel and run all cells in order. Keep the directory structure unchanged. The notebook finds `data/` when started from either this folder or `notebooks/`.

```sh
python -m pip install -r requirements.txt
```

The full 60,000-row training set is used. Five-fold cross-validation selects the L1 penalty separately for ordinary XGBoost and XGBoost with SMOTE. The random seed is 42. SMOTE is applied only to the training portion of each fold. Expect several minutes or longer to rerun, depending on the computer.

## Files

- `data/`: the original APS training/test CSV files and dataset description.
- `notebooks/`: the executed notebook.
- `results/`: metrics, cross-validation results, feature statistics, figures, and predicted probabilities.
- `requirements.txt`: package versions used for this run.
- `Xiao_Hongwei_HW6.pdf`: printable notebook with code and outputs.

The scatter matrix uses a fixed 3,000-row sample for readability; all fitted models use the full training set and all 170 features. The four textbook exercises follow the assignment's numbering; Chapter 6 exercises 3 and 5 appear under section 6.8 in the seventh printing of the first-edition ISLR book.
