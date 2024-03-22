Dashboard link : 
# Car Sales Data Analysis

Background: Our company is a car dealership that sells various car models. To effectively track and analyse our sales performance, we need a comprehensive Car Sales Dashboard in Power BI. 

Objective: The objective of this project is to design and develop a dynamic and interactive Car Sales Dashboard using Power BI. The dashboard will visualize critical KPIs related to our car sales, helping us understand our sales performance over time and make data-driven decisions.

Problem Statement 1: KPI’s Requirement

The dashboard should provide real-time insights into key performance indicators (KPIs) related to our sales data. This will enable us to make informed decisions, monitor our progress, and identify trends and opportunities for growth.

1.	Sales Overview:
•	Year-to-Date (YTD) Total Sales
•	Month-to-Date (MTD) Total Sales
•	Year-over-Year (YOY) Growth in Total Sales
•	Difference between YTD Sales and Previous Year-to-Date (PTYD) Sales

2.	Average Price Analysis:
•	YTD Average Price
•	MTD Average Price
•	YOY Growth in Average Price
•	Difference between YTD Average Price and PTYD Average Price

3.	Cars Sold Metrics:
•	YTD Cars Sold
•	MTD Cars Sold
•	YOY Growth in Cars Sold
•	Difference between YTD Cars Sold and PTYD Cars Sold



Problem Statement 2: Charts Requirement

1.	YTD Sales Weekly Trend: Display a graph chart illustrating the weekly trend of YTD sales. The X-axis should represent weeks, and the Y-axis should show the total sales amount.
2.	YTD Total Sales by Body Style: Visualize the distribution of YTD total sales across different car body styles using a Pie chart.
3.	YTD Total Sales by Colour: Present the contribution of various car Colours to the YTD total sales through a pie chart.
4.	YTD Cars Sold by Dealer Region: Showcase the YTD sales data based on different dealer regions using a map chart to visualize the sales distribution geographically.
5.	Company-Wise Sales Trend in Grid Form: Provide a tabular grid that displays the sales trend for each company. The grid should showcase the company name along with their YTD sales figures.
6.	Details Grid Showing All Car Sales Information: Create a detailed grid that presents all relevant information for each car sale, including car model, body style, colour, sales amount, dealer region, date, etc

I divided this Project into three Tasks with subtasks each as follows:


Task1:

1.	Step 1: Load the Dataset given by the Company into Power BI Desktop
2.	Transformed data and Checked for Quality of Columns. Also checked for Data duplicates and errors and null data cells. Data Cleaning is done at this stage.
3.	Started creating Calendar_table to make dates(ddmmyyyy)  into Yearly, Monthly Weekly and date wise and attached to Car_data using Data Modelling.
4.	Create a Overview Dashboard and use textbox box to display.
5.	Now using New measure Dax functions we found YTD total sales, PYTD total sales, difference of YTD and PYTD total sales, YTD Growth Sales in percentage and MTD total sales all in one KPI Name Card Visual.
To find PYTD sales  using DAX- “pytd total sales = CALCULATE(SUM(car_data[Price ($)]),SAMEPERIODLASTYEAR('calendar table'[Date]))”.
6.	Similarly I created KPIs for YTD Average Price,  PYTD Avg Price,  Difference of YTD and PYTD average prices and also formulated for YTD Average Growth Price and MTD Average Price.
7.	Similarly, for YTD Cars Sold, PYTD Cars Sold and Difference of YTD and PYTD Cars Sold
YTD Cars Sold Growth and MTD Cars Sold.
By here task 1 completed the first requirement.


Task 2:

1.	Took the Graph chart visual so that I gave Week wise on X-axis and YTD Weekly Sales, Max Point YTD Weekly sales on Y-axis. Highlighted the maximum sales point in the graph.
2.	YTD Sales by Body Styles Using Donut chart where labelled by different styles of Car from Car_ data to show which Body style cars are having more sales in YTD
3.	YTD Sales by Colour Using Donut chart where labelled by different Colours of Cars from Car_ data to which colour cars are having more sales.
4.	YTD Cars Sold by Dealer Region is built using Filled Map by dropping Dealer_region from Car_data to Location and YTD Cars sold to Bubble Size to show region wise performance of cars sold.
5.	I have built Company Wise Sales Trends Performance matrix table to analyse the Total Sales, Average Price, Total Cars Sold and Growth of each company wise.
6.	Body style, Dealers, Transmission and Engine as slicers to know their statistics in Sales, Pricing and Growth.
Here the second requirement is completed.


Task 3:

1.	 To visualize the performance metrics, Company Sales, Dealer wise with repect to customers is produced in a Matrix Table so that we can understand the customers interest and forecast the growth in Cars sales.
2.	I have built a Detail Dashboard and synced slicers to optimise and filter in both dashboards. 
