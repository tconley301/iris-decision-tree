# Iris Decision Tree (CS471 Assignment 4)

Train and evaluate a Decision Tree classifier on the classic **Iris** dataset.  
This repository includes a runnable Python script that mirrors a Google Colab workflow (EDA, train/val/test split, simple hyperparameter sweep, final model, metrics, and tree visualization).

## Project Structure
```
.
├─ src/
│  └─ train_decision_tree_iris.py
├─ plots/                 # generated: accuracy curve, tree visualization
├─ reports/               # generated: classification report (txt)
├─ notebooks/             # optional: place your .ipynb here (see below)
├─ requirements.txt
├─ .gitignore
└─ README.md
```

## Quickstart (Local)

### 1) Create and activate a virtual environment
```bash
# Windows (PowerShell)
python -m venv .venv
.\.venv\Scripts\Activate.ps1

# macOS / Linux
python3 -m venv .venv
source .venv/bin/activate
```

### 2) Install dependencies
```bash
pip install -r requirements.txt
```

### 3) Run the script
```bash
python src/iris-DT-clf.py
```

Outputs:
- **plots/accuracy_vs_max_depth.png**
- **plots/decision_tree.png**
- **reports/classification_report.txt**
- Console logs with shapes and scores

## Notes
- The script mirrors the choices in your notebook: `criterion='entropy'`, `max_depth` sweep 1..10, and a final model with `max_depth=3` (you can tweak this).
- Random seeds are fixed for reproducibility (`random_state=42`).

## License
See [LICENSE](LICENSE).
