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


### Filters
just show Top 10 in the Sales Amount by Location
Click the bar chart --

Filters pane--Filters on this visual, it is 'Amount'

Filters pane--Click on EntityName, and under here where it says Basic Filtering (under the 'Filter type'), select Top N. So that is going to give us the top N numbers of entities, meaning locations, and we want 10. 

Filters pane--Show items: Top and we have to input 10. 

Filters pane--By value, we need to use Amount, drag Amount from Fields to 'By value', then click 'Apply filter'


Bar chart-- Click three dot--choose 'Sort by' then choose 'Amount'

Bar chart-- Click three dot--choose 'Sort descending'

Then you could see the Top 10 Locations


We will change the visual to a clustered bar chart, to mix the visuals up a bit.

Next, we want to filter all pages to only show Actual sales amounts. To do that, we need to look at how the data is reported. Let's go to the Date View and look at the values in the FactStrategy table. We can see that the values have a scenario listed. (ScenarioKey column)

If we go to DimScenario we can see that the scenarios tell us whether the amount is actual, budgeted or forecasted. (ScenarioName column including: Actual, Budget, Forecast)

We are only interested in the actual values in this report, so let's add ScenarioName to the filter pane.

We want to filter on all pages so let's drag ScenarioName to Filters on all pages.

ScenarioName in Fields pane-- drag to--'Filters on all pages' in Filters pane.

There are three options, only select 'Actual'. Now every single amount value is just the actual amount. That is going to impact every page. Note that it's also possible to filter on a single page. (There is 'Filters on this page' above 'Filters on all pages', still in the Filters pane)

Actual Amount (card)

Sales Amount by Location   (bar chart --horizental)   

Monthly Amount  (bar chart--vertical)

Contoso Actual Sales Results (text title)

Year.QuaterFull  (slicer)

Notice that every time we click on a product category, the actual amount changes. But we don't want it to change, we want it to always be the same.

Let's go into the 'Format' tab (on the top) on top and choose'Edit the interactions' (under the 'Format' tab).

When we do that, you will notice filter and no symbols popping up on the visualizations. (small chart icon O/)

Let's select the Monthly amount visulization. (click [Monthly amount] bar chart)

Since this is the one highlighted, this is the context the filtering is going to happen in.

This means thay by editing the interactions we can change how the selected visualization, the Monthly Amount chart, interacts with he other visulizations on the report page. Let's turn off the interaction. (click small chart icon O/, and O/ turn to black)

Now, the actual amount will not be filtered based on what is selected in the Monthly Amount visual. 

Let's do the same thing for Year. Note that you might have to move some visuals around to see the interaction icons.

Let's look at the results. Turn off the 'Edit the interactions' functionality in the top left corner. You can see the interactions are disabled.

If you select a product category or filter on year, the Actual Amount card in the top left corner doesn't change. 


#### Exercise--Adding a filter

Context:

Filtering is an important tool when you're creating Power BI reports. You don't always want to look at all the data. Limiting the data used in visuals to only a selection that is relevant can help you anwser more detailed business question.

In the report, you can see that the cards on the Sales Analysis page tab are labeled Actual, Forecast, and Budget, but they all have the same values. You'll need to apply some filters to fix this.

Instructions:

1. 4_3_adding_a_filter.pbix report from Exercises folder

2. --Open the Filters pane
--Add a filter to the 'Actual' card visual that filters on rows where ScenarioName is equal to Actual.

When you click the 'Actual' card, 

There is 'Filters on this visual' above 'Filters on this page' and 'Filters on all pages', still in the Filters pane. (you will see 'Amount is All' under 'Filters on this visual')

Drag ScenarioName from Fields pane to 'Filters on this visual' in the Filters pane (Add data fields here)

Do the same for Forecast, and Budget respectively. Answer: Forecast Amount 18.13bn  (Actual: 18.34bn. Budget: 17.17bn)

### Turning off interactions
interaction icon -- O/ --the circle with the line through it.

Select the 'Budget Product Solid' visual.

Go into the interaction editing mode in the Format tab at the top of the screen.

Turn off the interactions with each of the three cards.

Click the 'TV and Videos' bar in the 'Budget Product Solid' visual. Amount in Budget card. (Answer: Budget: 17.17bn)

