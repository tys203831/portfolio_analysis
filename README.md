# Build a Tearsheet for your portfolio within 10 lines of code

## Overview
This portfolio tearsheet is mainly generated using 2 libraries, `openbb` and `quantstats`

- Used `openbb.portfolio.load` to load my transactions data from excel file: [portfolio_data.xlsx](./input/portfolio_data.xlsx) and then calculate my portfolio return
- Used `quantstats.reports.html` to generate a tearsheet for my portfolio. See the output here: [Portfolio tearsheet](./quantstats-tearsheet.html)

So, if you want to reuse this template, just merely change this two input:

1. data inside excel file [here](./input/portfolio_data.xlsx):

![image](./image/portfolio_data.png)

2. benchmark symbol you want to compare with

But, take note that the data source is from Yahoo Finance, so when you want to change the stock ticker in excel file, please refer that ticker symbol in Yahoo Finance.

![image](./image/quantstats-tearsheet.png "Quantstats")


## How to run this code
Make sure you have python installed in your computer

In your terminal, run the code as below
1. `pip install pandas openbb quanstats`
2. `python -m analysis`
