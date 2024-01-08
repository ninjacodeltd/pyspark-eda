# Kaggle Dataset | NBA History | Seasonal Data 1995-2023
[source](https://www.kaggle.com/datasets/bendikfltaas/nba-history-seasonal-data-1995-2023)

## About the data
There are 7 parquet files in this dataset:

- `total.parq` is a parquet file containing regular season stat totals per player for each team for observed years 1995-2023
- `total_playoffs.parq` is a parquet file containing playoff stat totals per player and for each team for observed years 1995-2023
- `advanced.parq` is a parquet file containing regular seasonal advanced stats (re: VOIP) per player for each team for observed years 1995-2023
- `advanced_playoffs.parq` is a parquet file containing more playoff advanced stats (re: VOIP) per player for each team for observed years 1995-2023
- `average.parq` is a parquet file containing regular season stats averages per player for each team for observed years 1995-2023
- `average_playoffs.parq` is a parquet file containing playoff stat averages per player for each team for observed years 1995-2023
- `roster.parq` is a parquet file containing the roster per team for seasons 1995-2023

## Loading the data
If you are familiar with pandas, it is just as easy to read a parquet file as it is reading a standard csv file. The compression and space occupancy for parquet is however much lower!

You can load it by simply writing:
```
import pandas as pd
df= pd.read_parquet('total.parquet')
in a notebook.
```
All data is sourced and can be found at [basketball-reference.com](https://www.basketball-reference.com/)