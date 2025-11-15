# -Task-1-Data-Cleaning-and-Preprocessing

These Procedures are helps me to clean the Dataset:
1. Download any dataset from Kaggle.com. (My Choice (retail_store_sales))
2. After download the dataset make sure to take one copy of the dataset for the backup.
3. To algin the raw dataset use this shortcuts Keys
4. (ctrl+A)-for selecting whole data,
5. (Alt+H+O+I)-for fix the column width,
6. (Alt+H+O+A)-for adjust the row height,
7. (Alt+H+A+C)-for center algin everything,
8. (ctrl+T)-for format it as a table,
9. (ctrl+shift+Down arrow)-for select all the rows.
10. Go to Home tab -> Conditional formatting -> Highlight cell rules -> Duplicate value (Using this to identify the Duplicates value)(There is No Duplicates in Trascation ID).
11. Go to Home tab -> Conditional formatting -> New rule -> Format only cells that contain -> Blank -> Format only -> Fill -> Colour (To identify the Blank cells in whole table).
12. To fill the missing values in (Price Per Unit) so use Formula to calculate (=[@[Total Spend]]/[@Quantity]).
13. Discounted amount column not in the dataset so,missing values of (Discount Applied column) is treated as a (FALSE) by default. Use Find & Replace option to replace the missing values into (FALSE) in the (Discount Applied) column.
14. With the help of ChatGPT fill the missing values in (Item column) used this prompt (Fill the missing values from the CSV file and give me the completed clean file) to fill the (Item) column.
15. Find the average of each catogery to fill the missing values of (Quantity) & (Total Spend) columns.
16. Category           -     Average     -       Around
17. Beverage           -      5.58       -         6
18. Butcher            -      5.48       -         5
19. Computer & Electric Ass - 5.60       -         6
20. Electric Household Ess  - 5.48       -         5
21. Food               -      5.56       -         6
22. Furniture          -      5.54       -         6
23. Milk Products      -      5.51       -         6
24. Passterie          -      5.51       -         6
25. Finally find out the averages for each category in (Quantity) column, use filter to categorize the table then Find & Replace option to replace the missing values into (Arounded Values) in the (Quantity) column.
26. After filling the missing values of (Quantity) column.
27. use this formula (=[@[Price Per Unit]]*[@Quantity]) to fill the (Total Spend) column.
28. Now the Dataset was cleaned.
