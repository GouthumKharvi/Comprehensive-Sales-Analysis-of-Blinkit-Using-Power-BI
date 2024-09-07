# BlinkiIt Analaysis 

### This project is aimed at performing a comprehensive sales analysis of Blinkit, focusing on identifying key insights and opportunities for optimization in sales performance, customer satisfaction, and inventory management. By leveraging Power BI, the project utilizes various KPIs and visualizations to provide a clear understanding of the business dynamics.

## STPES IN PROJECTS 

- Identify Business Requirements and Gather Data Needs
- Review and Explore Data
- Connect to Data Sources
- Clean and Validate Data for Accuracy
- Build Data Models
- Process and Manipulate Data
- Apply DAX Formulas for Data Analysis
- Plan and Structure the Dashboard Layout
- Create and Format Visual Elements
- Develop Dashboards and Reports
- Extract and Present Insights

## Business Requirement:

The objective is to thoroughly analyze Blinkit's sales metrics, customer satisfaction, and inventory allocation to identify critical insights and areas for improvement. This will be achieved by utilizing various key performance indicators (KPIs) and visual tools in Power BI.

### KPI Objectives:

1.	**Total Sales:** Assess the total revenue generated from all products sold.
2.	**Average Sales:** Compute the average income per sale.
3.	**Number of Items:** Track the total number of distinct products sold.
4.	**Average Rating:** Evaluate the overall customer feedback rating for the products sold.
   
**These KPIs are essential for evaluating the business performance and identifying potential enhancements.**



