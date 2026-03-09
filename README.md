# Power-BI-From-Data-Cleaning-to-DAX-Insights
Laboratory Work 2 - End-to-End Data Analytics in Power BI: From Data Cleaning to DAX Insights

# PDF Documentation
https://drive.google.com/file/d/1UXd5wrSNzSaU33OF96Htz7JpFOXhCvRf/view?usp=sharing<br><br>

Part 1: Open Power Query Editor<br><br>

1. Open Power BI Desktop.<br>
<img width="1914" height="1024" alt="image" src="https://github.com/user-attachments/assets/cfcea287-1ba2-4ae6-b86a-8939de4e8294" /><br><br>

2. Click Home → Get Data → Excel Workbook.<br>
<img width="787" height="754" alt="image" src="https://github.com/user-attachments/assets/e5cedda0-d2d8-4472-afe8-0bcc05f0b152" /><br><br>

3. Select Messy_Sales_Data.xlsx.<br>
<img width="1013" height="626" alt="image" src="https://github.com/user-attachments/assets/b700fcb6-e4e9-4893-8d97-8136472fc2e4" /><br><br>

4. Click Transform Data to open Power Query Editor.<br>
<img width="1210" height="977" alt="image" src="https://github.com/user-attachments/assets/c12843fd-7e6d-490c-bdf2-7ef780ba96aa" /><br><br>

Part 2: Remove Duplicates<br><br>

1. Select the table.<br>
<img width="295" height="739" alt="image" src="https://github.com/user-attachments/assets/5cabe271-26f2-4be8-838e-c74d801989d6" /><br><br>

2. Highlight the column(s) that should be unique (e.g., OrderID).<br>
<img width="295" height="739" alt="image" src="https://github.com/user-attachments/assets/8431286f-e0ca-458f-9c97-e7bdf6ed34f2" /><br><br>

3. Click Home → Remove Rows → Remove Duplicates.<br>
<img width="1919" height="988" alt="image" src="https://github.com/user-attachments/assets/aa287b0c-4a48-405d-8cf1-75156b453e1d" /><br><br>

Part 3: Handle Missing Values<br><br>

1. Identify columns with null values.<br>
<img width="1392" height="810" alt="image" src="https://github.com/user-attachments/assets/a8fe4c43-6fd2-44f5-a5d7-b0486b0398ee" /><br><br>

2. Apply appropriate action:<br><br>

○ Replace with 0 → Transform → Replace Values<br>
<img width="1070" height="580" alt="image" src="https://github.com/user-attachments/assets/de2267c9-d4cc-48dc-998d-84d893f81097" /><br><br>

○ Remove rows → Remove Rows → Remove Blank Rows<br>
<img width="1919" height="950" alt="image" src="https://github.com/user-attachments/assets/589d4d38-45e4-47f9-b6e4-64f22d4532d3" /><br><br>

○ Fill down → Transform → Fill → Down<br>
<img width="1400" height="358" alt="image" src="https://github.com/user-attachments/assets/394c4c5c-c608-4b43-b10d-ae1aa1430542" /><br><br>

Part 4: Change Data Types<br><br>

1. Check icons beside column names.<br>
<img width="69" height="85" alt="image" src="https://github.com/user-attachments/assets/7c8483d7-17b6-44f2-a02a-b9e7357b6c4e" /><br><br>
  
2. Set correct types:<br>
○ Date → Date type<br>
<img width="454" height="445" alt="image" src="https://github.com/user-attachments/assets/54a2245e-aff6-421f-85f3-96fc5c935662" /><br><br>

○ Sales → Decimal Number<br>
<img width="323" height="450" alt="image" src="https://github.com/user-attachments/assets/0b9ba608-af50-4203-af0b-500df353ef4c" /><br><br>

○ Quantity → Whole Number<br>
<img width="285" height="457" alt="image" src="https://github.com/user-attachments/assets/aa4d4fa2-2b18-4cf8-a859-f7e278ebd901" /><br><br>

Part 5: Rename Columns Properly<br><br>

1. Double-click column names.<br>
2. Use standard naming:<br>
○ order_id<br>
<img width="229" height="128" alt="image" src="https://github.com/user-attachments/assets/eada01f3-1d79-42f0-9bc3-6dd19541916e" /><br><br>

○ order_date<br>
<img width="267" height="122" alt="image" src="https://github.com/user-attachments/assets/33f2e20f-e5cf-4ab7-a325-4b614468f5fe" /><br><br>

○ customer_name<br>
<img width="219" height="131" alt="image" src="https://github.com/user-attachments/assets/7117fbac-9300-436e-a9fe-a7f18cb919bc" /><br><br>

