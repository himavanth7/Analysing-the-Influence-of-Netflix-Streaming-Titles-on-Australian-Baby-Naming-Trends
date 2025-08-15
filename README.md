# Analysing the Influence of Netflix Streaming Titles on Australian Baby Naming Trends

This repository contains the complete code, data notes, figures, and LaTeX sources for the Big Data Analysis project.  
The study investigates how Netflix releases may influence baby naming trends in South Australia.

---

## 📌 Abstract
This project explores the relationship between Netflix streaming titles and the popularity of baby names in South Australia (2014–2024).  
The analysis involves big data techniques, including data preprocessing, exploratory analysis, feature engineering, and predictive modelling, to identify trends and possible cultural influence.

---

## 📂 Repository Structure

```
baby_names/              # South Australian baby name data (2014–2024)
netflix_data/            # Netflix titles metadata (Kaggle)
figures/                 # Generated plots and visualisations
reports/                 # LaTeX source and final PDF
env/                     # Environment setup files
code.ipynb               # Main Jupyter Notebook for analysis
code pdf.pdf             # Executed notebook in PDF format
```

---

## ⚙️ Setup & Installation

**Requirements:**  
- Python 3.10+
- Jupyter Notebook
- Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

**1. Clone the repository**
```bash
git clone https://github.com/himavanth7/Analysing-the-Influence-of-Netflix-Streaming-Titles-on-Australian-Baby-Naming-Trends.git
cd Analysing-the-Influence-of-Netflix-Streaming-Titles-on-Australian-Baby-Naming-Trends
```

**2. Create and activate a virtual environment**
```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

---

## ▶️ Reproducing Results

**1. Run the full analysis**
```bash
jupyter nbconvert --to notebook --execute code.ipynb --output executed.ipynb
```

**2. Generate all figures**
```bash
make figures
```

**3. Build the LaTeX report locally** *(optional if using Overleaf)*
```bash
make report
```

---

## 📊 Methodology
The project follows 5 main phases:
1. **Data Collection** – Importing Netflix and SA baby name datasets.
2. **Data Preprocessing** – Cleaning, filtering, and preparing datasets for analysis.
3. **Exploratory Data Analysis (EDA)** – Visualising trends and relationships.
4. **Model Training** – Implementing classification models to predict name influences.
5. **Reproducibility** – Providing scripts, environment files, and documentation.

---

## 📎 Replication Package
- **GitHub Repository:** [Project Link](https://github.com/himavanth7/Analysing-the-Influence-of-Netflix-Streaming-Titles-on-Australian-Baby-Naming-Trends)  
- **Overleaf Report Link:** [Overleaf Link](https://www.overleaf.com/read/mzmfwwmhtmwy#fde3d2).

The repository is organised and documented to allow full reproduction of results.

---
**Author:** Himavanth Reddy Kalakota  
**University of Adelaide – Master of Data Science**
