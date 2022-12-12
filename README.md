# Holiday Investment Analysis Assignment
Analyze ecommerce data to help the stakeholder determine the marketing budget.

# Assignment
<b>Stakeholder Question</b>: The marketing budget is being set for next year. We would like to know the holiday 
that brings in the most revenue. Please complete this task by the end of day tomorrow. The ecommerce sales data is provided.
<br><b>*Ecommerce data for December is not provided.*</b></br>

# Datasets
<ol>
  <li><b>Ecommerce Dataset</b>: Will use the dates of sale, quantities and prices of items sold.</li>
  <li><b>U.S. Holiday Dates Dataset</b>: Will use dates and names of U.S. Holidays</li>
</ol>

# Cleaning and Organizing Data
<h3>The following was done on Excel and Power Query Editor:</h3>
<h4>Joining the Ecommerce Dataset and Holiday Dates Dataset</h4>
<ul>
  <li>Change date format to month/day/year (mm/dd/yyyy) and remove the time (hh:mm:ss) from the Holiday Ecommerce dataset</li>
  <li>Merge the Ecommerce Dataset and the U.S. Holiday Dates Dataset by using a Left Outer Join (Also known as a left inclusive join or left join) </li>
</ul>  

&emsp;&emsp;![LeftJoin](https://user-images.githubusercontent.com/110753469/194694889-38b5391a-f5cc-4570-93c6-7f7018d9363b.PNG)
<ul>
  <li>The left outer join will include all the data from the Ecommerce Dataset and only the matching data between the U.S. Holiday Dates and Ecommerce Datasets. Both   datasets will be joined by the matching dates.</li>
  <li>The new table created by the join will be named the Analysis Table.</li>
</ul> 
<h4>Modifying the Analysis Table</h4>
<ul>
  <li>Dates that are not holidays ("null" values) will be replaced with "Normal Day"</li>
  <li>Group same dates and holiday names on the Analysis Table</li>
  <li>Create two new columns, Total Revenue (sum of revenue) and Total Quantity (sum of quantity)</li>
  <li>Create a Pivot table with the average revenue and quantity for each holiday</li>
</ul>

&emsp;&emsp; ![PivotTable-AveRevQuantHoliday](https://user-images.githubusercontent.com/110753469/194737459-50c55170-4eee-483c-8198-0ec4c5ba882f.png)

<h3>Pivot Table</h3>

&emsp;&emsp; ![ExcelVisual-AveRevQuantHolidays](https://user-images.githubusercontent.com/110753469/194737855-fadcdf61-b294-43af-b349-8f15f71d882c.PNG)

# Analysis and Recommendation
<ul>
  <li><b>Analysis</b>: The analysis shows that Thanksgiving Eve has the largest average revenue and item quantity sold when compared to the rest of the holidays.</li>
  <li><b>Recommendation</b>: Dedicating a larger portion of the marketing budget during the lead up to Thanksgiving Eve may produce higher revenue during this period.</li>
<ul>
