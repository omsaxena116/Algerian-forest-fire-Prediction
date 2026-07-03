# lab-flask (local setup)

This mirrors the folder structure used in the instructor's browser-based
VS Code lab, adapted to run on your own machine.

## 1. Create a virtual environment

```bash
python -m venv venv
```

Activate it:

- **Windows:** `venv\Scripts\activate`
- **Mac/Linux:** `source venv/bin/activate`

## 2. Install dependencies

```bash
pip install -r requirements.txt
```

## 3. Run the Flask app

```bash
python app.py
```

Then open your browser and go to:

```
http://127.0.0.1:5000/
```

(Locally you don't need the `https://{your_url}.pwskills.app:5000/` tunnel URL —
that was only needed because the instructor's lab ran on a remote container.)

## Folder guide

- `app.py` — Flask entry point.
- `notebooks/` — Jupyter notebooks for EDA, feature engineering, and model
  training. Put the dataset CSV (e.g. `Algerian_forest_fires_cleaned_dataset.csv`)
  in this folder to match the notebook's relative path.
- `models/` — Save trained model/scaler `.pkl` files here.
- `templates/` — HTML templates for Flask (`render_template`) once you build
  out the prediction form.
- `static/` — CSS/JS/images for the Flask app.
- `.vscode/` — Recommended extensions and settings for this workspace.
