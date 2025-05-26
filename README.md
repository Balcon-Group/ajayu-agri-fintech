# Ajayu Agri-Fintech AI Platform

This repository contains the full Python implementation of **Ajayu**, an AI-powered agri-fintech platform designed to support predictive modeling, financial eligibility scoring, and data-driven policy design. It integrates structured agricultural data, export traceability, and geospatial risk analytics for Peru's non-traditional horticultural value chains.

---

## 📁 Repository Structure

```
data/
├── cenagro_2012/
│   └── [region]/
│       ├── REC01/
│       ├── ...
notebooks/
├── ingestion/
├── transformation/
├── modeling/
scripts/
├── append_pipeline.py
├── feature_engineering.py
requirements.txt
README.md
.gitignore
```

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Or use VSCode with the Jupyter extension.

---

## 📌 Key Notebooks

| Notebook                                  | Purpose                                                  |
|-------------------------------------------|-----------------------------------------------------------|
| `CENAGRO_2012_Ingestion_Pipeline.ipynb`   | Converts DBF → CSV, applies metadata mapping              |
| `cenagro_branch_goal_architechture.ipynb` | Establishes Git subtree architecture and regional logic   |
| `cenagro_onedrive_injection_githubclone.ipynb` | Injects OneDrive-based data to GitHub structure       |

---

## 🔀 Modular Git Subtree Usage

Each region’s data is managed via Git subtrees to preserve modularity and traceability:

```bash
git subtree add --prefix=data/cenagro_2012/amazonas remote_repo main --squash
git subtree push --prefix=data/cenagro_2012/amazonas remote_repo main
```

---

## 🧾 Requirements

See `requirements.txt`. For reproducibility:

```bash
pandas==2.1.4
scikit-learn==1.4.2
xgboost==2.0.3
matplotlib==3.8.2
jupyter==1.0.0
notebook==7.1.3
python-dotenv==1.0.1
```

---

## 📬 Contact

**Balcon Group**  
Project Lead: **Jose Carlo Burga**  
GitHub: [github.com/Balcon-Group](https://github.com/Balcon-Group)

---
