# AdventureWorks-Sales-Data
Dashboard to visualize sales data for one of example cycles company to keeps track of their product sales, bussiness, revenues based on geolocations and products/categories and subcategories. Restructure the dataset using Calculated columns and measures also build relationships between models to showcase combined results from multiple sources.

Problem Statement:
Creating the Dynamically interactive dashboard using Sales Data from Year 2015 to 2017
Dashboard should contain following aspects:
1) Total Orders by Category/Subcategory/Products
2) Need to Total orders by each product name and their return rates
3) Monthly Revenue/Monthly Orders/Monthly Returns
4) Top Product Name based on Total Returns
5) Top Product Name based on Total Profit
6) Map visualization based on Country


**Planning Phase:**
Adventure Works Shared CSV file which includes Sales data Between 2015-2017, Returns, Customers,Territory etc

Data Cleaning and Structuring Data 
1) Verify data should not contains any invalid values or nulls or duplicates.
2) Verify Data type mapped corectly after transforming these CSV files and also verify valid table name.
3) For Sales Related CSV files (We received 3 Sales CSV files) use folder structure to Merge these files together.
4) Create a single Calander File which includes dates between 2015 to 2017 and Add additional fields like Start of Week, Month, Year, Week day, Week end etc.

**Modeling Phase:**
1) Identify Dimentions tables and fact tables
2) Identify relationships between columns
3) Connect required feilds, Avois two way data flows and Use "snowflake schema" when we do not have proper common fields between tables
4) Disable the foreign key or Fact table reference keys from report view, this helps to avoid scenarios where customer selecting misleading columns from Report View
![image](https://user-images.githubusercontent.com/38867261/133906455-0c17f0c0-95f2-462b-9ce1-4687cf505419.png)

Addition Measures and Calculated columns
This is one of core where we try to analyze what needs to be displayed on Report View
1) Always use Measure in order to create functionalities like Total Returns, Total Revenue, Total Profit etc
2) Focus more on Explicit measure and try to avoid Implicit measures 
3) Use DAX fomulas in order to create measures and calculated columns

Reporting Phase:
After creating required fields to display the data insights now roll up sleeves and jump to most fun part
Verify problem statements again, try to draw rough figure of dashboards try to connect dots as much as possible
When you finalize your dashboard try to replicate on report tab 
Focus more on What our clients want and how can we give most informative, effective data insight

Here is what i come up with data visualization based on problem statement provided.
![image](https://user-images.githubusercontent.com/38867261/133906743-a9984a9a-54ac-42c5-876c-02a797f6e472.png)

Features:
1) Able to View Sales based on Product name/Subcategory name/category name
2) Selecting Date range helps to analyze the sales occured on specific time period
3) KPI cards with trend axis helps to idetify upward and downward trends of the sales
4) Top Product based on sales and top product based on profit based on filter selected by user
5) Map visualization provides total orders based on country

Also included "Drill-Through" option when user wants to see trend based on Specific Product name/Subcategory name/category name
![image](https://user-images.githubusercontent.com/38867261/133906896-5df6932b-f983-45db-b643-4fd8531ba6c9.png)
This visualization gives Monthly orders/Revenue/Returns with Target value that needs to achieved on gauge charts
Providing Forecast of next future 6 weeks sales will give rough idea on for that respective product how sales can behave



