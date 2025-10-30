# Pandas Data Analysis Exercise

## 1. Project Overview
This repository contains a collection of data analysis exercises completed using Python and the Pandas library. The projects demonstrate a range of core data manipulation and analysis skills, from basic data loading and cleaning to more advanced filtering, grouping, and merging techniques. Each project is self-contained within a Jupyter Notebook and uses a distinct dataset to solve a specific analytical task.

## 2. The Projects

---

### Project 1: Hogwarts Student Roster Analysis
*   **Notebook:** [`hogwarts-student-analysis.ipynb`](./hogwarts-student-analysis.ipynb)
*   **Datasets:** `ErstSemester.csv`, `StudierendenDaten.csv` (fictional student data).
*   **Description:** This analysis explores a fictional dataset of Hogwarts students (in German). The primary goal was to practice fundamental data wrangling tasks, including combining separate datasets, performing categorical analysis, and creating new features from existing columns to build a unified student roster.
*   **Key Skills Demonstrated:**
    *   **Data Loading & Inspection:** Reading multiple CSV files into Pandas DataFrames and using `.head()` and `.count()` for initial assessment.
    *   **Data Aggregation:** Using `value_counts()` to analyze the distribution of students by gender (`Geschlecht`) and House (`Haus`).
    *   **Grouping & Segmentation:** Applying `groupby()` to segment the data by category (e.g., by House) and perform calculations on each group.
    *   **Filtering & Subsetting:** Using boolean masking and `.loc` to create subsets of the data (e.g., filtering for only male students or students in a specific House).
    *   **Feature Engineering:** Creating new columns with `assign()` by combining `Vorname` and `Nachname` into a full name, and by extracting a username from the `E-Mail` column.
    *   **Data Merging:** Combining two separate student datasets into a single, comprehensive DataFrame using both `pd.concat()` and `pd.merge()`.

---

### Project 2: Stack Overflow Developer Survey Analysis
*   **Notebook:** [`stackoverflow-survey-analysis.ipynb`](./stackoverflow-survey-analysis.ipynb)
*   **Datasets:** `survey_results_public.csv`, `survey_results_schema.csv` (2023 Stack Overflow Developer Survey).
*   **Description:** This notebook performs an exploratory analysis of the official 2023 Stack Overflow Developer Survey. The focus is on demonstrating proficiency with Pandas' powerful indexing and filtering capabilities to answer specific questions about a large, real-world dataset.
*   **Key Skills Demonstrated:**
    *   **Data Exploration:** Using `.shape`, `.info()`, `.head()`, and `.columns` to inspect a large dataset with over 65,000 rows and 100+ columns.
    *   **Advanced Indexing:** Setting a meaningful index column (`index_col`) on data load and using `.loc` for label-based lookups.
    *   **Conditional Filtering:** Creating complex boolean masks to filter the data based on multiple conditions (e.g., developers with high salaries in specific countries).
    *   **Querying with String Methods:** Using the `.str.contains()` method to filter rows where a column contains a specific substring (e.g., finding all developers who want to work with Python).
    *   **Sorting & Slicing:** Using `sort_index()` and slicing (`df.loc[start:stop]`) to organize and view specific portions of the data.

## 3. Technical Stack
*   **Language:** Python
*   **Core Library:** Pandas
*   **Environment:** Jupyter Notebook

## 4. Repository Structure
The repository is organized for clarity and reproducibility:
```
/
├── data/
│ ├── ErstSemester.csv
│ └── StudierendenDaten.csv
│
├── hogwarts-student-analysis.ipynb
├── stackoverflow-survey-analysis.ipynb
├── .gitignore
└── README.md
```
## 5. How to Use
1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-username/pandas-data-analysis-projects.git
    cd pandas-data-analysis-projects
    ```
2.  **Download the Large Datasets:**
    The Stack Overflow survey files are too large for GitHub. Download them from the official Kaggle source:
    *   **[Download Link](https://www.kaggle.com/datasets/stackoverflow/stack-overflow-developer-survey-2023)**
    *   After downloading, place `survey_results_public.csv` and `survey_results_schema.csv` inside the `data/` folder.

3.  **Install Dependencies:**
    Ensure you have Python installed. Then, install the required libraries:
    ```bash
    pip install pandas jupyter
    ```
4.  **Run the Analysis:**
    Launch Jupyter from the main project folder:
    ```bash
    jupyter notebook
    ```
    From the Jupyter interface in your browser, you can open either of the `.ipynb` files to view and run the analysis.
