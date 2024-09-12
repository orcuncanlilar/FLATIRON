# Tableau Dashboards - Creating a Dashboard Layout

## Introduction
In this lab, we will provide a guide on how to build dashboards in Tableau in ten simple steps. The guide begins by emphasizing the importance of planning a dashboard and clarifying the objectives to visualize data effectively. The steps include creating a new dashboard, choosing the appropriate layout, adding sheets, arranging and resizing them, adding filters, titles and text, customizing the appearance, and publishing the dashboard. Then, you will complete an exercise in building a simple dashboard for visualizing sales by sub-category in two ways: total sales by sub-category and total regional sales for the top-5 sub-categories.

## Objectives

You will be able to:

* Create a dashboard in a Tableau workbook
* Use horizontal and vertical containers to implement a dashboard layout
* Apply customizations and add filters to a dashboard
* Save and publish a dashboard to Tableau Public

## Steps for Building Dashboards in Tableau
Now that we have learned the basics of Tableau dashboarding, it's time to build our own dashboard. Let's walk through the process step by step.

### Step 1: Plan your Dashboard
Before you start building your dashboard, it's important to have a clear idea of what you want to achieve and what data you want to visualize. Think about the questions you want to answer and the insights you want to communicate to your audience.

### Step 2: Create a New Dashboard
In the previous lesson, we discussed that there are a couple of ways to create a new dashboard in Tableau. One option selecting **Dashboard > Create New Dashboard** from the Menu Bar at the top of the screen. The other option is to use **New Dashboard** icon on the Sheets tab.

### Step 3: Choose your Layout
Choose the layout that best suits your needs from the "Layout" pane. You can choose from a variety of preset layouts, or create your own custom layout.

### Step 4: Add Sheets
Add one or more sheets to your dashboard by dragging them from the "Sheets" pane onto the dashboard canvas. You can add sheets for different types of visualizations, such as bar charts, line charts, maps, or tables.

### Step 5: Arrange and Resize Sheets
Arrange and resize the sheets on your dashboard by dragging and dropping them, and adjusting their size and position. You can also use containers to group related sheets together.

### Step 6: Add Filters
Add filters to your dashboard to allow users to interact with the data. You can add filters to individual sheets or to the entire dashboard.

### Step 7: Add Titles and Text
Add titles and text to your dashboard to provide context and guidance to users. You can add titles and text boxes using the "Text" tool in the "Objects" pane.

### Step 8: Customize the Appearance
Customize the appearance of your dashboard by selecting "Format" from the main menu. From here, you can change the background color, add borders, adjust fonts and colors, and make other cosmetic changes.

### Step 9: Publish your Dashboard
Once you're happy with your dashboard, you can publish it to Tableau Server or Tableau Online to share it with others. You can also save it as a packaged workbook to share with users who have Tableau Desktop

## Your Turn: Build a Simple Dashboard
Now that we have reviewed the steps, let's walk through them together to build out a simple dashboard.

### Dashboard Use Case
To complete step one, we have to understand our use case and plan our dashboard. 

For this exercise, our use case is to create a dashboard that will communicate Sales by Sub-Category in two ways:
1. Total Sales by Sub-Category
2. Total Regional Sales for the Top-5 Sub-Categories.

To communicate these data points, we can use a **bar chart** and **regional map** as visualizations.

## Create a New Dashboard and Vizzes
1. Open `learn-wb` and create a new dashboard using the Menu Bar or the Sheets tab. 


### Build Viz 1
2. Change the name of the dashboard sheet to "Regional Sales Dashboard".

3. Click on the Sheets tab for the "Profits by Sub-Category" visualization. Right click and select *Duplicate**.

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-duplicate-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>

4. Rename the new copy "Sales by Sub-Category".

5. Next, select the `SUM(PROFITS)` pill from the Column shelf. Right click and select **Remove**. Then, drag `Sales` from the Data Pane to the Columns shelf. Re-order as **Descending** if needed.

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-remove-profit-0.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-remove-profit.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>


