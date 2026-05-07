# TikTok Study Abroad: User Behavior Analysis

This project analyzes how Indonesian youth interact with "Study Abroad" content on TikTok. The goal is to understand their active hours and their interests (Scholarships vs. Life Abroad).

---

## Project Overview
* **Platform**: TikTok.
* **Data Period**: January - August 2025.
* **Keywords**: #KuliahLuarNegeri, #FullyFunded, #HidupDiLuarNegeri.
* **Total Data**: 225 rows of comments.

## Research Questions
1. When are the most active times for users to interact?
2. What is the difference between users looking for scholarships and users looking at life abroad?

## File Structure
* `analyst.ipynb`: Main notebook for descriptive analysis.
* `preprocessing.ipynb`: Notebook for data cleaning.
* `tiktok.csv`: Original raw dataset.
* `tiktok_bersih.csv`: Cleaned dataset after preprocessing.
* `kamusalay.csv`: Dictionary to fix informal Indonesian words.

## Data Preprocessing
Cleaned the data before analysis:
1. **Handling Missing Values**: Fill empty reply counts with 0.
2. **DateTime Conversion**: Change text time to actual date and hour.
3. **Text Cleaning**: Remove emojis, numbers, and punctuation.
4. **Normalization**: Change slang words (e.g., "ga" to "tidak") using `kamusalay.csv`.
5. **Stemming**: Change words to their basic form (e.g., "nilainya" to "nilai") using Sastrawi.

## Key Findings
* **Active Hours**: Users are most active at **19:00 WIB** (7 PM).
* **Active Days**: **Thursday** is the peak day for interactions.
* **User Interest**: Users care more about **Scholarships & Preparation (24.9%)** than Life Abroad (8.3%).
* **Top Topics**: Popular words are **Essay, IELTS, Template, and Australia**.

## Tools Used
* **Python** (Pandas, Matplotlib, Seaborn).
* **NLTK & Sastrawi** (For Indonesian text processing).
* **WordCloud** (For visualization).
