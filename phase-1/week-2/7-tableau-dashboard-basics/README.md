# Tableau Dashboards - Dashboard Basics

## Introduction
Until now, we have been using Tableau workbooks to get familiar with the Tableau interface. Now we will take your Tableau skills one step further and dive into Tableau dashboards. First, we will get familiar with the Tableau Dashboard Workspace. Then, we will show you how to create a dashboard with Tableau.

## Objectives
You will be able to: 
* Identify and describe dashboard Objects and other elements of a Tableau dashboard workspace
* Use horizontal and vertical containers to create a layout to arrange vizzes and objects on the dashboard
* Add interactive elements to a Tableau dashboard

## Creating a New Tableau Dashboard
There are a few ways to create a dashboard:
1. Menu Bar: In the menu bar at the top of the interface you will see **Dashboard**. Click on this drop-down and select **Dashboard > New Dashboard**.

2. Sheets Tab: To the right of the **New Worksheet** icon, you will find the **New Dashboard** icon.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/7_dashboard_basics/dashboard2-new.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

## Tableau's Dashboard Workspace
Tableau's Dashboard Workspace is similar to the Worksheets workspace, with a few notable differences. Let's review some of the new elements that are introduced in the Dashboard Workspace.

### Device Type Card
One of the benefits of Tableau is that is allows you to easily create visualizations that improve the experience of your end user. In today's business environment, users are often trying to gain insights on the go and like to use mobile devices to interact with dashboards on Tableau. To facilitate use with mobile devices, Tableau has implemented a **Device Type Card** on the Dashboard pane. Right now, the Default is set to **Phone**, which will limit the maximum width and height of the dashboard. 

To accomodate desktop users, we can add a Desktop layout to the Device Card.

1. On the Menu bar at the very top of the page, select **Dashboard > Device Layouts > Add Desktop**.  This option lets you see what your dashboard will look like on different devices, so you can ensure it will be visible. You can even customize the view for each device format. 

2. If you want to remove a device, you can hover over it on the Dashboard pane and click on the `...` and select **Delete Layout**.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/7_dashboard_basics/device-layout.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

### Objects Card
Objects are components that can be incorporated into your dashboard to add additional functionality, customization, and interactivity. The primary objects we will use to build our dashboards are **Horizontal Containers** and **Vertical Containers**.

Let's discuss a few of them using the labeled image below.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/7_dashboard_basics/more-options1.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

1. **Horizontal** - Adds a container to hold objects horizontally
2. **Vertical** - Adds a container to hold objects vertically (more on containers below)
3. **Text** - Adds text boxes in your dashboard to help convey information about your dashboard to the viewer
4. **Image** - Adds images to your dashboard such as a logo
5. **Web Page** - Allows you to embed a web page in your dashboard
6. **Data Story** - Embeds a presentation to add context
7. **Blank** - Adds some blank space
8. **Navigation** - Allows you to create a link to any part of the workbook so the viewer can look closer at some component
9. **Download** - Allows you to embed a button for the viewer to download the viz as a PDF or an image file


**Keep in Mind**: **Ask Data** (10), **Data Story** (11), and **Extension** (12), are not available with Tableau Public. If you would like to research their uses, you can look through the documentation on the <a src="https://www.tableau.com/" target="blank">Tableau Website</a>


### Object Placement
Objects can be placed in the dashboard in one of two manners, either **Tiled** or **Floating**. 

1. **Floating** allows the object to be placed anywhere on the dashboard and can be overlapping any part of the view. 

2. **Tiled** attribute forces the object to share the space with the other objects in the container. 

Both tiled and floating layouts in Tableau have their own benefits and drawbacks, and the choice of which one to use depends on the specific needs of your visualization.

A tiled layout is more structured and grid-like, and is useful when you want to ensure that all of your visual elements are aligned and evenly spaced. Tiled layouts are particularly useful when you are creating dashboards that need to be consistently formatted and have a clear hierarchy of information. Tiled layouts are also generally easier to create and maintain, as the alignment of visual elements is automatically handled by Tableau.

