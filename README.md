# Coffee_Shop_Sales_Analysis-Excel-
Coffee Shop Sales Analysis Using Excel includes the business objective, tools and techniques used (including Power Pivot and DAX), and a breakdown of the analysis process.

## Project Objective
The goal of this project was to analyze and visualize coffee shop sales performance across multiple dimensions (time, product, location, and category) to gain actionable insights for improving business strategy, product focus, and operational decisions.

## Dataset Used
<a href="https://github.com/yug0537/Coffee_Shop_Sales_Analysis-Excel-/blob/main/Coffe_Shop_Sales-Raw.xlsx">Raw Data<a/>

## Tools & Technologies Used
- Microsoft Excel
    - Power Query (for data cleaning and transformation)
    - Power Pivot (for data modeling and creating relationships)
    - DAX (for calculated columns and measures)
    - Pivot Tables & Charts
    - Slicers
    - Custom Visualizations for Dashboard

## Key Performance Indicators(kPIs)
- Total Sales : $698,812.33
- Total Footfall : 149,116
- Average Bill per Person : 4.69 
- Average Orders per Person :  1.44
- Store Location Performance : Top Store by Sales: Hell’s Kitchen – $236,511.17 :Top Store by Footfall: Hell’s Kitchen – 50,735
- Daily Order Distribution : Highest Orders Day: Friday – 21,701 orders : Lowest Orders Day: Saturday – 20,510 orders
- Size Distribution of Orders : Most Ordered Size: Regular (31%) and Large (30%)

## Dashboard Interaction
<a href="https://github.com/yug0537/Coffee_Shop_Sales_Analysis-Excel-/blob/main/Coffe_Shop_%20Sales_File.xlsx">Dashboard<a/>

## Data Preparation & Processing Steps
1. Data Cleaning with Power Query
   - Removed duplicates and null values
   - Converted date and time columns into proper formats
   - Split time to extract hour for time-based analysis
2. Data Modeling in Power Pivot
   - Created relationships between table Columns and Written some DAX queries including Some Formatting
3. DAX Calculations Used
   - Total Sales = SUM([Total_Bill])
   - Total Footfall = DISTINCTCOUNT(Transaction[Transaction ID])
   - Avg Bill Per Person = Sum(Transactions[Total_Bill])/Count(Transactions[Transaction_id])
   - Avg Order Per Person = Sum(Transactions[Transaction_qty])/distinctcount(transactions[transactions_id])
  
## Dashboard View
<img width="1394" alt="Screenshot 2025-05-17 at 16 55 33" src="https://github.com/user-attachments/assets/4c5854f3-3aad-4b1b-86d3-64c0ac24ea8e" />

## Key Insights
1. Sales Performance
   - Total Sales: $698,812.33
   - Total Footfall: 149,116
   - Avg. Bill / Person: $4.69
   - Avg. Orders / Person: 1.44
2. Peak Hours
   - Highest quantity ordered between 8 AM and 9 AM, aligning with morning rush hour.
3. Top Product
   - Barista Espresso generated the highest sales (~$91K)
4. Popular Categories
   - Coffee leads with 39% of total sales.
   - Followed by Coffee Beans (28%) and Drinking Chocolate (10%)
5. Store Locations
   - All stores (Astoria, Hell’s Kitchen, Lower Manhattan) perform similarly, with Hell’s Kitchen slightly ahead in total sale
6. Weekday Trends
   - Friday sees the highest number of orders (~21,700), followed by Thursday and Monday.
   - Saturday has the lowest, indicating less weekday traffic.
7. Order Size Analysis
   - Orders are almost equally split between Regular (31%), Large (30%), and Not Defined (30%)

## Conclusion & Recommendations
- Morning Promotions: Boost sales further during morning hours (7–9 AM) through targeted offers.
- Product Focus: Continue promoting Barista Espresso and high-margin items like Coffee Beans.
- Stock Optimization: Ensure key products are always in stock across high-performing locations.
- Customer Engagement: Consider loyalty programs to increase average orders per person.
- Weekend Strategy: Run special promotions or events on weekends to drive more traffic.




