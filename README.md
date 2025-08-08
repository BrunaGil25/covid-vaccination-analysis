# COVID-19 Vaccination & Mortality Analysis

## Overview

This project explores the relationship between COVID-19 vaccination rates and pandemic outcomes across continents using regression modeling and diagnostics. It combines global and regional data to assess the impact of vaccination on death rates, ICU burden, and case counts.

## Objectives

- Quantify the effect of vaccination on COVID-19 deaths globally and regionally
- Compare regression outcomes across continents
- Evaluate model assumptions and reliability using diagnostics
- Assess generalizability through cross-validation
- Provide actionable insights for public health policy

## Structure

| Section | Description |
|--------|-------------|
| **1–2** | Data loading and preprocessing |
| **3–4** | Exploratory data analysis and visualization |
| **5**   | Correlation heatmaps by continent |
| **6**   | Regression modeling (global, regional, multivariate) |
| **7**   | Model diagnostics (residuals, VIF) |
| **8**   | Cross-validation using GroupKFold |
| **9**   | Conclusion and policy implications |

## Methods

- **OLS Regression**: Global and continent-level models
- **Multivariate Regression**: Includes case rates and ICU burden
- **Residual Analysis**: Scatter plots, histograms, QQ-plots
- **Multicollinearity Check**: Variance Inflation Factor (VIF)
- **Cross-Validation**: GroupKFold by continent

## Key Findings

- Vaccination is consistently associated with reduced death rates
- Regional variation is significant—Oceania shows anomalous trends
- Multivariate models improve explanatory power (R² = 0.243)
- Diagnostics reveal non-normality and heteroscedasticity
- Cross-validation confirms geographic variability in model performance

## Policy Relevance

- Supports targeted vaccination strategies
- Highlights need for region-specific public health planning
- Emphasizes importance of data quality and transparency

##  Datasets Used

This project uses two datasets:

1. **OWID COVID-19 Data**  
   - Source: [Our World in Data](https://your-link.com/owid-covid-data.csv)  
   - ⚠️ Not included in this repo due to size.  
   - **Instructions**:  
     - Download the file from the link above  
     - Place it in the `data/` folder as `owid-covid-data.csv`

2. **Vaccination Data**  
   - Included in the repository as `data/vaccination-data.csv`

⚠️ Make sure both datasets are in the `data/` folder:


## Generated Visuals

All correlation matrices, residual plots, histograms, and QQ-plots were generated using:
- `matplotlib`
- `seaborn`
- `statsmodels`
- `scipy`

You can find the full set of images in this repository.

## Requirements

- Python 3.x
- `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `scikit-learn`, `scipy`

## To run this project locally:

1. Clone the repository
git clone https://github.com/BrunaGil25/covid-vaccination-analysis.git
cd covid-vaccination-analysis

2. Create a virtual environment
python -m venv venv

3. Activate the virtual environment
 Use the appropriate command for your system:
 - Windows
   venv\Scripts\activate

- macOS/Linux
  source venv/bin/activate

4. Install dependencies
pip install -r requirements.txt

5. (Optional) Install Jupyter Lab if not already installed
pip install jupyterlab

6. Launch the notebook
jupyter lab


## Author

Bruna — COVID-19 data analyst and public health enthusiast

---


