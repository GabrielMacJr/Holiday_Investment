#Holiday Investment Analysis Assignment
Analyze ecommerce data to help the stakeholder determine the marketing budget.

#Assignment
<b>Stakeholder Question</b>: The marketing budget is being set for next year. We would like to know the holiday that brings in the most revenue. Please complete this task by the end of day tomorrow. The ecommerce sales data is provided.
Datasets
1.	Ecommerce Dataset: Will use the dates of sale, quantities and prices of items sold.
2.	U.S. Holiday Dates Dataset: Will use dates and names of U.S. Holidays
Cleaning and Organizing Data
The following was done on Excel and Power Query Editor:
Joining the Ecommerce Dataset and Holiday Dates Dataset
•	Change date format to month/day/year (mm/dd/yyyy) and remove the time (hh:mm:ss) from the Holiday Ecommerce dataset
•	Merge the Holiday Ecommerce Dataset and the US Holiday Dates Dataset by using a Left Outer Join (Also known as a left inclusive join or left join)
   
•	All the data from the Ecommerce Dataset will be included and the matching data between the
•	U.S. Holiday Dates and Ecommerce Datasets will be kept. Both datasets will be joined by the matching dates.
•	This new table created will be named the Analysis Table.
Modifying the Analysis Table
•	Dates that are not holidays (null values) will be replaced with the name Normal Day in the Analysis Table
•	Group by Dates and Holiday Names on the Analysis Table
•	Create two new columns, Total Revenue (sum of revenue) and Total Quantity (sum of quantity)
•	Create a Pivot table with the average revenue and quantity for each holiday
    
Pivot Table
    
Analysis and Recommendation
•	Analysis: The analysis shows that Thanksgiving Eve has the largest average revenue and most quantity sold when compared to the rest of the holidays.
•	Recommendation: Dedicating a larger portion of the marketing budget during the lead up this holiday may produce higher revenue during this period.

