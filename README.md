# Existing Home Sales vs 10-Year Treasury Yield Plot

## Overview
This repository provides a Python script to plot U.S. existing home sales against the 10-year Treasury yield. The plot includes:
- Dual y-axes (sales and yield)
- Recession shading (2001, 2007-2009, 2020)
- Customized axis limits and ticks

## Requirements
- Python 3.7+
- pandas
- matplotlib

You can install dependencies with:
```bash
pip install pandas matplotlib
```

## Data
Place your data file at `data/merged_df.csv`. It must include columns:
- `date` (YYYY-MM-DD)
- `Actual` (existing home sales in millions)
- `yield` (10-year Treasury yield in %)

## Usage
Run the plotting script with:
```bash
python plot_sales_yield.py \
  --input data/merged_df.csv \
  --output output/
```

Generated files:
- `output/existing_sales_yield.png`
- `output/existing_sales_yield.svg`

## Recessions
Shading marks NBER recession periods:
- Mar 2001 to Nov 2001
- Dec 2007 to Jun 2009
- Feb 2020 to Apr 2020

## License
This project is released under the MIT License.

