# Veda Technology Internship
Short Write-up: Data Cleaning and Preprocessing - Superstore Dataset 
During the initial assessment of the Superstore dataset (9994 rows, 21 columns), several data 
quality issues were identified. Using Excel tools like Go To Special for blanks and Conditional 
Formatting for duplicates, the following issues were found:  
(1) Inconsistent text formatting in City and State columns with extra spaces and mixed cases, 
(2) Inconsistent date formats in Order Date and Ship Date, 
(3) 11 blank values in Postal Code, and  
(4) 3 duplicate rows based on Row ID.  
(5) Sales and Profit were stored as text. 
To resolve these, TRIM and PROPER functions were used to standardize text, Text to Columns 
was used to unify date format to DD/MM/YYYY and convert text numbers to numeric format. 
Blank Postal Codes were filled by mapping the correct code for that City, and true duplicate 
rows (where Row ID was duplicated) were removed using the Remove Duplicates tool by 
selecting only the Row ID column. Order ID and Customer ID duplicates were retained as they 
represent repeat purchases, not data errors. After cleaning, re-validation confirmed 0 blanks 
and 0 duplicate Row IDs, making the dataset ready for analysis.
