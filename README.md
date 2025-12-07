# ☁️ Open-Meteo Weather Forecast ETL

This project performs an ELT workflow using the Open-Meteo API and pandas.

## Data Source
* **Source:** Open-Meteo Public API (Weather Forecast)
* **Location:** Lisbon, Portugal (38.7167, -9.1333)

## Transformations
1.  **Selection and Renaming:** Columns were selected and renamed for clarity (e.g., 'time' to 'Date', 'temperature_2m_max' to 'Max_Temp_C').
2.  **New Column:** Calculated 'Temp_Range_C' (Max_Temp_C - Min_Temp_C).

## How to Execute
This project was built and executed in Google Colab.

1.  Mount Google Drive.
2.  Run the ELT script.
3.  The output is saved to `data/processed/output.csv` in the project directory.

## Output Structure (data/processed/output.csv)
| Date | Max_Temp_C | Min_Temp_C | Precip_mm | Temp_Range_C |
|:---|:---|:---|:---|:---|
