# Tableau Dashboards - Cumulative Lab

## Introduction

In previous lessons we have utilized the provided Superstore Sales dataset to learn about the Tableau environment interface, including the Start page, Data Source page, and Workspace/Worksheets. Then, we explored the useful visualizations that can be created in Tableau Public. Finally, we discussed how we can combine the vizualizations in our workbooks to create dashboards to communicate our insights.  Now it's your turn to apply your skills in Tableau.

In this exercise, you will use knowledge of the Tableau interface and data visualizations to create the Super Store Sales dashboard. Refer to previous lessons and labs if needed!

To create the dashboard, follow the instructions below. When you are finished, save and publish your completed dashboard to your Tableau Public account. Then, add the link to your dashboard in this assignment in canvas and click submit. You've just created your first interactive dashboard with Tableau Public.

The final product should look like this:

<br>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/dashboard_final.png/dashboard_final.png" alt="Final Dashboard Image for Super Store Sales" style="width: 800px;"/>
</td></tr></table>
    </center>
</div>

[Tableau Dashboard Link](https://public.tableau.com/views/learn-wb-24-DB/SuperStoreSalesDashboard?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)


## Instructions

### Part A - Connect to THE Data Source and Create a New Workbook

1. Launch Tableau Public and from the Start page, use the Connect pane to open the SuperStore Sales dataset. It can be found in this repo or it can also be downloaded directly from [Tableau Public](https://public.tableau.com/app/learn/sample-data?qt-overview_resources=1#qt-overview_resources).
2. On the Data Source page, populate the page with the `Orders` table and the `People` table. Remember that Tableau will automatically form a relationship if/when possible.

**Note:** This data file is updated periodically by Tableau, newer versions might display different names/infomation then shown below.

### Part B - Create a Bar Chart

*For Part B, use lessons "Tableau Visualizations: Visualization Basics" and "Tableau Visualizations: Visualization Basics Lab" as a reference.*

1. Create a new worksheet - title it "Profits by Sub-Category"
2. Drag the `Profits` pill to the Columns shelf from the Data Pane.
3. Drag the `Sub-Category` pill to the Rows shelf from the Data Pane.
4. Edit the title to be centered and have font size 16. Format the title background/shading to be light gray. **Format Title > Shading dropdown**.
5. Order the bars in descending order.
6. Next, drag the `Profits` pill from the Data pane to the Marks card, and use the Marks card to change the color of the bars to "Orange-Blue Diverging".
7. Next use the Marks card to add labels that indicate the sum of the profits for each of the bars by dragging another `Profits` pill from the Data pane and using the label mark. Format the labels using "Currency (Custom)" under the Numbers formatting option. Display the amount in thousands with the dollar sign symbol. **Bonus:** Change the axis label to include "Thousands"
8. Fit the visualization to "Entire View".

<br>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/profits_subcat.png/profits_subcat.png" alt="Profits by sub catergory image" style="width: 800px;"/>
</td></tr></table>
    </center>
</div>


### Part C - Create a Regional Map

*For Part C, use lessons "Tableau Visualizations: Visualization Basics" and "Tableau Visualizations: Visualization Basics Lab" as a reference.*

1. Create a new worksheet - title it "Sales By Regional Manager". Change the font size to 16, center the title, and change the background to light gray again.
2. Drag the `Longitude` and `Latitude` to the Columns shelf and the Rows shelf respectively.
3. Add `Sales` to the Marks card, and select the Size attribute. Then, add `Postal Code` to the Marks card and select the Detail attribute. This will populate the map with sales by postal code. Using the **Show Me** dropdown, select symbol map if Tableau did not default to the map view.
4. Rename `Person` pill to be `Regional Manager` by right clicking > Rename.
5. Drag the "new" `Regional Manager` pill to the Marks card and select the Color attribute. 
6. Also drag the `Region` pill into the Marks card without selecting a specfic mark. Then left click and change it to color. This should get you both the name and the region as one color label.
7. Then, click the Color icon and select Edit Color. Using the Color Blind pallete, assign the following colors to each Regional Manager, Region:

<br>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/color_select.png/color_select.png" alt="color selection image" style="width: 600px;"/>
</td></tr></table>
    </center>
</div>

8. Next, drag `Profit` to the Marks card and add the Detail attribute. This will allow users to view the profits in conjunction with sales (because high sales does not always mean high profits).
9. Then, drag `Regional Manager` to the Filter shelf. Click the dropdown arrow on the new filter and select **Apply to Worksheets > All Using This Data Source.** This will allow the filter to work across the dashboard.

<br>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/filter_all.png/filter_all.png" alt="apply filter to all" style="width: 600px;"/>
</td></tr></table>
    </center>
</div>

<br>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/sales_region.png/sales_region.png" alt="sales by region map" style="width: 800px;"/>
</td></tr></table>
    </center>
</div>


### Part D - Create a Time Series Line Graph

*For Part D, use lessons "Tableau Visualizations: Visualization Basics" and "Tableau Visualizations: Visualization Basics Lab" as a reference.*

1. Create a new worksheet - title it "Quarterly Sales by Region". Change the title to size 16, center it, and color the background light gray as before.
2. Drag the `Sales` and `Order Date` pills from the Data pane to the Row shelf and the Column shelf respectively. You will notice that `Sales` becomes `SUM(Sales)` and that `Order Date` becomes `YEAR(Order Date)`. On the `YEAR(Order Date)` pill, click the arrow directly to the right of the text on the `YEAR(Order Date)` pill. This will reveal a drop down menu. Select **Quarter** from the dropdown, which will change `YEAR(Order Date)` to `Quarter(Order Date)`.
3. Add `Regional Manager` to the Marks card, and select the Color attribute. In the same manner as the previous figure, also add `Region` to the Marks card without choosing a mark and then change it to color.
4. Confirm that your colors match. Tableau should default to the existing colors you used previously but you should double check to confirm they match!
5. Drag the `Sales` pill to the Marks card and choose Label, format the amounts appropriately.
6. Finally, drag the `Profit` pill to the Marks card and select Tooltip.

<br>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/quarterly_sales.png/quarterly_sales.png" alt="Quarterly sales by region" style="width: 800px;"/>
</td></tr></table>
    </center>
</div>

### Part E - Create and Publish the Dashboard

*For Part E, use lessons "Tableau Dashboards: Introduction", "Tableau Dashboards: Dashboard Basics" and "Tableau Dashboards: Dashboard Basics Lab" as a reference.*

1. Create a new dasboard - title it "Super Store Sales Dashboard"
1. Create the **Desktop** layout by right clicking **Default > Add Desktop Layout**. Select **Fit Width** and set **Height** to 1060px. Then, select **Custom** and **Tiled** from the layout card.
2. Check **Show Dashboard Title**. Change the font size to 26. Center the title and change the background to light gray. When the title is selected, select the Layout tab on the left bar menu, then choose Background.
4. Add a **Horizontal Container** under the dashboard title and set the layout to **Tiled**. 
5. Using two **Vertical Containers**, position the charts and legends in the layout displayed below.
**Remember that you need to add worksheets to the default layout before you can access them in the Desktop layout**

<br>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/dashboard_final.png/dashboard_final.png" alt="final image dashboard" style="width: 800px;"/>
</td></tr></table>
    </center>
</div>

6. Save and publish to Tableau Public as `learn-wb-MM-DD-YY-XX` where `XX` is your initials and `MMDDYY` refers to the current month, date, and year.

7. Locate the share link on your Tableau Public site and submit your dashboard link to canvas. Congratulations you have now published a successful Tableau Public dashboard. Keep exploring this one or dive into some of the other datasets Tableau provides for some more practice creating visuals! Take a look at Tableau Public for some example ideas.

<br>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/publish_share.png/publish_share.png" alt="This is the alt-text for the image." style="width: 800px;"/>
</td></tr></table>
    </center>
</div>

### Level-Up: More advanced filtering

*In Tableau you can set advance filters and highlighters across multiple worksheets via the Actions panel*

1. On any worksheet (not dashboard) go the **Worksheet dropdown > Actions**
2. From here you can add any number of action rules including filtering and highlighting
3. Here are some quick filters to explore for this dashboard.
    - Filter by Sub-Category
        - Source Sheets: Orders+ > **Profit by Sub-Category**
        - Target Sheets: Dashboard > All three
        - Choose to run on select and to show all values when clearing
        - Filter > Selected fields > **Sub-Category**
    - Filter by Regional Manager - for Sub-Categories
        - Source Sheets: Orders+ > **Sales by Regional Manager**
        - Target Sheets: Dashboard > All three
        - Choose to run on select and to show all values when clearing
        - Filter > Selected fields > **Regional Manager**
    - Filter by Manager and Quarter - for Sub-Categories
        - Source Sheets: Orders+ > **Quarterly Sales by Region**
        - Target Sheets: Dashboard > All three
        - Choose to run on select and to show all values when clearing
        - Filter > Selected fields > **Regional Manager** followed by **# QUARTER(ORDER Date)**
4. Check out how all these filters interact on the final dashboard!