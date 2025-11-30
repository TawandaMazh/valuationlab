# ValuationLab – Corporate Valuation & Forecasting Platform

## Overview
ValuationLab is a corporate valuation and forecasting platform that combines time‑series modelling, discounted cash‑flow (DCF) valuation and sensitivity analysis to evaluate businesses. The project demonstrates financial modelling knowledge and data analytics skills by automating revenue and cost forecasts, computing the weighted average cost of capital (WACC) and net present value (NPV), and providing interactive dashboards and professional reports.

## Business problem
Equity analysts need a rigorous valuation of a target firm to inform investment decisions. Traditional spreadsheets are error‑prone and lack reproducibility. This project builds a data‑driven platform that forecasts financial statements, performs a DCF valuation and analyses how changes in growth rates and discount rates affect valuations.

## Features
- Ingest and clean historical financial statement data via SQL pipelines.
- Forecast revenues and costs using ARIMA/Prophet time‑series models【418713139711144†L79-L99】.
- Project free cash flows, compute WACC and perform a DCF valuation【924890776488646†L327-L351】.
- Conduct sensitivity analysis on growth and discount rates to understand valuation drivers【456937291416347†L276-L342】.
- Provide an Excel model for auditors and Power BI/Tableau dashboards with forecasts, NPV and sensitivity charts.
- Generate a PDF report summarising assumptions, valuation results and investment recommendations.

## Repository structure
```
/valuationlab
    /data          # historical financial statements & forecasts
    /src           # Python modules for forecasting, DCF valuation & sensitivity analysis
    /notebooks     # notebooks illustrating forecasting, valuation & scenario analysis
    /dashboards    # interactive dashboards with financial forecasts & DCF outputs
    /docs          # valuation report, assumptions & model diagrams
    requirements.txt
    README.md
```

## Getting Started
1. Clone the repository and create a virtual environment.
   ```bash
   git clone https://github.com/your-username/valuationlab.git
   cd valuationlab
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```
2. Ingest and clean the dataset by running the SQL scripts in `/src` (or place the prepared CSVs in `/data`).
3. Run the notebooks in `/notebooks` to build forecasts, compute the DCF valuation and perform sensitivity analysis.
4. Open the dashboard in Power BI or Tableau (`/dashboards`) to interactively explore forecasts, valuation and scenarios.
5. Read the report in `/docs` for a summary of assumptions and results.

## Deliverables
- Cleaned dataset of historical financial statements.
- Python scripts/notebooks performing time‑series forecasting, DCF valuation and sensitivity analysis.
- SQL scripts for data ingestion and transformation.
- Excel workbook replicating the DCF model.
- Power BI/Tableau dashboard showing forecasts, NPV calculations and sensitivity charts.
- PDF executive summary with key assumptions, valuation results and investment guidance.
- README describing installation, methodology and scenario analysis.

## Extensions
Future enhancements could include:
- Scenario analysis with multiple macroeconomic cases (recession, base, growth).
- Monte‑Carlo simulation for distributions of valuation outcomes.
- Web interface allowing analysts to adjust assumptions and generate updated reports.
