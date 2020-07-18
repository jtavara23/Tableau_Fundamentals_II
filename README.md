# Tableau - Desktop II: Intermediate

Tags: ToDo, in progress
source link: https://elearning.tableau.com/desktop-ii-intermediate

### About This Course

In this course, I pushed my data analysis skills in Tableau Desktop to the next level. Determining when to create extracts and when to use joins, unions, and blends to modify data connections. I've learnt to filter across data sources and analyze subsets of data using context filters and sets. I went further with calculations, using LOD expressions and specifying options to control table calculations, and I did more with mapping. To enable analysis, I created parameters and user controls, and show data trends and forecasts, as well as data distributions. Round out your skills by designing dashboards that incorporate visual best practices.

### **Time Estimate:**

8+ hours

### Some **Learning Objectives**

- Combine data from multiple tables using joins and unions, and learn when to use blends.
- Use extracts to improve performance.
- Build advanced chart types, including bar-in-bar and bullet graphs.
- Use advanced calculations and table calculations to modify data as needed for analysis.
- Use statistical techniques to analyze your data.
- Use parameters and input controls to support audience analysis.
- Implement advanced geographic mapping techniques and use custom images and geocoding to build visualizations of non-geographic data.
- Build better dashboards using techniques for guided analytics, interactive dashboard design, and visual best practices.

---

---

## 1. **Working with a Data Extract**

- It creates a TDs file.
- A live data connection may not be an option (offline). Maybe you're traveling, or the connection is slowing down workbook performance. Discover the power of data extracts!
- Use a data extract to improve workbook speed, streamline data in the view, and add portability to a workbook, as we are working with a copy of the data.
- Uses Tableau Data Engine to Perform queries (queries are not processed in the source dB) .
- May include only a subset of the data.

Some limitations:

- Doesn't update automatically - manually refresh the data extract or configure a incremental/scheduler refresher.

We can use it from here:

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled.png)

Or from here:

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%201.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%201.png)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%202.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%202.png)

the symbol changed:

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%203.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%203.png)

Update extract: 

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%204.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%204.png)

## 2. **Joining Tables**

inner, left, right, and outer join

## 3. **Joining Tables Using Calculations**

we can to create a join field but that new field won't be available for using in sheets or dashboard.

## 4. **Blending Multiple Data Sources**

Blue checkmark to the primary  Data-source. It's defined by the first field we drag on the view.

Orange checkmark on the pane for the secondary source.

It always behaves as a LEFT JOIN.

we can change which it's the principal and visitor sheets on multiples sheets through the workbook.

## 5.**Blending Data without a Common Field**

- We need to create a common field, we can do it by:
    - Renaming the field in one of the data-sources.
    - Data > Edit Relantiopships

we can also edit Aliases  or create field from already created fields:

- Data > *SourceDataName* > Edit Aliases > *Specific FIeld*

## 6.**Using Unions to Combine Data**

Whereas **joins appends COLUMNS**, **unions appends ROWS.**

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%205.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%205.png)

## 7.**Filtering Across Data Sources**

Across database filter: we need to find/create a common field (datatype and name matches) that we are gonna use it as main field for all worksheets. 

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%206.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%206.png)

## 8.**Using Sets to Highlight Data**

create Sets to monitor key data values(part of data).

A set commonly appeared under Measures.

Tableau automatically creates an IN/OUT field for sets.

Sets can be used as a Filter as well.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%207.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%207.png)

Combined Sets: allows you to compare multiple sets to one another.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%208.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%208.png)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%209.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%209.png)

## 9.**Using Context Filters to Limit Scope**

Context Filter: Pre filter for a filter. 

Has to be positioned as the first filter.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2010.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2010.png)

## 10. **Using Split and Custom Split**

you can't join on a split but you can blend on it. 

we can make it custom

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2011.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2011.png)

we can make it automatically from the Data Source or "Transform"  in the field's option

## 11. **Advanced Calculations: Aggregating Dimensions**

Dimensions can be aggregated in 3 ways:

- Creating a new calculated field
- Dragging dimension into the view and select an aggregation types: ATTR, MAX, MIN , COUNT or Count Distinct.
- Click on Attribute

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2012.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2012.png)

