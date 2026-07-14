# Unemployment Analysis in India

This project explores unemployment data across Indian states and looks at how the COVID-19 lockdown affected unemployment rates.

## Dataset

`Unemployment_in_India.csv` has the following columns:
- Region
- Date
- Frequency
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Area

Note: The original brief pointed to a dataset on Kaggle called "Unemployment in India". Since I couldn't access Kaggle directly, I put together a dataset with the same structure (same columns, same kind of state-wise monthly data, and a realistic spike in unemployment during the April 2020 lockdown period) so the notebook can be run and explored right away. If you'd rather use the real Kaggle dataset, just download it and replace this CSV with the same filename — the notebook will work the same way.

## What's in the notebook

- Loading and cleaning the data (nulls, date conversion)
- Region-wise and month-wise average unemployment
- Time series line chart for 3 major states
- Bar chart of top 10 states by average unemployment rate
- Correlation heatmap (unemployment rate, employed, labour participation rate)
- Pre-COVID vs post-COVID comparison
- Short notes explaining each chart

## How to run

1. Install the required packages:
   ```
   pip install pandas numpy matplotlib seaborn
   ```
2. Keep `Unemployment_in_India.csv` in the same folder as the notebook.
3. Open `unemployment_analysis.ipynb` in Jupyter Notebook or JupyterLab.
4. Run all cells from top to bottom.

## Result

Unemployment rates jump sharply for all states starting around April 2020, matching the COVID lockdown period, and drop back down somewhat in the following months.
