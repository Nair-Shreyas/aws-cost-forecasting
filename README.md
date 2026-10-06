# Forecasting & Visualizing AWS Cloud Costs

![Project Overview](docs/images/1_project_overview.png)

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python: 3.12"/>
  <img src="https://img.shields.io/badge/Runs_on-Google_Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=white" alt="Runs on: Google Colab"/>
  <img src="https://img.shields.io/badge/Data-AWS_usage_%26_cost-c9440c?style=flat-square" alt="Data: AWS usage & cost"/>
</p>

A data analysis project exploring AWS usage and cost patterns, combining exploratory analysis, visualization, and simple predictive modeling to understand what drives cloud spend over time.

## What it does
- Grouped summaries of cost by service, region, and date
- Dual-axis visualizations comparing daily cost against usage hours, to see whether usage actually drives cost
- Exploratory analysis to surface spending trends and anomalies
- A 15-day cost forecast based on historical trends

`aws_usage.csv` is bundled so the notebook runs standalone — no external downloads needed.

## Results

Daily cost tracks usage hours fairly closely, with a few notable spikes worth digging into:

![Dual Axis Cost vs Usage](docs/images/2_dual_axis_cost_usage.png)

A 7-day rolling average smooths out day-to-day noise to reveal the underlying trend:

![Rolling Average](docs/images/3_rolling_average.png)

Projecting forward from historical patterns:

![Forecast](docs/images/4_forecast.png)

## Tech
Python, pandas, NumPy, matplotlib, seaborn, scikit-learn
