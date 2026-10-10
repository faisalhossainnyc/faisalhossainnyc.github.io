# NYC Civilian Complaint Records

Exploratory Analysis and Data Quality Assessment

An exploratory analysis of 10,000 NYC Civilian Complaint Review Board (CCRB) allegation records using Python, pandas, Matplotlib, and Seaborn. The project examines allegation categories, recorded outcomes, officer rank and tenure, and how missing information and changes in data collection affect interpretation.

**Authors:** Faisal Hossain and Jason Wilson

**Original context:** CIS 9650 final project

## Read the analysis

- [Read the report](https://faisalhossainnyc.github.io/projects/nyc-civilian-complaints/) — a standalone HTML report with all 16 charts embedded.
- [View the notebook](analysis.ipynb) — the Python code, explanations, and saved outputs.

Reading either version requires no API key or Python setup. You can also download `index.html` and open it directly in a browser.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Readable report with expandable code and detailed outputs. |
| `analysis.ipynb` | Source notebook with its saved charts and results. |

## Run the notebook

1. Download `analysis.ipynb` and open it in Google Colab.
2. The first cell mounts Google Drive; run it if needed, or skip it when using Colab's runtime storage. The CSV paths in the notebook are relative to the working directory.
3. Run the remaining cells from the API setup through the analysis. The notebook installs `sodapy`; Colab provides pandas, Matplotlib, and Seaborn.
4. The retrieval and cleaning steps generate `Allegations.csv` and `Allegations_cleaned.csv` in the working directory.

An optional Socrata application token can be provided through the `SOCRATA_APP_TOKEN` environment variable before running the API setup cell. The notebook can retrieve public data without a token, subject to the service's throttling limits. The API contains live data, so rerunning may produce different results from the saved report.

## Data source and interpretation

[NYC Open Data — CCRB Allegations Against Police Officers](https://data.cityofnewyork.us/d/6xgr-kwjq), retrieved through the Socrata API.

An allegation is a recorded claim, and a complaint can contain multiple allegations. The notebook documents its custom category mappings and the data quality limitations relevant to its findings.
