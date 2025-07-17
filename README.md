# Data-analyst-project2
# 🎬 Movie Data Cleaning & Preprocessing Project

A professional data cleaning project that processes and prepares a raw movie dataset for analysis. This project demonstrates key skills in **data wrangling**, **data transformation**, and **feature engineering** using Python libraries such as **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn** within a Jupyter Notebook environment.

---

## 📌 Objective

The primary objective of this project is to clean and structure a raw dataset containing metadata about movies, enabling reliable downstream analysis and visualization. The notebook handles inconsistencies, missing values, formatting errors, and prepares features that are ready for Exploratory Data Analysis (EDA) or modeling tasks.

---

## 🗂️ Project Structure

```
movie-data-cleaning/
│
├── moviesclean.ipynb       # Jupyter notebook with the full cleaning workflow
├── movies.csv              # Raw dataset (not included in repo for size/privacy)
├── README.md               # Project documentation (this file)
└── requirements.txt        # Optional: list of dependencies
```

---

## 📊 Dataset Overview

The dataset (assumed as `movies.csv`) includes various columns such as:

* 🎞️ `TITLE`: Movie name
* 📆 `YEAR`: Year of release (to be cleaned)
* 🕐 `RunTime`: Duration of the movie (cleaned & renamed to `RUNTIME`)
* 💰 `Gross`: Box office gross (cleaned & renamed to `GROSS`)
* 📝 `ONE-LINE`: Short description or tagline
* 🌟 `STARS`: Star cast (removed)
* ...and potentially other metadata

---

## 🔧 Features & Processing Steps

### ✅ Cleaning Workflow Includes:

* **Data Loading**

  * Read CSV into a Pandas DataFrame.

* **Data Inspection**

  * Use `df.info()`, `df.describe()`, and `df.head()` to understand structure and quality.

* **Column Renaming**

  * Renamed `RunTime` ➝ `RUNTIME`
  * Renamed `Gross` ➝ `GROSS`

* **Data Type Conversion**

  * Extracted 4-digit year using regular expressions.
  * Converted numeric columns to appropriate types.

* **Missing Value Handling**

  * Replaced invalid placeholders (`'nan'`, `'\\nAdd a Plot\\n'`) with actual `NaN`.
  * Dropped or imputed rows/columns as necessary.

* **Feature Selection**

  * Removed non-informative or redundant columns like `STARS`.

* **Initial Cleaning Summary**

  * Dataset is reshaped into a consistent format, suitable for visualization or modeling.

---

## 📈 Future Work (Optional Extensions)

This project is modular and can be extended to include:

* 📊 **Exploratory Data Analysis (EDA)** with visualizations
* 🤖 **Predictive modeling** (e.g., predicting GROSS based on RUNTIME, year, etc.)
* 🧠 **NLP on plot descriptions**
* 📉 **Time-series trends** by year or decade
* 📂 **Genre classification** (if data is available)

---

## 🧰 Technologies Used

| Tool/Library | Purpose                        |
| ------------ | ------------------------------ |
| `pandas`     | Data manipulation              |
| `numpy`      | Numerical computation          |
| `matplotlib` | Static plotting                |
| `seaborn`    | Statistical data visualization |
| `jupyter`    | Notebook-based development     |

---

## ▶️ Getting Started

### 🔨 Requirements

Make sure you have the following installed:

* Python 3.7+
* Jupyter Notebook
* Required libraries (install below)

### ⚙️ Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/movie-data-cleaning.git
cd movie-data-cleaning

# Install dependencies (optional)
pip install -r requirements.txt

# Launch notebook
jupyter notebook moviesclean.ipynb
```

### `requirements.txt` (suggested content)

```txt
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## ✅ Deliverables

* ✔️ A cleaned movie dataset ready for downstream use
* ✔️ Reproducible Jupyter Notebook with documented code
* ✔️ Standard practices in data preparation and validation

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**Your Name**
[GitHub](https://github.com/prem3097)
[LinkedIn](https://www.linkedin.com/in/premkumar-r-ba4a002a1?)

---

## 🙏 Acknowledgements

* Dataset source: \[IMDb or relevant source if known]
* Inspired by best practices in data cleaning and Kaggle competitions

---
