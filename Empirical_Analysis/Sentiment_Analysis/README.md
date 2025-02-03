# Overview
This repository contains a Python script that utilizes **TextBlob** and its **PatternAnalyzer** module to perform sentiment analysis on textual data. The script evaluates the sentiment polarity of a given text and categorizes it as positive, negative, or neutral. This is particularly useful for general text sentiment evaluation.

---

## Table of Contents :memo:

1. [Requirements](#requirements)  
2. [Key Features](#key-features)  
3. [How to Run](#how-to-run)  
4. [Example Output](#example-output)  

---

## Requirements :wrench:

- **Python 3.7+**  
- **TextBlob** (for sentiment analysis using PatternAnalyzer)  

Install the required package via:

    pip install textblob

----------
## Key Features :star:

-   **Sentiment Analysis**:
    -   Calculates the polarity of text using TextBlob’s **PatternAnalyzer**.
    -   Classifies the sentiment into one of three categories:
        -   **Positive** (polarity > 0)
        -   **Neutral** (polarity = 0)
        -   **Negative** (polarity < 0)

    - Polarity values range from -1 to 1.
----------

## How to Run :checkered_flag:

1.  **Clone or Download** this repository.
2.  **Set Up Text Data**:
    -   Update the `textos` list with the texts you want to analyze.
    -   Example:
    -
        `textos = [
            "I love this product!",
            "It's okay, nothing special.",
            "I really dislike the service."
        ]` 
        
3.  **Run the Script**:
    -   Execute the script in any Python environment (e.g., Jupyter Notebook).
4.  **View Results**:
    -   The script will print the sentiment and polarity for each input text.

----------

## Example Output :bar_chart:

Given the following input:

`textos = [
    "I love this product!",
    "It's okay, nothing special.",
    "I really dislike the service."
]` 

The output will be:

    Texto: I love this product!
    Sentimento: positivo
    Polaridade: 0.5
    --------------------------------------------------
    Texto: It's okay, nothing special.
    Sentimento: neutro
    Polaridade: 0.0
    --------------------------------------------------
    Texto: I really dislike the service.
    Sentimento: negativo
    Polaridade: -0.6
    --------------------------------------------------

-----------------------------------------

