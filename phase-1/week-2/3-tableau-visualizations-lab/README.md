# Tableau Visualizations - Visualizations Basics Lab

## Introduction
In previous lessons, we reviewed all of the essential components of the Tableau environment to help you quickly begin creating visualizations in Tableau. We have learned how to connect to resources to create a data source. Then, we learned how to create relationships between our connected data and generate worksheets. Finally, we built out some simple visualizations. 

Now that you have gotten a taste of some of the features Tableau has to offer, it is time to put that knowledge to work and test out additional features. In this lab, we are going to use our knowledge of Tableau's interface and its functionality to create a workbook that can help us to build out a cohesive dashboard and tell a story with our data. 

## Learning Objectives

You will be able to:
* Create a customized bar chart in Tableau
* Create a customized regional plot
* Create a customized time series plot in Tableau

## Visualizing Profits
Suppose you want to create a visualization that will communicate which kinds of products yield the most profits. A bar chart is a great choice for conveying this kind of information. In previous lessons, we created a simple bar chart and demonstrated how to use Tableau's functionality to customize it. Now, it's your turn to create a bar chart.

### Connect to a Data Source and Launch the Tableau workspace
1. Launch Tableau and use the Connect pane on the Start page to connect to the Super Store Sales data set.

2. From the Data Source page, drag the `Orders` table and the `Returns` table to the canvas. A noodle should form between the table names to indicate an automatic relationship.

3. Select Sheet 1 from the Sheets tab to launch the Tableau Workspace.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/6_data_viz_lab/tab-1.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

### Create a Bar Chart
4. Rename the new worksheet "Profits by Sub-Category".

5. Drag the `Orders. Sub-Category` pill from Dimensions in the data pane to the Column shelf. Then, drag the `Orders. Profit (SUM)` pill from Measures and drag them to the rows shelf. 

5. Select **Swap** from the Command bar to transform the bar chart into a vertical bar chart.

7. Navigate to the top of the Sheets pane and edit the title so that it is centered and has a size 16 font.

8. Navigate to the Fit drop-down on the Command bar at the top of the screen. Select "Entire View".

Now, your screen should look like this:

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/bar-first.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

### Customize a Bar Chart
9. Drag the `Orders. Profit (SUM)` pill from the Data pane to the Marks card. Then, assign the Color attribute. This will automatically change the color of the plot. Next, we will customize by clicking on the Color card on the marks card and entering the same parameters from the image below.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/viz-lab-colors.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

10. Drag the other `Orders.Profit (SUM)` pill from the Data pane to the Marks card. Then, click on the icon next to the pill and select Label. This will automatically apply a label at the top of each bar on the chart to indicate the value of `Orders.Profit (SUM)` for that sub-category.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/bar-marks.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>


11. Right-click on one of the labels you created and select **Format**. The Format pane will appear to the far left of your screen. 

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/format.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>



12. Under the Default heading, select the **Number** drop-down and choose **Currency (Standard)**, and set the decimal places to zero. Close the Format pane.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/currency.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

13. Now, you should have a plot that looks like this:

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/bar-final.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>


## Visualizing Orders by Region
Next, let's create a chart that visualizes the number of orders by region.

### Create a Regional Map
1. Select the New Worksheet Icon from the sheets tab.

2. Double-click the title bar on the Sheets pane and enter "Orders by Region". Center the title and change the font size to 16.

3. Drag the `Orders.Orders Count` pill from the Data pane to the Rows shelf. Then, drag the `Orders.Postal Code` pill to the Columns shelf. 

Your screen will look like this:

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/region-1.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

4. Next, select the Show Me Pane from the upper right-hand corner of the screen and choose the Map visualization. Tableau will automatically rearrange the pills between the Row and Column shelf, like so:

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/region-2.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

### Customize the Regional Map
5. Next, go to the Marks card and change the `CNT(ORDERS)` pill to the Size attribute.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/region-3.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

7. Then, drag `Region` from the Data pane to the Marks card and change the attribute to Color.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/region-4.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

5. Navigate to the Fit drop-down on the Command bar at the top of the screen. Select "Entire View".

Your screen will look like this:

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/region-5.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

Great, now we have a plot that visualizes the orders by region!

### Visualize Sales Over Time
Finally, we will visualize monthly sales on a time series plot, which is a version of a line graph.

1. Select the New Worksheet Icon from the sheets tab.

2. Double-click the Title bar on the Sheets pane and enter "Sales by Month". Make the typeface bold and change the size to 22.

3. Then, double-click the tab for the current sheet in the Sheets tab and rename the tab "Sales".

4. Drag the `Orders.OrderDate` pill from the Data pane to the Columns shelf. You will notice that the pill is transformed and now reads `YEAR (OrderDate)`. 

5. Drag the `Sales (SUM)` pill to the Rows shelf. 

6. Navigate to the Fit drop-down on the Command bar at the top of the screen. Select "Entire View".

Your screen will look like this:

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/6_data_viz_lab/time0.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

7. Navigate to the Columns shelf and select the down-arrow on the `YEAR (OrderDate)` pill and select "Month".

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/6_data_viz_lab/time2.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

8. Now, your plot should look like this:

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/6_data_viz_lab/time3.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

8. Next, drag the `Orders.Category` pill to the Marks card. Select the icon to the left of the pill and select Color. Finally, select the Show Me pane and drag it away from the right corner. You will notice a legend that provides the product category for each color. This is the final product:

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/6_data_viz_lab/time-final.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

## Save to Tableau Public
Finally, we are going to save our new workbook to Tableau Public so we can retrieve it in future lessons to build out our dashboard.

1. Select the Save Icon from the Command bar at the top of the Tableau workspace.

2. Log into Tableau if prompted.

3. Save and publish to Tableau Public in your `learn-wb`. 

## Summary
In this lesson, we created three customized plots for three different use cases. We created a bar plot to demonstrate profits among the different product sub-categories in the Super Store Sales data set. Then, we created a scatter plot to visualize the relationship between sales and discounts and added size to demonstrate the number of orders. Finally, we created a viz that communicates monthly sales over time for the three product categories.



