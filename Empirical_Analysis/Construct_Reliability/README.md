# Overview
This repository contains three Python codes designed to evaluate the reliability of survey items (from a questionnaire using a seven-point Likert-type scale with end points of ‘strongly disagree’ and ‘strongly agree’) and to perform normality tests on data. Specifically, the scripts compute:

 1. **Cronbach’s Alpha** ,
 2. **Kendall’s Tau** correlation coefficient, and
 3. **Shapiro–Wilk normality tests** for each item (column) in a dataset.

Below is an overview of the purpose and usage of each code snippet.
## Table of Contents  :memo:

1.  [Requirements](#requirements)
2.  [Data Structure](#data-structure)
3. [How to Run](#how-to-run)

----------

## Requirements :wrench:

-   **Python 3.7+**
-   **NumPy** (for array manipulation)
-   **Pandas** (for tabular data handling)
-   **SciPy** (for statistical tests)
-   **Matplotlib** & **Seaborn** (optional, in case you need any plotting)

Install the packages via:

    pip install numpy pandas scipy matplotlib seaborn

----------

## Data Structure :bulb:

1.  **`data`**: A NumPy array of shape (n_samples, n_items). Each row corresponds to a participant’s responses, and each column corresponds to a survey question (item).
    
2.  **`constructs`**: A list of lists, where each sub-list contains the indices of items belonging to a particular construct. For example:

 

       constructs = [
        [0, 1],        # Construct 1 (items Q1, Q2)
        [2, 3, 4],     # Construct 2 (items Q3, Q4, Q5)
        [5, 6]       # Construct 3, etc.
    ]
    
    
----------

## How to Run :checkered_flag:

1.  **Clone or download** this repository.
2.  **Open a Python session or Jupyter Notebook** in the directory containing the scripts.
3.  **Replace** the `data = np.array([...])` sections with your actual dataset (NumPy array or pass in the Pandas DataFrame’s values).
4.  **Replace** or **verify** that `constructs` aligns with your survey item indices.
5.  **Run** each script block (you may run them in the same script or separately as needed).

