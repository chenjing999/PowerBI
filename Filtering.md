### Drilling down and filtering
A hierarchy enables the ability to show different levels of data without having to create new visuals.

By adding a hierarchy to your visualizations, you can easily navigate up and down a hierarchy. For example, you can display data for each year, zoom in on a quarter, and end with a month.


### The underlying data and hierarchies
Bar chart -- click three dots--show as a table

Export data

how to create the hierarchies

1. Go to 'Data' view--Drag Qrt on top of Year, when we do that,  a hierarchy is automatically created. (you will see 'Year hierarchy ')

we are going to rename the hierarchy by double clicking on the hierarchy name and changing it to 'Date Rollup'.

Then we'll add the MonthName, we could drag it over like before, or, right click on the column name and then add it to the 'Date Rollup' hierarchy. (right click 'MonthName', choose 'Add to hierarchy', choose 'Date Rollup')

You could switch the order of them in 'Date Rollup' by dragging them in the correct order. You can also switch them back.

2. Go back to the 'Report' view, Visulazation pane--Axis--'Date Rollup' (drag/ choose)

Bar chart --click down arrow to turn on Drill down -- After doing that, down arrow turns to black, meaning it is enabled. if you don't turn on drill down, selecting a visual element won't drill down. instead, it will cross-filter the other charts on the report page. As we covered eariler, the double arrow will get us down another levels for all years, and the double arrow with a line combines information from the current and next level.

Bar chart --click 'double arrow'  or click the 'double arrow with a line' to get a feel for how drilling works.

#### Exercise:
1. Navigate to the DimDate table in the Data View.

2. Create a hierarchy that starts with 'Year', goes on to the QuarterFull, then the MonthName, and ends with the DateKey.

If the drag functionality isn't working, you can right-click DimDate's Year in the Fields pane and select 'Create hierarchy'. From there, you can right-click the necessary fields and select 'Add to hierarchy'.

3. Rename the hierarchy to Date Hierarchy.

4. In the column chart on the Report view, replace the ShortMonth Axis value of the column chart by the Date Hierarchy.

5. Use the drill controls in the top right corner of the visual to explore the different levels. Click the single down arrow to enable drill mode.

6. Which quarter across all years had the highest amount (format example: Y2020 Q1)  (Answer: Y2017 Q4)

Click the single down arrow--click one bar to see the details in a year (click 2017 and you will see four quarter value Q1 Q2 Q3 Q4). If you want to return, using the single up arrow, do the same thing with 2018 and 2019, and compare to find the quarter that had the highest amount.


Go to 'Data' view--Drag QuarterFull on top of Year does not work, we could click three dot on the right hand of 'QuarterFull ', and choose 'Create hierarchy' (you will see 'QuarterFull hierarchy ')

Go back to the 'Report' view, Click bar chart first, then Visulazation pane (Build visual)--Axis (X-axis ShortMonth change to Date Hierarchy, e.g. drag Date Hierarchy from the Fields to X-axis)