## 12. **Controlling Table Calculations** 🔺

unlike basic calculations, table calculations are based on the view when it's filter.

They are context sensitive.

They are applied to MEASURES in the view.

Quick table calculation:

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2013.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2013.png)

Table Calculation:

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2014.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2014.png)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2015.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2015.png)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2016.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2016.png)

## 13. **Using Level of Detail Expressions**

As we are more dimensions we make the data more granular or aggregated if we use less dimensions.  

Levels: 

### - Fixed

Locked at some field.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2017.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2017.png)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2018.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2018.png)

Some cases:

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2019.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2019.png)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2020.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2020.png)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2021.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2021.png)

### - Include

### - Exclude

## 14.**Filtering and LOD Expressions**

applied before table calculations.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2022.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2022.png)

## 15. **Using Parameters to Control Data in the View**

First we need to create parameters, then use them and finally show them.

Parameters are global, meaning that are applied for all sheets.

Purpose:

- to adjust calculation
- to control filters

## 16. **Parameters: Swap Measures**

Dynamic Measure selection - to set a single view but with multiple Measures to show.

First we create a parameter, in this case:  *"Parameters to check"*

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2023.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2023.png)

Then we create a calculated Filed:

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2024.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2024.png)

we can also do Dynamic Aggregation following similar flow.

## 17. **Advanced Mapping: Modifying Locations**

to fix gaps in maps or fix data locations in general.

- Edit Errors in Geocode data

    ![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2025.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2025.png)

    Maps > Edit Locations

    ![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2026.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2026.png)

    <More than 1 place has that name. So adjust the geographic role or matching locations>

- Assign Locations to data

    ![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2027.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2027.png)

## 18. **Advanced Mapping: Customizing Tableau’s Geocoding**

we can set manually the latitude and longitude geocode (user-defined)

Typically we use a 2nd data source that contains fields with specific geolocation data and we **blend the data based on common field.**

## 19. **Advanced Mapping: Using a Background Image**

On the Map menu, select Background Images and choose image location+ (Work Data.xls).

In the Background Images dialog box, click Add Image.

Complete the Add Background Image dialog box with these settings: 

Name: Injury Image 

File or URL: click Browse, then navigate to and select X Map Image.gif 

Click Open.

Set the X Field drop-down list to Location X, and enter 0 for Left and 99 for Right. 

Set the Y Field drop-down list to Location Y, and enter 0 for Bottom and 100 for Top. 

Click OK, then click OK again in the Background Images dialog box.

## 20. **Viewing Distributions**

## Histograms

compose of ranges/bins with continuous data.

Select measure and then

- select Using "Show me", a Histogram can be created.

Or we can create manually a bin (right click - create bin)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2028.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2028.png)

          we need to change to a ***Discrete*** Value on the Aggregation Function and a C***ontinuous*** in Bins

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2029.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2029.png)

IF number of bins is 1 , it will include every field value.

## Box and Whisker Plots

Box uses a circle mark type.

In Analytics pane, we can find Box Plot.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2030.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2030.png)

Another way is to use : select *the dimension* and then "*Show ME*"

## 21. **Comparing Measures Against a Goal**

### Bar in Bar chart

to compare two measures.

Drag the 2nd measure into the Axis. 

We use Measure Names(dimension) and Measure Values (which are created automatically).

We move the Measure Names to COLOR → to create stack bars.

To merge and start both from 0 → Go to Analysis → stack bars  → OFF

We can make both bars visible by changing the size → Ctrl + Measure Names→ drag to Size.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2031.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2031.png)

### Building Bullet Graphs

Start by maximum value- > Select a measure to Detail, then:

Add reference line → per cell option (line by default) → sum value→ Sum aggregation type.

Add 2nd reference line → Distribution type → per cell → percentages of sum

Create a Boolean field, and add it to color.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2032.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2032.png)

## 22. **Showing Statistics and Forecasting: Use the Analytics Pane and Trend Lines**

### Trend lines

- To explain relationship between two MEASURES. e.g. Regression or correlation.
- It has 4 types: linear, logaritmic, exponential and polynomial.
- Clicks in Analytics pane > Model > Trend Line. (by default per pane)
- It has a bold-line(the actual trend line) and two lighter lines (referencing the confident).
- Summary in Describe Trend Model

    ![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2033.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2033.png)

