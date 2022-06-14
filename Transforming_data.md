Load  right hand -- Transfrom data

Don't forget click 'Close & Apply'  if you make any changes

## Power Query Editor

### Applied Steps  
notice it (Applied Steps) tracks and changes
when loading the data, it has already 2 steps

--Source

--Changed Type

--Removed Top Rows (entry 1 just remove the top row)

--Promoted Headers (Click 'use first row as headers' button)

--Changed Type1

--Remove Columns (Press or click, in new version, there is 'Reduce rows' button including 2 buttons: 'keep rows' and 'remove rows')

Answer 6 Applied Steps 

click 'Close & Apply'

### Edit Query  (one field right side, find... then click to choose 'Edit query' )
In the Fields pane, select the 'Edit query' option from DimCustomer.
'DimCustomer' right side has ..., click to choose 'Edit query'.
Return Power Query Editor page, and do that again if we change our mind.

### Quick View
--add new page on the bottom

--make a table, and add color and price fields

--also can change the value you want, avg, sum, and choose clustered column chart


## Transfrom before load

## Field Aggregation
--Visulization pane  Y-axis  Total including tax --find right side arrow--choose Minimum

--According to total including tax, how much is the cheapest sale make to Tailspin Toys 

--Hover on the bar, then got Answer: 5.52

## Transforming and formatting columns
get Power Query Editor by selecting 'transformed data'

Data Type-- different options


Replace Values -- entry ?   blank    replace ? with blank
change Data type

click 'Close & Apply'  ---don't forget


##### In the 'Data' View
Column tools --- Format

0000 ---- 2   2 decimals

Column tools --- Summarization

Go back to 'Report' View --  card  change to decimal 99.53K  Credit Limited (Answer: $99.53K)

(Original is one bar)?? then click card, chose Credit Limited field to get answer.

Another Excercise: 2_4_format_currency.pbix  -------  format currency Summarization  add card for total including tax (Answer: $865.82)

#### Making maps with geographic data
Column tools --- Data categroy

Table tools---

Visualization pane -- Location  City

Visualization pane -- Size Quantity  

Exercise:

Step1:
--Load the dimension table DimCity.csv from the Datasets/WWI folder on the Desktop.

--Go to the Model view and make sure a relationship is found between DimCity and FactSale.

Step2:
In the Data view, change the Data category of DimCity's State Province to "State or Province"

Step3:
Make sure the default summarization for Profit from FactSale is "Average".

Step4:
--In the Report view, navigate to the second tab.

--Create a Map visualazation using State Province as Location and Profit as Bubble size.

Step5:
Add a Slicer for the Buying Group field from the DimCustomer table. Arrange the report to your liking and add a title.

Step6:
Using the map and the slicer, which state generate the highest average profit for the "Wingtip Toys"? Answer: Washington

In Buying Group slicer  click Wingtip Toys, hover the bubbles in the map to see and find the value (Washington/Oregon/California/Alaska).



