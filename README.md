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



     
**2. Sales Analysis by Item Type:**
   - **Goal:** To evaluate the sales performance of various item types.
   
   - **Additional KPIs to Consider:** Examine other metrics such as Average Sales, Number of Items Sold, and Average Ratings across different item types.
     
   - **Recommended Chart Type:**  Bar Chart.




**3. Outlet Comparison of Fat Content in Relation to Total Sales:**
   - **Goal:** To compare total sales across different outlets categorized by fat content.
 
   - **Additional KPIs to Consider:** Investigate how Average Sales, Number of Items, and Average Ratings change with fat content across outlets.
    
   - **Recommended Chart Type:** Stacked Column Chart.



     
**4. Total Sales by Outlet Characteristics:**
   - **Goal:** To explore how the establishment’s type or age affects total sales.
 
   - **Recommended Chart Type:** Line Chart.



     
**5. Total Sales Based on Outlet Size:**
   - **Goal:** Investigate the relationship between the size of the outlet and the total sales figures.
    
   - **Recommended Chart Type:** Donut or Pie Chart.



 
**6. Sales Distribution by Location:**
   - **Goal:** Evaluate how sales are geographically distributed across various locations.
    
   - **Recommended Chart Type:** Funnel Map.



 
**7. Comprehensive Metrics Overview by Outlet Type:**
   - **Goal:** Display a detailed breakdown of all key metrics (including Total Sales, Average Sales, Number of Items Sold, and Average Ratings) segmented by different outlet types.
    
   - **Recommended Chart Type:** Matrix Card.




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
   
   - **Sales Analysis by Item Type**:
     - Insert a **Bar Chart**.
       
     - Add **Item Type** to the axis and **Total Sales** to values. Add **Average Sales** as a secondary metric if needed.
   
   - **Outlet Comparison of Fat Content in Relation to Total Sales**:
     - Use a **Stacked Column Chart**.
       
     - Place **Outlets** on the x-axis and **Fat Content** on the legend. Add **Total Sales** as the main value.
   
   - **Total Sales by Outlet Characteristics**:
     - Use a **Line Chart** to map sales based on outlet types or outlet age.
   
   - **Total Sales Based on Outlet Size**:
     - Add a **Donut or Pie Chart** to visualize the relationship between outlet size and sales.
   
   - **Sales Distribution by Location**:
     - Use a **Funnel Map** to display sales geographically. Assign locations to the map and **Total Sales** as values.
   
   - **Comprehensive Metrics Overview by Outlet Type**:
     - Use a **Matrix Visual** to show detailed metrics like **Total Sales**, **Average Sales**, **Number of Items Sold**, and **Average Ratings**, all broken down by **Outlet Type**.

10. **Apply DAX Formulas for Data Analysis**
    - After creating visuals, apply DAX formulas to make your analysis dynamic. For example, add slicers for outlet type or date range, which will adjust the data displayed across all charts.
      
    - Example DAX for filtering by date:
      
      ```DAX
      Sales Last Year = CALCULATE([Total Sales], SAMEPERIODLASTYEAR(Sales[Date]))
      ```

11. **Extract and Present Insights**
    - Finalize the dashboard by adjusting formatting, titles, and color schemes.
      
    - Add tooltips to visual elements to provide extra information when users hover over charts.
      
    - Use bookmarks or storytelling features in Power BI to create a guided view of the analysis.

12. **Publish and Share**
    - Once the dashboard is complete, publish it to Power BI Service and share it with stakeholders. Set up refresh schedules if your data source is updated regularly.

### Conclusion:
Following these steps ensures a well-organized and insightful sales analysis for Blinkit, with interactive dashboards that make data-driven decision-making easier.









