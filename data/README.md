# Data Documentation (Milestone 2)

## Dataset A — SDG 7.2.1 (Renewable energy share of total final energy consumption)
- Source: World Bank
- Web page: https://data.worldbank.org/indicator/EG.FEC.RNEW.ZS
- Access date: 2026-03-01
- License: CC BY 4.0 (as shown on the World Bank indicator page)
- Files stored:
  - data/7.2.1_Canada_raw_worldbank_EG.FEC.RNEW.ZS_DS2_en_excel_v2_68.xls (raw download)
  - clean_CA_renewables_share_EG.FEC.RNEW.ZS.csv (cleaned, Canada-only, long format)

## Dataset B — SDG 7.3.1 (Energy intensity of primary energy, MJ per 2021 PPP GDP)
- Source: World Bank
- Web page: https://data.worldbank.org/indicator/EG.EGY.PRIM.PP.KD
- Access date: 2026-03-01
- License: CC BY 4.0 (as shown on the World Bank indicator page)
- Files stored:
  - data/7.3.1_Canada_raw_worldbank_EG.EGY.PRIM.PP.KD_DS.xls (raw download)
  - clean_CA_energy_intensity_EG.EGY.PRIM.PP.KD.csv (cleaned, Canada-only, long format)

## Derived / Combined Dataset
- Method: merged Da:contentReference[oaicite:28]{index=28} in Excel Power Query
- File stored:
  - clean_CA_joined_renewables_intensity.csv