5. Drag `Sales` from the Data Pane to the Marks card and add a Color attribute. Then, add a Label attribute for `Sales` to display the sales in USD. (Don't forget the currency symbols!)

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-change-color-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>


<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-format-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-currency-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>

Your viz should look like this:

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-final-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>



### Build Viz 2
6. Click on the sheet tab for "Sales by Sub-Category" and select **Duplicate**.

7. Rename the new copy "Regional Sales for Top Sub-Categories".

8. Then, arrange the Column and Row shelf so that that `SUM(Sales)` is in the Column shelf and `Sub-Category` and `Postal-Code` are on the Rows shelf.

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-2-bar-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>


9. Select the **Show Me Pane** from the upper right corner of the screen, and select **Map**.

10. You'll notice that Tableau automatically does a few things:
a. Generates `Longitude` and `Latitude` from `Postal Code`. `Postal-Code` also gets moved to the Marks card. with a Detail attribute.
b. Tableau also automatically moves `Sales` to the Marks card and adds a Size attribute.


<p>
<div>
    <center>
<table><tr><td>
<video controls src = "https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/show-me-map.mov" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>


11. Next, Remove `Sub-Category` from the Rows Shelf and add `Sub-Category` to the Marks card and assign a Color attribute.

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-2-change-color-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>


12. Now, let's filter the data so that only categories in the top 5 for sales are featured by dragging the `Sub-Category` Dimension to the Filter shelf. Then, right click and select **Edit Filter > Top > By Field > Top: 5 > Sales > Sum**, then apply. 

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-2-filtered-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>

### Build Dashboard Layout
13. Now that we have two new vizzes, we can build a dashboard by selecting the New Dashboard icon from the Sheets tab.

14. From the Dashboard pane, add a Desktop Layout. 

15. Then select:
    a. Default layout
    b. Tiled
    c. Show Title
    
<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/dashboard-layout-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>


16. Next, right click the dashboard title and select **Edit Title**. Make sure that the title is centered, and that the font size is 18.

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/dashboard-title.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>



17. Next, drag a Vertical Container from the Objects card and add it beneath the title. Drag the "Sales by Sub-Category" viz from the Sheets Pane over and drop it under the title. Then, drag the legend from the left side of the dashboard underneath the viz.


<p>
<div>
    <center>
<table><tr><td>
<video controls src = "https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/dash-1.mov" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>


18. Next, drag a Horizontal Container from the Objects card and drop it underneath the bar chart and legend. Then, drag and drop the "Regional Sales by Sub-Category" viz into the container from the Sheets pane. Make sure that the legends appear to the left of the map. 

In the video below, we perform steps 17-18.

<p>
<div>
    <center>
<table><tr><td>
<video controls src = "https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/dash-3.mov" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>

18. Next, click on the bar chart and select **Use as a Filter**.

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-use-filter.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>

<p>
<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/8_dashboard_labs/viz-1-use-filter-2-1.png" alt="Image of the sheets tab in the lower-left corner of the Tableau Data Source Page, with the Left Pane and Canvas visible." alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center>
</div>

Now, you can use the categories in the bar chart to filter the entire dashboard, including the regional map.


19. Save and Publish to Tableau Public! Submit your workbook link when you are finished.

## Summary
In this lab, we reviewed the basic steps for building a dashboard. The steps include planning the dashboard, choosing a layout, adding sheets, arranging and resizing sheets, adding filters, adding titles and text, customizing the appearance. Then, we walked through creating a simple dashboard for communicating Sales by Sub-Category in two ways: Total Sales by Sub-Category and Total Regional Sales for the Top-5 Sub-Categories.

By now, you should have a fairly good understanding of dashboarding basics in Tableau. In the upcoming cumulative lab, you will have a chance to apply your skills and create an interactive dashboard on your own.
