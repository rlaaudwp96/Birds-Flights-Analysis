# Bird Flight Phase Analysis

**Author:** Myungje Kim  
**Program:** M.S. Data Science (Statistics), California State University East Bay  

---

## Project Overview

This project explores the relationship between **phase of flight** and **time of day** using the `birds` dataset from the `openintro` R package.

The goal of the analysis is to examine how bird flight behavior varies across different times of the day and identify patterns in flight phases. The project uses exploratory data analysis and visualization to understand these relationships.

---

## Dataset

Source: `openintro::birds`

The dataset contains observations of bird flight behavior and includes categorical variables describing the phase of flight and the time of day when the observation occurred.

Key variables used in this project:

| Variable | Description |
|--------|-------------|
| `phase_of_flt` | Phase of bird flight (e.g., flapping, gliding, soaring) |
| `time_of_day` | Time period when the observation was recorded |
| `state` | Location where the observation was recorded |

For this analysis:

- Missing observations were removed.
- The variables `phase_of_flt` and `time_of_day` were converted into categorical factors.
- The dataset was separated into two groups:
  - Observations from **California**
  - Observations from **other states**

This allows comparison of flight behavior across different locations.

---

## Methods

The following steps were used in the analysis:

1. **Data Loading**
   - Imported the birds dataset from the `openintro` package.

2. **Data Cleaning**
   - Removed missing values.
   - Converted categorical variables into factors.

3. **Data Subsetting**
   - Created separate datasets for California and non-California observations.

4. **Exploratory Data Analysis**
   - Frequency counts of flight phases.
   - Distribution of flight phases across time of day.

5. **Visualization**
   - Bar charts showing the relationship between time of day and flight phase.

---

## Tools and Libraries

This project was completed using:

- **R**
- **Quarto**
- **tidyverse**
- **openintro**
- **ggplot2**

---

## Repository Structure
```
Bird-Flight-Analysis
│
├── Myungje_Kim_Final_Project.qmd
├── Myungje_Kim_Final_Project.html
└── README.md
```

| File | Description |
|----|----|
| `Myungje_Kim_Final_Project.qmd` | Quarto source file containing the full analysis |
| `Myungje_Kim_Final_Project.html` | Rendered report with code, analysis, and visualizations |
| `README.md` | Project documentation |

---

## Key Findings

- Bird flight behavior varies across different times of the day.
- Certain flight phases appear more frequently during specific periods.
- Separating California observations allows comparison with observations from other states.

Further analysis could apply statistical modeling to formally test the relationship between time of day and flight phase.

---

## Reproducibility
To reproduce the analysis:

1. Clone this repository.
2. Open the `.qmd` file in **RStudio**.
3. Run:

```r
quarto render Myungje_Kim_Final_Project.qmd
```

This will generate the HTML report.

---

## Future Work

Possible extensions of this project include:

- Logistic regression modeling of flight phase probabilities
- Time-based analysis of bird flight behavior
- Spatial analysis of bird observations
- Machine learning classification of flight phases

---

## License

This project is intended for academic and educational purposes.
