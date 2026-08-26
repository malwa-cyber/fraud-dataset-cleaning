# finance-fraud-datacleaning
A finance fraud datacleaning/data analysis project
## description of the zip file
It is a zip file with different csv files, so I extracted the transaction csv file to start cleaning it
## objectives
1. To clean, validate and analyze the financial transaction data using Excel.
2. To identify transaction patterns, trends and potential areas of risks using Power BI.
3. To segment accounts by risk level.
4. To identify which features are most associated with fraud.
# cleaning
Now let's get started!!
## checking missing values
I started by assessing whether there are missing values using the countblank function (=countblank(A2:A50001)) which I applied in all columns and found out that there are 1000 missing values in the transaction date column... the date were also misformatted.
## checking for duplicates
I used the countif function (=countif($A$2:$A$50001,A2)>1). Applied this to all columns to check if there are any duplicates and found out that there are 1000 duplicates in the transaction ID column.

## handling duplicates
I used the conditional formatting and highlighted the duplicates and deleted them once I've confirmed that they are really duplicates.

## formatting the date-time column


## handling missing values
I used the conditional formatting approach to highlight the missing values on the date and used the data provided in the dataset to fill it. Using this formula (=IF(H3="", H2, H3)) suggesting that if H3 is missing, then replace it with the value in H2 if not H3 stands.
 
