# Data Wrangling — Milestone 2

## 1. Tools Used
- Tableau Desktop (Chinese UI): used to filter country records, pivot (transpose) year columns into long format, and check missing values
- Microsoft Excel (.xlsx): used to paste Tableau outputs, standardize column headers, sort, and export as CSV

## 2. Raw Data Overview
This project uses World Bank WDI indicator datasets downloaded as Excel (.xls):
- SDG 7.2.1: EG.FEC.RNEW.ZS (Renewable energy share of total final energy consumption)
- SDG 7.3.1: EG.EGY.PRIM.PP.KD (Energy intensity of primary energy, MJ per 2021 PPP GDP)

Key characteristics of the raw files:
- The datasets are in wide format: years (e.g., 1990, 1991, …) are stored as separate columns, which is not ideal for time-series and relationship charts in Tableau.
- Some years contain missing values (e.g., NULL).

## 3. Cleaning Goals
- Keep only Canada records
- Convert wide format to long format with consistent fields:
  - `Year`
  - indicator value column (`Renewables_Share` for 7.2.1, `Energy_Intensity` for 7.3.1)
- Export reproducible, visualization-ready CSV files
- Create a merged dataset for relationship analysis (scatter plot) using overlapping years only

## 4. Cleaning Steps in Tableau Desktop
### 4.1 SDG 7.2.1 (EG.FEC.RNEW.ZS)
1) Connected the raw .xls file and selected the `Data` sheet
2) Confirmed the file contains `Country Name / Country Code / Indicator Name / Indicator Code` plus multiple year columns
3) Filtered records to keep only `Country Name = Canada`
4) Selected all year columns (e.g., 1990 to the last year) and used Tableau’s transpose/pivot function to convert the table into long format
5) Renamed the generated fields to:
   - `Year`
   - `Renewables_Share`
6) Verified the structure is “one row per year” and the value field is numeric
7) Missing values: some years (e.g., 2022) are NULL. No imputation was performed; missing values can be filtered during export/visualization if needed.

### 4.2 SDG 7.3.1 (EG.EGY.PRIM.PP.KD)
Repeated the same steps as 7.2.1:
1) Connected the raw .xls file and selected the `Data` sheet
2) Filtered to keep only Canada
3) Transposed/pivoted year columns into long format
4) Renamed fields to:
   - `Year`
   - `Energy_Intensity`
5) Verified Year is an integer year and Energy_Intensity is numeric
6) Applied the same missing-value rule: no imputation, only documented and filtered when needed.

## 5. Exporting Cleaned Results (Tableau → Excel → CSV)
To ensure the final outputs are standard text-based CSV files, I used the following workflow:
1) Built a simple two-column table in Tableau (Year + indicator value)
2) Copied the table output and pasted it into Excel (.xlsx)
3) In Excel:
   - Confirmed headers are `Year` and the correct indicator column name (`Renewables_Share` or `Energy_Intensity`)
   - Sorted by `Year` ascending (optional but improves readability and checking)
4) Used Excel “Save As” to export as CSV (comma-delimited)

Clean CSV outputs:
- `7.2.1_clean_Canada_renewables_share_EG.FEC.RNEW.ZS.csv`
- `7.3.1_clean_Canada_energy_intensity_EG.EGY.PRIM.PP.KD.csv`

## 6. Combined Dataset (Overlapping Years / Inner Join by Year)
For the scatter plot and relationship analysis between the two indicators, I created a merged dataset:
1) Matched the two cleaned CSV files using `Year` as the key
2) Kept only the overlapping years (years present in both datasets), equivalent to an inner join by Year
3) Output structure includes three columns:
   - `Year`
   - `Renewables_Share`
   - `Energy_Intensity`

Combined CSV output:
- `combined_CA_renewables_share_and_energy_intensity_by_year.csv`

Notes:
- The two indicators have different year coverage. To avoid missing values affecting relationship analysis, the merged dataset uses overlapping years only.
- Trend charts are still produced from each indicator’s full time series and do not rely on the merged dataset.

## 7. Assumptions & Limitations
- No missing-year imputation was performed to avoid introducing bias.
- The merged dataset is used only for relationship analysis (e.g., scatter plot) and does not replace full time-series analysis.
- Indicator definitions follow the World Bank series descriptions and SDG-aligned measures.