- It's good when *High R-squared and a low P-value*

Example:

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2034.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2034.png)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2035.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2035.png)

### Forecast in View

You need:

- One continuous date
- One Measure
- Five data points
- At least two seasons (if required)

Click on Analytics pane > Model > Forecast (drag and drop)

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2036.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2036.png)

Verify the accurate of "prediction interval" of forecasting:

- Select a sheet and Duplicate as cross tab resulting in one listing the actual and other estimated.

## 23. **Advanced Dashboards: Using Design Techniques and Filter Actions**

Make use of four-key steps when planning a dashboard:

1. Determine Purpose and Audience
2. Plan thoroughly
3. Build using design best practices:
    - don't overcrowd it, use story points / coherent subsections
    - Streamline the legend (keep the important ones) and filter (one acting on multiple view or even better use action of parameters to avoid lots of filters.
    - Filters should be on the left.
    - Include instructions.
    - Include meaningfully tooltips, that will improve clarity, consistency, etc.
    - Don't put lots of titles
    - Remove unneeded headers, labels, tick marks.
    - Use muted and contrasting colors. (color blind palette)
    - Font sizes adjustments.
4. Test Dashboard
    - Apply 5 seconds rule.

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2037.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2037.png)

Use a target filter to filter both data sources(1) and regions view(2)

1. Click the Dashboard menu, and then click Actions.
2. In the Actions dialog box, click Add Action, and then Filter. 
3. Fill out the Filter Action dialog box:

     • Name: “Filter Coffee Chain”

     • Source Sheets: Profit Analysis dashboard	

    Region Selection with Run action on: Select

     • Target Sheets: Profit Analysis dashboard

    	Coffee Chain Profit Analysis and Coffee Chain Profit Trend 

     • Clearing the selection will: Show all Values 

4. Under Target Filters, choose Selected Fields, and then click Add Filter. 

    • Source Data Source: Superstore, Field: Region 

    • Target Data Source: Coffee Chain, Field: Market

5. Click OK three times to close the dialog boxes. 
6. Test to make sure the Region Selection filter controls the Coffee Chain views.

Build a view with an arrow to use as a link to another dashboard

![Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2038.png](Tableau%20Desktop%20II%20Intermediate%20ccd451cfee9a44e68a4b3c772ac1c44b/Untitled%2038.png)

1. Click the New Worksheet tab and rename the new worksheet: Navigate 
2. Confirm that the Superstore data source is selected, then click the Analysis menu, and select Create Calculated Field. 
3. Name the calculated field “Navigation” and enter the formula: “Click here to view the Profits by Location dashboard.” NOTE: Include the quotation marks. 
4. Click OK to close the calculation editor. 
5. From Dimensions, drag Navigation to Rows.
6. On the Marks card, change the mark type drop-down menu to Shape.
7. On the Marks card, click Shape and then change the symbol to a filled, right-pointing arrow. 
8. Press CTRL + SHIFT + B a few times to make the cells on the view larger.
9. Right-click the Navigation header, and select Hide Field Labels for Rows.
10. Click the Profit Analysis dashboard tab. Drag the view Navigate to the dashboard to the left of Region Selection.
11. Select the Navigate view, then click its drop-down menu, click Fit, and select Entire View.
12. On the Dashboard menu, click Actions.
13. In the Actions dialog box, click Add Action and then click Filter. 
14. Fill out the dialog box:
    - Name: “Navigate to Profits by Location”
    - Source Sheets: Profit Analysis dashboard	Navigate (Superstore)
    - Run action on: Select
    - Target Sheets: Profits by Location dashboard	(leave all worksheets selected)
    - Clearing the selection will: Leave the filter
15. Click OK twice to close the dialog boxes. 
16. Test the new action to make sure the link works.

## 24. **Telling Stories with Data**

Tableau Stories are created by dragging worksheets and dashboards into the view of each story point and adding descriptive captions on the navigator.

Useful to guide users through data.

It doesn't change the data in worksheets and vice versa(once it is updated - snapshot was captured).

---

---

[Certificate for Desktop II: Intermediate](https://verify.skilljar.com/c/2z6fvf4u34q9)