## Charts Needed:
**1. Impact of Fat Content on Total Sales:**
   - **Goal:** To assess how different levels of fat content influence total sales.
     
   - **Additional KPIs to Consider:** Look into how metrics like Average Sales, Number of Items, and Average Ratings vary with fat content.
     
   - **Recommended Chart Type: Donut Chart.**
     




      ![Screenshot 2024-09-07 034951](https://github.com/user-attachments/assets/71d707d4-99d0-4a9c-91fc-fcf80a9ca412)





     
**2. Sales Analysis by Item Type:**
   - **Goal:** To evaluate the sales performance of various item types.
   
   - **Additional KPIs to Consider:** Examine other metrics such as Average Sales, Number of Items Sold, and Average Ratings across different item types.
     
   - **Recommended Chart Type:**  Bar Chart.


      ![Screenshot 2024-09-07 035631](https://github.com/user-attachments/assets/4cd41dca-3520-4abc-94b4-c910dee0fb76)




**3. Outlet Comparison of Fat Content in Relation to Total Sales:**
   - **Goal:** To compare total sales across different outlets categorized by fat content.
 
   - **Additional KPIs to Consider:** Investigate how Average Sales, Number of Items, and Average Ratings change with fat content across outlets.
    
   - **Recommended Chart Type:** Stacked Column Chart.

      ![Screenshot 2024-09-07 035814](https://github.com/user-attachments/assets/f569ebd2-41d6-488a-af5d-e832f2c9335b)


     
**4. Total Sales by Outlet Characteristics:**
   - **Goal:** To explore how the establishment’s type or age affects total sales.
 
   - **Recommended Chart Type:** Line Chart.

   ![Screenshot 2024-09-07 040247](https://github.com/user-attachments/assets/8f6ea65b-026b-447d-8df2-3098ebc33c5b)


     
**5. Total Sales Based on Outlet Size:**
   - **Goal:** Investigate the relationship between the size of the outlet and the total sales figures.
    
   - **Recommended Chart Type:** Donut or Pie Chart.


      ![Screenshot 2024-09-07 040316](https://github.com/user-attachments/assets/ead30267-ecfe-43a2-b7e6-97f75cedc9f8)

 
**6. Sales Distribution by Location:**
   - **Goal:** Evaluate how sales are geographically distributed across various locations.
    
   - **Recommended Chart Type:** Funnel Map.

      ![Screenshot 2024-09-07 040346](https://github.com/user-attachments/assets/3aa66454-329d-40c9-afda-8c62448300c8)

      
 
**7. Comprehensive Metrics Overview by Outlet Type:**
   - **Goal:** Display a detailed breakdown of all key metrics (including Total Sales, Average Sales, Number of Items Sold, and Average Ratings) segmented by different outlet types.
    
   - **Recommended Chart Type:** Matrix Card.


![Screenshot 2024-09-07 040800](https://github.com/user-attachments/assets/7ab0094b-e342-4f20-998e-b53f3d9168b4)



### Steps for Creating the Blinkit Sales Analysis Dashboard in Power BI

1. **Identify Business Requirements and Gather Data Needs**
   - Start by understanding the business requirements, focusing on sales performance, customer satisfaction, and inventory management.
    
   - Review which key metrics you need: total sales, average sales, number of items sold, and customer ratings.
    
   - Determine what data sources are available, such as sales transactions, inventory levels, and customer feedback.

2. **Review and Explore Data**
   - After gathering the data, explore it in Excel or SQL to understand its structure. Identify key fields such as product names, sales numbers, outlet details, and customer ratings.
    
   - Look for missing data or anomalies and make a plan to clean and transform it in Power BI.

3. **Connect to Data Sources**
   - Open Power BI Desktop, and from the **Home** tab, select **Get Data**.
    
   - Connect to your data source (Excel, SQL, etc.). For this project, you’ll be pulling data like sales numbers, outlet information, and product details.

4. **Clean and Validate Data for Accuracy**
   - Once your data is imported, open **Power Query Editor** to clean it.
     
   - Remove duplicates, fix any data types (e.g., converting text to numbers for sales), and filter out any irrelevant data.
     
   - If there’s missing information, you can replace null values with an average or median, depending on the requirement.
   
5. **Build Data Models**
   - Once the data is clean, define relationships between tables in the **Model** view.
     
   - Ensure relationships are set between sales transactions and outlets, products, and customers.
     
   - For example, a **one-to-many** relationship between the outlets and sales tables allows you to aggregate sales by outlet.

6. **Process and Manipulate Data**
   - Create calculated columns and measures using DAX. For example:
     
     - **Total Sales**: `Total Sales = SUM(Sales[Amount])`
       
     - **Average Sales**: `Average Sales = AVERAGE(Sales[Amount])`
       
     - **Number of Items Sold**: `Number of Items = COUNT(Sales[Item_ID])`
       
     - **Average Rating**: `Average Rating = AVERAGE(Reviews[Rating])`
    
     

7. **Plan and Structure the Dashboard Layout**
   - Start by sketching out a wireframe of your dashboard. Think about where each chart will go and how users will interact with it.
     
   - Typically, place key performance indicators (KPIs) at the top, followed by a grid layout for your charts.

8. **Create and Format Visual Elements**
   - Insert your first chart (for example, a **Donut Chart** for the impact of fat content on total sales). Use **Fat Content** on the legend and **Total Sales** in the value field.
     
   - Add conditional formatting for data labels if needed.

9. **Develop Dashboards and Reports**

   #### A. **Create Each Chart**:
   
   - **Impact of Fat Content on Total Sales**: 
     - Use a **Donut Chart**.
       
     - Add **Fat Content** to the legend, and **Total Sales** to values.
       
     - Apply KPIs like Average Sales and Ratings if relevant.
    
      ![Screenshot 2024-09-07 034951](https://github.com/user-attachments/assets/71d707d4-99d0-4a9c-91fc-fcf80a9ca412)
   
   - **Sales Analysis by Item Type**:
     - Insert a **Bar Chart**.
       
     - Add **Item Type** to the axis and **Total Sales** to values. Add **Average Sales** as a secondary metric if needed.


     ![Screenshot 2024-09-07 035631](https://github.com/user-attachments/assets/4cd41dca-3520-4abc-94b4-c910dee0fb76)

     
   
   - **Outlet Comparison of Fat Content in Relation to Total Sales**:
     - Use a **Stacked Column Chart**.
    

     ![Screenshot 2024-09-07 035814](https://github.com/user-attachments/assets/f569ebd2-41d6-488a-af5d-e832f2c9335b)
  
     
       
     - Place **Outlets** on the x-axis and **Fat Content** on the legend. Add **Total Sales** as the main value.
   
   - **Total Sales by Outlet Characteristics**:
     - Use a **Line Chart** to map sales based on outlet types or outlet age.

      ![Screenshot 2024-09-07 040247](https://github.com/user-attachments/assets/8f6ea65b-026b-447d-8df2-3098ebc33c5b)


   - **Total Sales Based on Outlet Size**:
     - Add a **Donut or Pie Chart** to visualize the relationship between outlet size and sales.
    
       
      ![Screenshot 2024-09-07 040316](https://github.com/user-attachments/assets/ead30267-ecfe-43a2-b7e6-97f75cedc9f8)
     
   
   - **Sales Distribution by Location**:
     - Use a **Funnel Map** to display sales geographically. Assign locations to the map and **Total Sales** as values.
  
       
     ![Screenshot 2024-09-07 040346](https://github.com/user-attachments/assets/3aa66454-329d-40c9-afda-8c62448300c8)
     
   
   - **Comprehensive Metrics Overview by Outlet Type**:
     - Use a **Matrix Visual** to show detailed metrics like **Total Sales**, **Average Sales**, **Number of Items Sold**, and **Average Ratings**, all broken down by **Outlet Type**.
      
     ![Screenshot 2024-09-07 040800](https://github.com/user-attachments/assets/7ab0094b-e342-4f20-998e-b53f3d9168b4)


9. **Apply DAX Formulas for Data Analysis**

     ## What is DAX?

**DAX (Data Analysis Expressions)** is a formula language used in Power BI, Excel, and SQL Server Analysis Services to create calculations, aggregate data, and work with relational data models. It allows users to define custom calculations and manipulate data dynamically, making it essential for building advanced data models and dashboards in Power BI.

### Use of DAX:
DAX is used to:
- Create **calculated columns** and **measures** to analyze data dynamically.
- Aggregate, filter, and perform calculations on data across tables.
- Enable complex data analysis by performing tasks like summing, averaging, counting, and creating ratios or percentages.

### Explanation of DAX Expressions:

#### 1. **Total Sales:**

```DAX
Total Sales = SUM(Sales[Amount])
```
- **What it does:** This formula sums the values in the Amount column from the Sales table.
  
- **Purpose:** To calculate the total sales for all items sold, based on the individual amounts of each sale.

- **Use case:** You can use this measure to show overall sales figures in a card visual or aggregate sales in charts.


#### 2. **Average Sales:**

```DAX
Average Sales = AVERAGE(Sales[Amount])
```

- **What it does:**  This calculates the average value in the Amount column from the Sales table.
- **Purpose:** To find the average sale value across all transactions.
- **Use case:** It’s useful for understanding how much revenue, on average, each transaction brings in. You can display this value in reports to assess overall                    sales performance.

  
#### 3. Number of Items Sold:

```DAX
Number of Items = COUNT(Sales[Item_ID])
```

- **What it does:** This formula counts the number of non-blank entries in the Item_ID column of the Sales table.
- **Purpose:** To count the total number of items sold (each represented by an Item_ID).
- **Use case:** You can use this measure to show how many distinct products or transactions took place during the analysis period.

#### 4. Average Rating:

```DAX
Average Rating = AVERAGE(Reviews[Rating])
```

- **What it does:** This calculates the average of the Rating values from the Reviews table.
- **Purpose:** To compute the average customer rating for the products or services.
- **Use case:** Useful for assessing overall customer satisfaction. You can display it in a dashboard to provide insights into the quality of customer feedback.



## Creating DAX Expressions:
**To create these DAX formulas in Power BI:**

- **Open Power BI.**
- **Navigate to the “Modeling” tab in the ribbon.**
- **Choose “New Measure” or “New Column”, depending on whether you are creating a calculated measure or column.**
- **In the formula bar, enter the DAX expression (e.g., Total Sales = SUM(Sales[Amount])).**
- **Once created, you can use these measures in visualizations like cards, charts, or tables.**

  
**These DAX expressions help summarize and analyze your data dynamically in Power BI, allowing you to gain key insights from your data model.**


# Creating Metrics in Power BI

## Title: How to Create Metrics in Power BI

### What are Metrics?

In Power BI, **metrics** are key performance indicators (KPIs) that help track and evaluate the success of specific business activities. They allow users to monitor data trends and make informed business decisions. Metrics can be defined using **measures** or **calculated columns** created with **DAX** formulas.

The following example creates a set of important metrics for analyzing BlinkIT’s Grocery Data, including Total Sales, Average Sales, Number of Items Sold, and Average Rating.



### Example Metrics in Power BI:

```DAX
Metrics = {
    ("Total Sales", NAMEOF('BlinkIT Grocery Data'[Total Sales]), 0),
    ("Avg Sales", NAMEOF('BlinkIT Grocery Data'[Avg Sales]), 1),
    ("No of Items", NAMEOF('BlinkIT Grocery Data'[No of Items]), 2),
    ("Avg Rating", NAMEOF('BlinkIT Grocery Data'[Avg Rating]), 3)
}
```



10. **Extract and Present Insights**
    - Finalize the dashboard by adjusting formatting, titles, and color schemes.
      
    - Add tooltips to visual elements to provide extra information when users hover over charts.
      
    - Use bookmarks or storytelling features in Power BI to create a guided view of the analysis.



# Conclusion:
Following these steps ensures a well-organized and insightful sales analysis for Blinkit, with interactive dashboards that make data-driven decision-making easier.









