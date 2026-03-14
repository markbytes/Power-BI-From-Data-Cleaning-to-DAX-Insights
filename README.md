# Power-BI-From-Data-Cleaning-to-DAX-Insights
Laboratory Work 2 - End-to-End Data Analytics in Power BI: From Data Cleaning to DAX Insights

# PDF Documentation
https://drive.google.com/file/d/1UXd5wrSNzSaU33OF96Htz7JpFOXhCvRf/view?usp=sharing<br><br>

Guide Questions<br><br>

1. Why is removing duplicates important in data analysis?<br>
- Removing duplicates is important because repeated records can make the data inaccurate. For example, if a sales transaction appears more than once, it can make the total sales look higher than they actually are. By removing duplicates, we make sure the data is clean and the results of the analysis are more reliable.<br><br>

2. What problems can missing values cause in reports?<br>
- Missing values can lead to incomplete or misleading reports. When important information like sales amount or quantity is missing, calculations such as totals or averages may not be correct. It can also cause errors in charts or formulas, which affects how the data is interpreted.<br><br>

3. How does correct data typing affect calculations?<br>
- Correct data typing helps ensure that calculations work properly. For example, sales should be stored as numbers so they can be added or averaged, and dates should be set as date types so they can be sorted or filtered by month or year. If the data type is wrong, calculations may not work or may produce incorrect results.<br><br>

4. What naming conventions improve data readability?<br>
- Using clear and consistent names makes data easier to understand. Column names should be simple, descriptive, and consistent, such as OrderDate, CustomerName, or SalesAmount. Avoiding confusing abbreviations and keeping the format consistent helps anyone reading the dataset understand it more easily.<br><br>

# Enhancement Activities
● Create a data quality checklist for future datasets.<br>
- Ensure there are no missing values in important fields.<br>
- Verify that data values are correct and realistic.<br>
- Data format should be the same (e.g., date format, capitalization).	<br>
- Remove repeated records in the dataset.	<br>
- Columns should have the correct type (number, text, date).<br>	
- Values should fall within acceptable limits.<br>	
- Categories should be uniform.<br>
- Remove leading or trailing spaces in text fields.<br><br>

● Research: What is ETL and how does Power Query support it?<br>
- **ETL** stands for **Extract, Transform, and Load**, a process used to prepare data for analysis. **Extract** means collecting data from different sources such as Excel files, databases, websites, or CSV files. **Transform** involves cleaning and modifying the data by removing duplicates, filtering rows, changing data types, merging tables, or splitting columns. **Load** is the final step where the processed data is placed into a system like Excel tables, dashboards, or databases. **Power Query** supports ETL by allowing users to import data from various sources, clean and transform it using built-in tools, and load the prepared data into Excel or Power BI. It also records each step automatically so the same process can be repeated when new data is added.<br><br>

# Guide Questions
1. What is the difference between Merge and Append?<br>
- Merge and Append are both used to combine data, but they work in different ways. Merge combines two tables by matching a common column (like CustomerID), similar to how a database join works. It adds related columns from one table to another. On the other hand, Append simply stacks tables on top of each other, adding more rows to a single table as long as the columns are similar.<br><br>

2. Why use Inner Join instead of Left Join?
- An Inner Join is used when you only want records that exist in both tables. This helps ensure that the data is complete and matching. It removes records that do not have a match, which can help avoid incorrect or incomplete information in the final dataset.<br><br>

3. What happens to unmatched records in an Inner Join?
- When using an Inner Join, any records that do not have a match in the other table are excluded from the result. Only the rows with matching values in both tables will appear in the merged dataset.<br><br>

4. When is Append more appropriate than Merge?
- Append is more appropriate when you want to combine datasets with the same structure by adding more rows. For example, if you have sales data from January, February, and March, you can append them together to create one complete dataset for the whole period.<br><br>

