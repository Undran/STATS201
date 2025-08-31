## Dataset: A multi-scale time-series dataset for machine learning in decarbonized energy grids

**Source:** This is the official dataset from the paper by Ospina, Juan, et al. "A multi-scale time-series dataset with benchmark for machine learning in decarbonized energy grids." *Scientific Data* 9.1 (2022): 359.

**Purpose:** The dataset is designed to benchmark machine learning tasks critical for the operation of decarbonized power grids. It provides data at three spatial scales (macro, micro, sub-micro) and includes time-series for load, generation, weather, and market operations. This allows researchers to develop and test models for forecasting, imputation, and anomaly detection on a realistic representation of a modern grid with high renewable penetration.

**Access:** The full dataset is hosted on Zenodo:
- **DOI:** [10.5281/zenodo.6524310](https://doi.org/10.5281/zenodo.6524310)
- **Total Size:** ~5.4 GB

The code in the parent directory's notebook will automatically download a specific sample file (`macroscale.csv.zip`) for demonstration purposes. This approach saves repository space and allows users to fetch only the data they need.

**Data Dictionary (Sample - Macroscale):**
| Variable Name          | Description                                           | Unit          | Scale       |
| ---------------------- | ----------------------------------------------------- | ------------- | ----------- |
| `timestamp`            | The timestamp of the observation (UTC).               | datetime      | All         |
| `load`                 | The total system electricity demand.                  | Megawatts (MW)| Macro       |
| `solar`                | Total solar power generation.                         | Megawatts (MW)| Macro       |
| `wind`                 | Total wind power generation.                          | Megawatts (MW)| Macro       |
|`wind_forecast`         | Day-ahead forecast for wind generation.               | Megawatts (MW)| Macro       |
| `temperature`          | Dry-bulb temperature at a key location.               | Degrees Celsius (°C) | Macro |
| `day_ahead_price`      | The day-ahead energy market price.                    | $/MWh         | Macro       |