On the other hand, a floating layout provides more flexibility and control over the placement and size of individual visual elements. Floating layouts allow you to position visual elements anywhere on the canvas, including overlapping them, and adjust the size and shape of each element independently. This can be particularly useful when you have complex visualizations with multiple layers, as it allows you to control the placement and size of each layer separately.

Overall, the choice between a tiled and floating layout depends on the needs of your specific visualization. If you need a more structured and consistent layout, a tiled layout is likely the better choice. If you need more flexibility and control over the placement and size of visual elements, a floating layout may be a better fit.

## Building a Dashboard Layout
By using horizontal and vertical containers in Tableau, you can easily organize your dashboard layout and arrange your sheets to create an effective and visually appealing data presentation.

### Adding Containers
Horizontal and vertical containers in Tableau are useful for creating organized and flexible layouts for your visualizations. Here are a few reasons why you might want to use them:

1. Organizing content: Containers allow you to group related content together, making it easier for users to understand and navigate your visualization. For example, you might use a horizontal container to group related charts or tables side by side, or a vertical container to stack them on top of each other.

2. Dynamic sizing: When you add content to a container, it automatically adjusts to fit the size of the content. This means that you can add or remove visualizations or other content from a container without having to manually adjust the size of the container.

3. Consistent layout: Containers help you maintain a consistent layout across multiple worksheets or dashboards. For example, you might use a vertical container to ensure that the spacing between visualizations is consistent across different pages of a dashboard.

4. Resizing and repositioning: With containers, you can easily resize and reposition visualizations within the container by dragging and dropping. This makes it easy to adjust the layout of your visualization as your needs change.

Horizontal and vertical containers are useful tool for organizing and presenting your visualizations in Tableau. They can help you create more flexible and dynamic layouts that are easier for users to navigate and understand. So how do we use them?

1. Create a container: To create a container, click on the "Horizontal" or "Vertical" container button in the "Objects" pane, and drag it onto the canvas where you want to position it.

2. Add visualizations to the container: Drag and drop the visualizations you want to add to the container onto the container itself. You should see a blue drop zone appear around the container when you hover over it with the visualization.

3. Adjust the container: Once you have added your visualizations to the container, you can adjust its size and position by dragging the edges or corners of the container. You can also adjust the spacing between visualizations by dragging the lines between them.

4. Add additional containers: You can add additional containers to the worksheet by repeating steps 3-5. You can create both horizontal and vertical containers, and you can nest containers within each other to create more complex layouts.

5. Customize container properties: You can customize the properties of the containers by right-clicking on them and selecting "Format". From here, you can change the container's background color, add a border, and adjust other properties.

That's it! By using horizontal and vertical containers, you can create flexible and dynamic layouts for your visualizations in Tableau.

## Interactive Elements: Filters
Tableau dashboards can contain interactive elements that allow the end user to alter the view of the data in the dashboard to answer a novel question or perform an **ad hoc analysis**. For example, users can apply **Filters** to view the data that pertains to the segment of the population most relevant to them.

We can apply filters by using the **More Options** menu. You can find this menu by clicking the down arrow on the top right of the viz on your sheet.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/7_dashboard_basics/more-options-2.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

In this example, we add a filter for `Sales (SUM)`. In the upper-right corner, there a slider appears that allows the use to toggle the sales amount they wish to filter by.

<div>
    <center>
<table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3/tableau/tableau/7_dashboard_basics/slider.png" alt="This is the alt-text for the image." style="width: 700px;"/>
</td></tr></table>
    </center> </div>
<br>

## Summary
In this lesson, we introduced Tableau's Dashboard workspace and discussed some of the most important functionality, like Device Type and Objects. Then we discussed how you can add interactivity to your dashboards to allow users to ask questions of the data to gain insights. Finally, we discussed how each of these components works together to enhance the end user experience.
