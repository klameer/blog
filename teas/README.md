## Analysis of Sri Lanka Tea Data Sets

#### To Facilitate Business Intelligence and Look for Patterns in the Data
[TOC]

# Project Tea Data Set Analysis
## Business Case
1. Exploratory analysis of tea auction and export data to get more business intelligence about the process. 
2.  Compare rainfall data with tea auction data to consider a correlation between the two. 

## Objectives for Tea Auction and Export Data
 - How does ESWARAN BROTHERS compare against other buyers by size and mix of purchases?
 - Are ESWARAN BROTHERS purchasing efficiently for their purchasing profile?
 - Are there any trends that can be discerned from the data?
 - How does ESWARAN BROTHERS compare against other exports by size and mix of purchases? This will only be done for teabags.
 - Country analysis. Who are the biggest purchases?
 - How do countries purchasing prices differ from each other?

# Analysis
## Correlation Between Lot Size and Price
![Alt](https://raw.githubusercontent.com/klameer/blog/master/teas/img_lotsize_price_correlation.png)

## Mix Comparison
ESWARAN BROTHERS EXPORTS (PVT) LTD | Everyone Else
---- | ----
0.097 | 0.46
0.24 | 0.31
0.66 | 0.22

![Alt](https://raw.githubusercontent.com/klameer/blog/master/teas/img_grade_mix.png)

## Buy Trend
Is ESWARAN BROTHERS buying efficiently  

ESWARAN BROTHERS | Everyone Else
---- | ----
0.22 | 0.016
0.17 | 0.019
0.12 | 0.0045
0.09 | 0.041
0.086 | 0.016
0.055 | 0.073
0.054 | 0.066
0.052 | 0.026
0.048 | 0.012
0.024 | 0.071

![Alt](https://raw.githubusercontent.com/klameer/blog/master/teas/img_buy_trend.png)

## Exports

In the dataset there is a difference in magnitude between the first and second half of the year. 

![Alt](https://raw.githubusercontent.com/klameer/blog/master/teas/img_exports_over_year.png)


![Alt](https://raw.githubusercontent.com/klameer/blog/master/teas/img_exports_by_continent.png)

Continent Breakup over year. Can break these down into individual continents.
![Alt](https://raw.githubusercontent.com/klameer/blog/master/teas/img_continent_breakup_over_year.png)

# Data Set Info
## Tea Auction Data
Assumptions
 - Selling price of a lot is QTY sales * QTY saled price

Source File
 - Saved as xlsx from xlsb as this is not accepted by Pandas

Data
 - Removed Qty Sales and Price of 0. These are unsuccessful auctions and zero values will skew analysis. 

Added Fields
 - Sales Value by combing Sales Quantity by Price
 - Bucketed quantities into 5 to consider a relationship between lot size and price


# Changes Done to the Data
### Tea Auction Data


# Glossary

### Tea Auction Data
Broker - Responsible for organising the auction transaction.  
Lot Number - Action item count. Resets every month.  
Week Number - Week of year.  
Date - Date of Transaction.  
Estate - Where the tea was produced.  
Grade - Grade of Tea.  
QTY Production - ???  
Price - ???  
QTY sales - Quantity of sold lot.  
QTY saled price - Final Price.  
Company - Company who purchased lot.  
Year - Year of transaction. Derived from Date.  
Corrected Estate - Derived from Estate. Used in Analysis.  
Corrected Company - Derived from Company. Used in Analysis.  

### 
