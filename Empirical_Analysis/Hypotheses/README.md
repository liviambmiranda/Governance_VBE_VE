# Overview

This repository contains Python code designed to evaluate statistical properties of survey data (from a questionnaire using a seven-point Likert-type scale with end points of ‘strongly disagree’ and ‘strongly agree’) using non-parametric methods. It includes functionality to calculate:

1. **Cliff’s Delta** (a effect size measure),  
2. **Confidence intervals for Cliff’s Delta**, and  
3. **Exact procedure of Wilcoxon signed-rank test** (to compare medians against a hypothesized value).


## Table of Contents :memo:

1. [Requirements](#requirements)  
2. [Data Structure](#data-structure)  
4. [How to Run](#how-to-run)  

---

## Requirements :wrench:

- **Python 3.7+**  
- **NumPy** (for numerical operations)  
- **SciPy** (for statistical tests and distributions)  

Install the required packages via:

    pip install numpy scipy

---


## Data Structure :bulb:

1.  **`data`**: A NumPy array of shape (n_samples, n_items). Each row corresponds to a participant’s responses, and each column corresponds to a survey question (item).
    
2.  **`constructs`**: A list of lists, where each sub-list contains indices for items that belong to a specific construct. For example:

  `constructs = [
        [0, 1],        # Construct 1 (items Q1, Q2)
        [2, 3, 4],     # Construct 2 (items Q3, Q4, Q5)
        [5, 6]       # Construct 3, etc.
        ]`
    
 3. **`hypothesized_median`**: A numeric value (e.g., `4` on the 7-point Likert scale) against which the medians of survey responses are tested.
    
----------

## How to Run :checkered_flag:

1. **Clone or Download** the repository.
2.  **Set Up Data**:
    -   Replace the `data` variable with your dataset.
    -   Update `constructs` to match your survey's structure.
3.   **Run the Code**:
    -   Open the file in a Python environment (e.g., Jupyter Notebook or an IDE).
    -   Execute the script.
4.   **View Results**:
    -   Results include detailed outputs for each test and descriptive statistics.



