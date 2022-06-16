### Making changes (Change and format visuals)

--Edit the slicer:

Visulizations pane

Selection controls--Show 'Select all' option  (slider choose 'On')

turn off the Slicer Header  -- Slicer header  (slider choose 'Off')

Items-- Text size

---Change Matrix to Table 

Still in Visulizations pane click icon 'Table ' which is next to 'Matrix '


Total forecasted sales amount (Answer: $18126759053.91B)

Make sure you did not choose the category, otherwise, you will get the wrong answer: (e.g. $4585888066.580B)


### Editing properties
--Change the table to a matrix

--Go to Format menu under the Visualizations pane and change the text size of the Row Headers and Column Headers to 18.

search Row Headers and Column Headers in Format visual

--Go to the Values section to change the font size in the rest of the columns to 18 as well.

search Values in Format visual

--What is the budgeted amount for cell phones(using two decimal points)? 

### The underlying data and hierarchies

Hover in the matrix, row:Budget, col: Cell phones. (Answer:1208041332.59)


### Sorting and more formatting
slicer--in the top right corner-- clicking three dots ...-- Sort descending/Sort ascending
do the same thing in the bar chart--right corner-- clicking three dots ...---Sort by--MonthName/Amount

Sort by--MonthName, April will be the first month. It seems like the months are sorted in alphabetical order, this is not what we want. To sort the data in the correct way, from January to December, we need to modify the data.

To do this, we'll go to the 'Data' view. Here we'll select the DimDate table.

Now, what we want to do is mofidy a property of the data so it wil always sort the way we want.

choose MonthName, then in 'Column tools' (the contextual menu at the top of the screen)click an icon that says 'Sort by column' , and make sure to sort  MonthName column by 'MonthNumber'. Do the same thing fro ShortMonth. Let's go back to 'Report' view.

Resize the treemap, Format--General--Height (change 285 to 250, you will see the orange part, which is overlapped/covered before)

Change slicer, format--Slicer header On--go back to slicer in down arrow-- choose 'Dropdown'.


### Making it look good/nicer
How to Change Power BI Dashboard Theme?

From the View ribbon, select the Themes dropdown button and select Customize current theme or other themes.

change Height to make slicer dropdown's height as the same as the multi-columns in the card.

right or left instead of resize a visual--using X-position


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

