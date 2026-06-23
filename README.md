# Patriotic Songs, National Narratives, and Macroeconomic Conditions in Pakistan (1962–2024)

## Overview

This project investigates how Pakistani patriotic songs reflect and shape national narratives over time. Using a custom Urdu thematic dictionary, the study converts song lyrics into measurable themes and examines their relationship with macroeconomic conditions and political regimes between 1962 and 2024.

The research combines computational text analysis with economic and political data to explore whether patriotic messaging changes during periods of economic stress, political transition, or national events.

---

## Research Questions

* How do patriotic songs construct national narratives in Pakistan?
* Which themes dominate patriotic music over time?
* Do macroeconomic conditions influence the thematic content of patriotic songs?
* How do themes vary across democratic and non-democratic periods?

---

## Dataset

The dataset consists of Pakistani patriotic songs released between 1962 and 2024.

### Data Sources

* ISPR (Inter-Services Public Relations) patriotic songs
* Publicly available patriotic music archives
* YouTube lyric sources and official releases

### Macroeconomic Variables

* GDP
* Inflation
* Unemployment
* Government type (Democracy / Non-democracy)
* Historical event dummies (1965, 1971, 1977, and 1999 periods)

---

## Methodology

### 1. Lyric Collection and Processing

* Patriotic song lyrics were collected and verified manually.
* Lyrics were converted into UTF-8 text files.
* Urdu text was cleaned and standardized for analysis.

### 2. Dictionary Construction

A thematic Urdu dictionary containing more than 1,500 words was developed.

The dictionary was created through:

1. Initial word generation using a Large Language Model (LLM)
2. Review and refinement by an Urdu language expert
3. Iterative updates during lyric processing

### Themes

* National Unity
* State Legitimacy
* Military Defence
* Economic Progress
* Economic Sacrifice
* Future Outlook
* Global Identity

### 3. Theme Scoring

Each song was converted into quantitative theme scores using a lexicon-based approach.

Theme scores were calculated using weighted word frequencies:

* Words unique to a theme received full weight.
* Words shared across multiple themes received proportional weights.

### 4. Statistical Analysis

Theme scores were analyzed using regression models to examine relationships between lyrical themes and:

* GDP
* Inflation
* Unemployment
* Political regime type
* Major historical periods

---

## Project Structure

```text
├── data/
│   ├── lyrics/
│   ├── macroeconomic_data/
│   └── processed_data/
│
├── dictionary/
│   └── full_dictionary.txt
│
├── notebooks/
│   ├── preprocessing.ipynb
│   ├── theme_scoring.ipynb
│   └── regression_analysis.ipynb
│
├── figures/
│   ├── songs_per_year.png
│   ├── dictionary_distribution.png
│   └── wordcloud.png
│
├── src/
│   ├── preprocessing.py
│   ├── scoring.py
│   └── regression.py
│
└── README.md
```

---

## Key Visualizations

* Number of patriotic songs per year (1962–2024)
* Distribution of dictionary words across themes
* Word cloud of thematic vocabulary
* Theme trends over time
* Dual-axis charts comparing themes and macroeconomic indicators

---

## Tools and Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Statsmodels
* OpenPyXL
* WordCloud

---

## Academic Contribution

Most previous lyric-analysis studies rely on English-language NLP methods or translate non-English lyrics before analysis. This project contributes by developing a native Urdu thematic dictionary and applying computational text analysis directly to Urdu patriotic songs, preserving linguistic and cultural context.

---

## Author

Ahmed Riaz

BSc Economics & Mathematics

Research Interests:
Computational Social Science, Political Economy, Text Analysis, Financial Economics, and Applied Machine Learning
