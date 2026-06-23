# World Happiness Report 2023: Exploratory Data Analysis

> Exploratory Data Analysis on the World Happiness Report 2023, focusing on the relationship between Ladder Score and Healthy Life Expectancy across the Top 15 happiest countries.

---

## Objective:

To find the relationship between **Ladder Score** (Happiness Score) and **Healthy Life Expectancy** among the Top 15 happiest countries in the world (2023).

---

## Dataset:

- **Source:** [Kaggle: World Happiness Report 2023](https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2023)
- **Scope:** Filtered to the **Top 15 happiest countries** of 2023
- **Format:** CSV

**Key variables used:**

| Variable | Description |
|---|---|
| `Ladder score` | Happiness score of the country (0–10 scale) |
| `Healthy life expectancy` | Average number of years a person can expect to live in good health |
| `Logged GDP per capita` | Log of GDP per capita |
| `Social support` | Perceived social support from friends/family |
| `Freedom to make life choices` | Perceived freedom in life decisions |
| `Generosity` | Charitable giving measure |
| `Perceptions of corruption` | Perceived corruption in government/business |

---

## Libraries Used:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## Graphs & Analysis:

The following charts were used to explore the data:

1. **Histogram** — Distribution of Ladder Score and Healthy Life Expectancy
2. **KDE Plot** — Density distribution of both variables
3. **Scatterplot** — Relationship between HLE and Ladder Score
4. **Line Plot** — Trend between HLE and Ladder Score
5. **Boxplot** — Spread and outliers in both variables
6. **Heatmap** — Correlation between all key variables

---

## Key Findings:

- There is a **moderate positive correlation (r ≈ 0.45)** between Healthy Life Expectancy and Ladder Score
- **Social Support (r ≈ 0.63)** and **Freedom (r ≈ 0.60)** are the strongest predictors of happiness within this group
- The **United States** is a consistent outlier; it has the lowest HLE (65.85 years) and the lowest Ladder Score (6.894) among the Top 15, despite being in the global top tier
- Most top-ranked countries have HLE clustered tightly between **71–73 years**, showing similar health outcomes

---

## Conclusion:

The objective was fulfilled. The EDA confirms a **moderate positive relationship** between Healthy Life Expectancy and Ladder Score. However, HLE alone does not fully determine happiness — social support and personal freedom play an equally significant role at this level.

---

## Project Structure:

```
world-happiness-eda/
│
├── Main.ipynb          # Jupyter Notebook with full EDA
├── WHR2023.csv         # Dataset (Top 15 countries)
└── README.md           # Project documentation
```

---

## How to Run:

1. Clone the repository
```bash
git clone https://github.com/riwazzzz/world-happiness-eda.git
```

2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn
```

3. Open the notebook
```bash
jupyter notebook Main.ipynb
```

---

*Data Source: World Happiness Report 2023 via Kaggle*