○ total_sales<br>
<img width="243" height="71" alt="image" src="https://github.com/user-attachments/assets/98d250c5-298f-461c-b392-9259d7959169" /><br><br>

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

  ● Compare dataset size before and after cleaning.<br>
  Before cleaning the dataset:<br>
<img width="492" height="25" alt="image" src="https://github.com/user-attachments/assets/6dfcffc2-0cc3-4ff7-b328-238a9160fa8d" /><br><bR>

After cleaning the dataset:<br>
<img width="459" height="22" alt="image" src="https://github.com/user-attachments/assets/8cb1be82-2a9d-4c6e-857c-ab9b48f03020" /><br><br>

● Research: What is ETL and how does Power Query support it?<br>
- **ETL** stands for **Extract, Transform, and Load**, a process used to prepare data for analysis. **Extract** means collecting data from different sources such as Excel files, databases, websites, or CSV files. **Transform** involves cleaning and modifying the data by removing duplicates, filtering rows, changing data types, merging tables, or splitting columns. **Load** is the final step where the processed data is placed into a system like Excel tables, dashboards, or databases. **Power Query** supports ETL by allowing users to import data from various sources, clean and transform it using built-in tools, and load the prepared data into Excel or Power BI. It also records each step automatically so the same process can be repeated when new data is added.<br><br>

# Merge and Append Queries

Part 1: Load Data<br>
<img width="1909" height="769" alt="image" src="https://github.com/user-attachments/assets/dd7b6d53-d9bf-45d8-bc4f-d5b34974e1ce" /><br>
<img width="1919" height="780" alt="image" src="https://github.com/user-attachments/assets/c4b4241c-fc00-4fbc-9bef-c9282c4bb2e2" /><br><br>


Part 2: Merge Datasets (Inner Join)<br>
<img width="1689" height="777" alt="image" src="https://github.com/user-attachments/assets/3de5e8a0-1511-4391-913d-1d6f208b7acd" /><br><br>

Part 3: Append Monthly Sales Files<br>
<img width="1919" height="783" alt="image" src="https://github.com/user-attachments/assets/9b5a0d33-c6cc-4dda-8b9f-9b0820db6886" /><br><br>

Part 4: Validate Merged Data<br><br>

● Check row counts.
<img width="435" height="21" alt="image" src="https://github.com/user-attachments/assets/37e91543-b702-4c47-8af6-7bc0669a989e" /><br><br>
<img width="459" height="31" alt="image" src="https://github.com/user-attachments/assets/0802f869-69bd-48f1-8ebd-111f2865a3a8" /><br><br>

● Verify no unexpected null values.<br>
<img width="432" height="737" alt="image" src="https://github.com/user-attachments/assets/2b72b6f6-9ba3-4418-aabb-df051af9e622" /><br><br>

● Confirm matching customer details.<br>
<img width="1348" height="445" alt="image" src="https://github.com/user-attachments/assets/241d4cab-451a-43a9-84ff-88a13a24ed40" /><br><br>


# Guide Questions
1. What is the difference between Merge and Append?<br>
- Merge and Append are both used to combine data, but they work in different ways. Merge combines two tables by matching a common column (like CustomerID), similar to how a database join works. It adds related columns from one table to another. On the other hand, Append simply stacks tables on top of each other, adding more rows to a single table as long as the columns are similar.<br><br>

2. Why use Inner Join instead of Left Join?
- An Inner Join is used when you only want records that exist in both tables. This helps ensure that the data is complete and matching. It removes records that do not have a match, which can help avoid incorrect or incomplete information in the final dataset.<br><br>

3. What happens to unmatched records in an Inner Join?
- When using an Inner Join, any records that do not have a match in the other table are excluded from the result. Only the rows with matching values in both tables will appear in the merged dataset.<br><br>

4. When is Append more appropriate than Merge?
- Append is more appropriate when you want to combine datasets with the same structure by adding more rows. For example, if you have sales data from January, February, and March, you can append them together to create one complete dataset for the whole period.<br><br>

# Enhancement Activities
● Try Left Join and compare results.<br>
<img width="1919" height="781" alt="image" src="https://github.com/user-attachments/assets/282bf482-67b5-4ed4-9aad-c2a3f10f4eba" /><br><br>

● Identify unmatched records.
<img width="1362" height="758" alt="image" src="https://github.com/user-attachments/assets/be552937-55b6-4764-b02e-ea09ba3beedf" /><br><br>

● Create a diagram showing join types.
<img width="1260" height="1003" alt="image" src="https://github.com/user-attachments/assets/c0661b4d-e690-421d-9cf1-3bed08c64e4c" />


