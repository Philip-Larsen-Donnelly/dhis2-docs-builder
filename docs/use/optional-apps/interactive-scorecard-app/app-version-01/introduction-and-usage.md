# Introduction and Usage

## Scorecard and demo server <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/scorecard-and-demo-server.md -->

### Introduction to scorecard

In public health setting such as Ministries of Health, scorecard offers
a useful and standardized method for analysis with traffic lights color
codes, combining related indicators into one table.

A scorecard can gives an overall view of the performance of a health
program such as a vaccination program, highlighting successes,
weaknesses, and areas for improvement.

There are two ways to create a scorecard: you can use:

  - The Scorecard app, as explained in this guide , or
  - The Pivot Table app, as explained in dhis2 website here:
    https://www.dhis2.org/node/243  

This guide  focuses mainly on the scorecard application, as explained
below; The difference between the two, is that the scorecard app is
tuned for advanced scorecard analysis and is developed and maintained by
HISP Community developers, while the Pivot Table App is for basic
scorecard analysis and is developed and maintained by the Dhis2 core
team.  With both scorecard app and pivot table app, you can download and
use your scorecard offline and share it on the DHIS2 dashboard. With a
scorecard app, you have more advanced control and power to easily create
and analyse multiple elements and dimensions in your data.  Additionally
the scorecard app gives an opportunity to cascade your analysis by
including bottleneck indicators in the scorecard dashboard as well as
analyses your data with broad spectrum of visualization tools, such as
pivot table, charts and maps.

![Standard layout of RMNCAH Scorecard](../content/scorecard/resources/images/image122.png)

![](../content/scorecard/resources/images/image123.png) 

### About demo server and scorecard meta-data

DHIS2 Scorecard team maintains a demonstration server
at [https://scorecard-dev.dhis2.org/demo](https://scorecard-dev.dhis2.org/demo).
This is by far the easiest way to try out Scorecard application in
DHIS2.

#### Using DHIS2 Demo server

To use the scorecard demo server you will have to login into the server,
you can use the login credentials that are displayed on the login page
to login and explore the amazing features of the scorecard app.

#### Scorecard metadata

The Scorecard borrows its meta-data from the general DHIS2 data source
and uses this to create a data store for ease of analysis. Scorecard
metadata such as indicators and indicator groups are managed using the
DHIS2 Indicator maintenance App. The Scorecard App is also integrated
with function maintenance App, used to create custom indicators. Custom
Indicators are indicators whose definition and calculation cannot easily
be created using the Indicator maintenance app in the DHIS2.  

        



## Installing scorecard <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/installing-scorecard.md -->

Scorecard application is completely free and open source, and it is
available on DHIS2 app store (https://play.dhis2.org/appstore), download
the latest scorecard application with long term support.

To install any application into DHIS2, requires superuser privilege,
make sure your account has necessary authorities to install the
application, or contact DHIS2 support team for acquisition of account
with privileges for installation of apps.

> **NOTE**
>
> Interactive scorecard supports all versions of DHIS2 from 2.25 going
upward, It can run in lower versions with limited functionalities and with no
support for fixing any issues.

There are two ways of installing interactive scorecard into your
DHIS2 instance.

### Installation from within DHIS2

This installation approach is the most direct, but only available on
DHIS2 running version 2.28 and above.

Step 1:

Simply open Apps management by clicking on Apps search menu or apps icon
on the top bar to locate Apps Management, click to bring down list of
apps, or search “Apps Management”. Open the Apps management to go to
apps listing See figure below:

![Apps management on search menu](../content/scorecard/resources/images/image125.png)

Step 2:

Once Apps management is open, go to Apps store panel, accessible on the
left navigation menu, a list of online applications for installation
will show up, look for interactive scorecard.

![App store listing, with interactive scorecard](../content/scorecard/resources/images/image124.png)

Once found, click install to install the application. When done
installing, the interactive scorecard will be accessible from the search
menu.

> **NOTE**
>
> This step is only successful is you have an internet connection and your
DHIS2 instance is accessible online.

### Installation from DHIS2 App store website

This approach of installing DHIS2 requires visiting DHIS2 App store
website, downloading a zip file of the latest stable build of scorecard
app, and manually installing it into DHIS2.

This approach is recommended for all DHIS2 instances running on version
2.27 and below.

> **NOTE**
>
> Ensure that you have good and stable internet connection to download the
zip file.

![Apps listing in DHIS2 App Store](../content/scorecard/resources/images/image126.png) 

Step 1: Downloading the compatible version from app store

Once on DHIS2 App store, locate interactive scorecard application, and
click it to get the list of available versions of the scorecard. Pick
the most latest version of the scorecard and download a zip file of the
latest build into your local hard disk.

![List of versions and supported version of DHIS2 ](../content/scorecard/resources/images/image127.png)

> **NOTE**
>
> The zip file name may have cryptic alphanumeric name such as
“3ad63731-a75d-4adb-95a1-4f646e481c20”. You may rename the zip file to
easily locate it in the future, with naming such as “scorecard-v2.x.zip”, where “x” is version number of your build.

Step 2: Uploading the app into Dhis2

Click on Apps search menu or apps icon on the top bar to locate Apps
Management, click to bring down list of apps, or search “Apps
Management”.

![Apps management on search menu](../content/scorecard/resources/images/image125.png)

Open Apps management to see and manage list of installed applications on
DHIS2, Interactive scorecard app can be installed by clicking the upload
icon.

![The upload Icon](../content/scorecard/resources/images/image128.png)

Once installed, interactive scorecard application will be enlisted under
standard apps

![Interactive scorecard on list of installed standard applications](../content/scorecard/resources/images/image129.png)

When done installing, interactive scorecard will be accessible from the
search menu.  If scorecard doesn’t appear on your menu, it may be not
visible for one of the two issues.

### Installation Access credentials/Permissions.

While scorecard application may be installed in your DHIS2 instances,
you may not have necessary permissions to view  it. In such cases
communicate with DHIS2 moderator or DHIS2 support team for the
application to be assigned to one of your user roles.

### Installation not successful.

Scorecard application will not be visible in your application, if it’s
either not yet installed in your DHIS2 instance or installation process
failed for technical reasons.

Most common failure to install, results from misconfiguration of
read/write permissions of the installation folder on the server hosting
dhis2. Misconfiguration of permission can also result from  denial of
ability to delete an installed application.

To resolve this, back-end access of DHIS2 is required, to assign proper
ownership and read-write permission of the folder for holding installed
apps.

> **NOTE**
>
> Location of folder for installed apps varies depending on the version of
DHIS2 Installation.

1.  From version 2.27 going down, the folder for installed apps is
    located in \[DHIS2\_HOME\]/apps
2.  From version 2.28 and above, the folder for installed apps is
    located in \[DHIS2\_HOME\]/files/apps

For more information on how to create and install applications on DHIS2
please visit https://www.dhis2.org/how-to-create-find-install-apps




## Opening and browsing scorecards <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/opening-and-browsing-scorecards.md -->

Scorecard application can be found in  the Apps menu, if scorecard
application is not yet installed in your DHIS2 instance or installation
has issues, refer to the installation instruction (Chapter 2) of this
documentation for further guidance.

### Opening of scorecard application

Open scorecard by locating it in Apps search menu or apps icon on the
top bar, click to bring down list of apps, or search “scorecard”.

![Scorecard application on apps menu.](../content/scorecard/resources/images/image112.png)

Once open, scorecard application will bring list of created scorecards,
or when no scorecard exists, a step by step instruction on how to create
scorecard.

> **NOTE**
>
> If scorecard application is taking too long to load, and you’re not on a
slow network, make sure you have cleared your browser cache.

Scorecard makes good use of cached files for better offline experience,
as a result, when installing higher version, scorecard may use older
version of cached files and thus break down while loading.

![](../content/scorecard/resources/images/image113.png) 

Figure 3.1-B: Scorecard application in a continuous state of loading.

### Clearing application cache

Approaches to clear application cache and browser interface, vary from
browser to browser, but the common standard keyboard shortcut for all
browsers is “CTRL+SHIFT+DELETE”.

Accessing interface for clearing browser cache can be done via the
following approaches:

  - Google chrome: Go to the menu icon on the top right corner, and
    click it to open, go to more tools menu, and choose “Clear browsing
    data”. Once interface is open, Make sure  “Clear the following items
    from” is set to “The beginning of time”.  
  - Mozilla Firefox: Go to the menu icon on the top right corner, and
    click it to open, go to  Library, and go to History, and choose
    “Clear recent history”. Once interface is open, Make sure “Time
    range to clear” is set to “Everything”, and “Details” option is
    expanded to show all details options.  Once on the clear browsing
    data or recent history, tick “Cache”, “Cookies”, “Hosted app data”
    or “Offline Website data”. To clear all cached files, cookies and
    locally stored data by scorecard.

 ![Menu icons in Google chrome and firefox  ](../content/scorecard/resources/images/image114.png)

> **NOTE**
>
> These will also clear all cache information and cookies from other
websites you’ve visited in your browser.

![Google chrome interface for clearing browser cache](../content/scorecard/resources/images/image115.png)

![Mozilla firefox interface for clearing browser cache](../content/scorecard/resources/images/image116.png)

### Browsing the  scorecard application

Once a scorecard application is open, it will display a list of all
scorecards the user has permission to access. Items are by default
displayed with list view, showing three items at a time, with pagination
to access more scorecards. All scorecards are sorted by names in
ascending order.

To locate scorecard, use the search panel to search by name or
description of the scorecard, search will locate all favorites user have
access to and list them sorted in ascending order.

![Default list view of scorecard application](../content/scorecard/resources/images/image117.png)

### Display/Listing of scorecards

There are three standard types of scorecard listings to allow navigation
and traversing through long list of scorecards

#### List view

This is the default listing scorecard, displaying three items per page,
while providing pagination options to move between pages.

![List view of scorecard application](../content/scorecard/resources/images/image118.png)


#### Card view

This displays all scorecards without paginations in multiple rows with
two columns throughout, allowing vertical navigation of scorecards.

![Card view of scorecard application](../content/scorecard/resources/images/image119.png)

#### Thumbnail view

This displays all scorecards without pagination in multiple rows with
one column throughout, allowing more detailed view of each single
scorecard.

![Thumbnail view of scorecard application](../content/scorecard/resources/images/image10.png)

To visualize data with scorecard, click a particular scorecard of
interest. For more information on all functionalities available for
navigating scorecard, visit the “Analysis with scorecard” section of the
documentation.




## Analysis with scorecard <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/analysis-with-scorecard.md -->

Once the scorecard is open, you can analyze the data visualized by the
scorecard through different dimensions using various components offered
by the scorecard app.

### Navigating the scorecard

For analysis purposes the scorecard app allows you to

  - Switch between organization units and period types
  - Switch between layouts on the fly
  - Show and Hide some components and data
  - Print and Download scorecard
  - Sort by data values in ascending and descending orders
  - Performing Trend and Bottleneck analysis

All explained in this chapter.

### Drill down analysis

Scorecards support drill down analysis from scorecard rows, where row
headers can be clicked to reveal lower level of analysis. By default
scorecard lists organization units in rows and data in columns, thus
default drill down analysis accessible to user is by organization units.

Data in columns can be moved to rows with drag and drop layout change,
thus supporting drag and drop on indicators in rows, where organization
units will be moved to columns.

> **NOTE**
>
> Drill down on indicators is only supported for indicators with related
indicators assigned to them.

#### Drill down analysis by Organization units

In order to drill down across organization unit levels just click the
name of the children organization level and the scorecard of the
particular organization unit will appear under the row of that
organization.

![Drill down  analysis by orgunit](../content/scorecard/resources/images/image11.png)

#### Drill down analysis by Data

In order to drill down across data, indicators names/headings needs to
be on the rows of the scorecard, this can be achieved by drag and drop
of indicators heading from columns to rows and clicking of row
headers(indicator names) to drill down.

Among use cases of drill down analysis by indicators includes mapping of
performance from bottleneck chart to scorecard.

![Mapping of performance indicators from bottleneck chart to scorecard](../content/scorecard/resources/images/image12.png)

Only indicators with related indicators will support drill down
analysis, thus only indicators with related indicator analysis icon will
have drill down capability showing the related indicators on lower
level, if any of the lower level indicators also have related indicators
assigned to them, drill down can proceed further down.

With utilization of scorecard layout change feature (see scorecard
layouts chapter) and support related indicator analysis through related
indicators analysis by individual indicator selections , When  viewing
the scorecard at a parent level, you can drill down to see scorecard of
children levels.

![Drill down  analysis by indicators](../content/scorecard/resources/images/image13.png)

### Organization unit selection

The Scorecard app allows you to make organization unit selections based
on groups, levels and user organization units, these are known as
selection modes.

All organization unit selections types begin with clicking the select
option button that displays the selected organization unit. Then click
the branching icon.

![ Selection of orgunits](../content/scorecard/resources/images/image14.png)

#### Selection by levels

From the selection mode dropdown menu click “Select Level” then navigate
to the button on the right that reads “Select Organization Unit Levels”,
from the dropdown list of Levels, you can then make your selections by
clicking the desired levels to view on your scorecard.

![ Selection of org units by levels](../content/scorecard/resources/images/image15.png)

#### Selection by groups

From the dropdown menu that appears click “Select Group” then navigate
to the button on the right that reads “Select Organization Units Group”,
from the dropdown list of Groups, you can then make your selections by
clicking the desired groups to view on your scorecard.

![ Selection of org unit  by groups](../content/scorecard/resources/images/image16.png)

#### Selection by user organization unit

From the dropdown menu that appears click “Select Organization Unit”
then navigate to the button on the right that reads “Select Organization
Unit”, from the dropdown list, you can then make your selections with
respect to your organization by clicking the desired option unit to view
on your scorecard.

![ Selection of org units by user orgunit](../content/scorecard/resources/images/image17.png)

### Period selection

The scorecard app allows you to make period selections for fixed
periods, relative periods and extended relative periods.

All period selections types begin with clicking the select option button
that displays the starting period. Then clicking on the period type
select option button which lists all the period types.

![ Period selection](../content/scorecard/resources/images/image18.png)

#### Fixed period selections

To select fixed periods, start by selecting a period type from the
period type list. You can then select periods from the list of available
periods.

![Fixed period selections](../content/scorecard/resources/images/image1.png)

#### Relative period selections

To select relative periods start by selecting a period type from the
period type list. You can then select periods from the list of available
periods.

![Relative period selections](../content/scorecard/resources/images/image2.png)

#### Extended relative periods

Extended relative periods are relative periods that do not ship out with
the dhis2 by default. These extended relative periods include : Quarters
this year, Quarters last year, Months this year and Months last year.

To select extended relative periods start by selecting a period type
from the period type list. You can then select the extended relative
periods from the list of available periods.

![ Extended relative periods](../content/scorecard/resources/images/image3.png)


## Scorecard layouts, headers and legends <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/scorecard-layouts-headers-and-legends.md -->

### Layout change with drag-n-drop

When viewing the scorecard you can change layout by simply clicking at
column labels(text), and dragging it to a row heading.

This also works when dragging a row heading to a column heading.

![Layout before change of rows to columns with drag and drop](../content/scorecard/resources/images/image4.png)

> **NOTE**
>
> Dashed lines indicate the drag n drop zones.

![Layout after change of rows to columns with drag and drop](../content/scorecard/resources/images/image6.png)

### Scorecard header

The scorecard header appears on the top of scorecard. To create custom
header and add additional branding, see chapter 9.2.1 “Branding
scorecard header”.

The scorecard header is by default composed with the Scorecard Title,
the selected Organization Unit(s) and the selected period(s)

![The scorecard header](../content/scorecard/resources/images/image7.png)

> **NOTE**
>
> Scorecard header can be branded from basic text with bold, color and
font type, to full blown customized header with national flags, pictures
and other branding supported with HTML5.

### Scorecard legend

The scorecard legend is displayed under the scorecard header. By default
all scorecard will start with legend displayed.

The scorecard legend gives meaning on the colors displayed on the
scorecard visualization.

![The scorecard legend](../content/scorecard/resources/images/image9.png)

> **NOTE**
>
> Gray color for Not Applicable (N/A) is used when values falls out of
range of the minimum and maximum of existing color code classes.

White color code is used when there’s no value (returned results are
empty/null not zero)

![](../content/scorecard/resources/images/image38.png) Important

Error loading data is among the errors that can be notified on the
legend, this error can happen when viewing a scorecard which any the
data selection made has been deleted in the system. Thus it should be
noted that the scorecard app requires data selections that exist in the
dhis2 system and deleting data selection involved in scorecards shall
lead to an error.

### Column headers, hints and tool-tips

Column headers appear on top of every column. By default, a column
header is the conventional name of the particular data selection.

##![](../content/scorecard/resources/images/image40.jpg)

Figure 5.4-A: The column header of a scorecard with hints.

> **NOTE**
>
> The most common errors are internal server errors or failed network
operations while loading data, oftenly abbreviated with error codes
(409, 404, 502, etc..). Check with your system administrator on
indicators and the server setup to resolve the errors.

Tooltips appear when you hover on the cells that have deviated from the
previous period selection. The tooltip will brief on the previous value,
the deviation and the minimum value that makes a deviation count as
significant.

##![A tooltip on a cell of a scorecard.](../content/scorecard/resources/images/image42.png)




## Additional options <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/additional-options.md -->

Scorecard application allows user to Customize the look of scorecard.
add numbering, ranking, hide/show legend, average column and row.

Scorecard options can be modified in the viewing or the creation
interfaces by clicking the “Options” button.

Options are divided in three sections: Show/Hide, Best/Worst and
Average.

![The available settings that can be regulated from within the options menu](../content/scorecard/resources/images/image43.png)

> **NOTE**
>
> To keep options permanently visible, click on the options button, this
will keep options menu permanently accessible for changes, click again
on options to close it when leaving the menu.

### Hide/show legend

To show the legend, make sure the Legend checkbox is checked.

To hide the legend, make sure the Legend option is unchecked.  

![](../content/scorecard/resources/images/image46.jpg)

Figure 6.1-A: The legend displaying on top of the scorecard

### Hide/show item number

To show the item number, make sure the Item Number checkbox is checked.

To hide the item number, make sure the Item Number option is unchecked.
 

![The Item Number column displaying on the scorecard](../content/scorecard/resources/images/image48.png)

> **NOTE**
>
> Item number is always ascending following the current column used for
sorting, which will contain up/down arrow indicating column used for
sorting in ascending/descending order

 

### Hide/show empty rows

To show empty rows, make sure the Empty Rows checkbox is checked.

![](../content/scorecard/resources/images/image49.jpg)

Figure 6.3-A: Scorecard with empty row on organization units

To hide the empty rows, make sure the Empty Rows option is unchecked.  

![](../content/scorecard/resources/images/image36.jpg)

Figure 6.3-B: Scorecard with hidden empty rows

### Hide/show average row/column

To show average row or average column, make sure the Average Column or
Average Row checkbox, respectively is checked.

![The average column displaying on the scorecard](../content/scorecard/resources/images/image22.png)

To hide average row or average column, make sure the Average Column or
Average Row checkbox, respectively is unchecked.

> **NOTE**
>
> Average columns may not always make sense depending on set of indicators
under display, it only make sense mostly when values are of the same
nature or range, e.g. percentage or client counts.

### Hide/show below/above average

To show below average or above average performance, make sure the below
average or the above average checkbox, respectively is checked.

To hide below average or above average performance, make sure the below
average or the above average checkbox, respectively is unchecked.

![A scorecard displaying rows that have performed above average](../content/scorecard/resources/images/image25.png)

> **NOTE**
>
> The Average values used is by default to sort scorecard rows for
hiding/showing above and below average are based on column used for
sorting(sorted column), if sorted column is organization unit, average
column is used.

### Show top ten/five/three

To show top ten/five or three performance, make sure the ten/five or
three checkbox, respectively is checked.

To hide top ten/five or three performance, make sure the below average
or the above average checkbox, respectively is unchecked.

![A scorecard displaying the top five performing organization units](../content/scorecard/resources/images/image28.png)

> **NOTE**
>
> Top ten/five/three is based on sorted column, which by default is
organization unit column.

### Download Scorecard

You can download the scorecard in excel format by clicking, the “Excel”
button. This shall download the scorecard in csv format and you can
perform any desired operations on an excel file handling application
offline. The “excel” button can be spotted on top of the scorecard
header next to the edit button.

![A collapsed excel button for downloading.](../content/scorecard/resources/images/image31.png)

![An expanded download to excel button.](../content/scorecard/resources/images/image33.png)

### Print Scorecard

To print the scorecard simply click the Print button.

![A collapsed print button.](../content/scorecard/resources/images/image34.png)

![An expanded print button.](../content/scorecard/resources/images/image20.png)

![Downloading a scorecard.](../content/scorecard/resources/images/image21.png)

> **NOTE**
>
> To hide headers and footer containing page url or page name, and get
colored PDF document.
>
>  - On Chrome browsers, Expand “More settings” and untick headers and
>    footer,  choose destination printer to “Save as PDF” to download
>    colored PDF document.
>  - On Firefox, open “Options” tab and set header and footer to
>    “--blank--”, choose destination printer to “Print to file” to
>    download colored PDF document.





## Context menu <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/context-menu.md -->

The scorecard app offers two types of context menu for quick access of
additional features and scorecard capabilities. The two context menu
includes:

1.  Column context menu (accessible via headers)
2.  Cell context menu (accessible via cells)

The column context menu can be accessed by right clicking on a column
header, and a cell context menu can be accessed by right clicking on a
particular cell.

![The column context menu when viewing a scorecard](../content/scorecard/resources/images/image78.png)

### Further analysis by entire column

From the Column context menu, clicking “Further Analysis” opens a modal
with a pivot table visualizing the data of the column.

![A modal with a pivot table visualizing the data of the column](../content/scorecard/resources/images/image79.png)

Navigation within the further analysis modal is explained in Chapter 8.

> **NOTE**
>
> Further analysis by entire column uses entire selections in rows, by
default selection in rows are organization units.

### Sort asc/desc by column

From the Column context menu, clicking “Sort Asc” will sort the data
with respect to the ascending order of the column content and an arrow
pointing downwards shall display next to the column name to signify that
the values decrease going down the column.

Similarly, clicking the “Sort Desc” will sort the data with respect to
the descending order of the column content and an arrow pointing upwards
shall display next to the column name to signify that the values
increase going down the column.

![Sorting by ascending order of the second column](../content/scorecard/resources/images/image82.jpg)

### Best/worst by columns (top 10,5,3)

From the Column context menu, you can view the Best performers by
choosing Top 3,5,10.

Similarly, you can view the Worst Performers by choosing Last 3,5,10.

![A scorecard displaying the top three performing organization units](../content/scorecard/resources/images/image84.png)

### Hide/show column

To Hide a column, simply right click on the column head and click Hide.

![Hiding a column by using the column context menu](../content/scorecard/resources/images/image86.png)

If there are any hidden columns, to show them right click on the column
head and the context menu will have have a “show all” option.

![Showing all columns of a scorecard.](../content/scorecard/resources/images/image87.png)

### Further Analysis by cell

From the cell context menu, clicking “Further Analysis” opens a modal
with a pivot table visualizing the data of the cell.

![The column context menu when viewing a scorecard](../content/scorecard/resources/images/image73.png)

### Trend analysis by cell

On the cell context menu, you can analysis the trend of the data for the
last 3,6,12 months, last 4 quarters or the last 5 years by clicking
trend analysis and picking a period of interest.

![Trend analysis for PCV 3rd dose coverage(%) for the last 12 months visualized as an area chart](../content/scorecard/resources/images/image74.png)

### Related Indicators analysis by cell

From the cell context menu, if an indicator has related indicators then
you will see an option that allows you to perform related
indicators analysis. Further explanation on related indicators analysis
can be found in Chapter 12.




## Further analysis <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/further-analysis.md -->

As hinted earlier the further analysis menu can be access via the
context menu. This chapter explains deeply on the operation that can be
performed in the further analysis module. 

### Related indicators analysis

On the Interactive Scorecard if a data selection support related
indicators analysis and option to perform related indicator analysis
will be visible when performing further analysis. Clicking the Related
indicator analysis button will display a chart of the indicators related
to the data selections.

To show chart labels click on the chart labels checkbox which appears
below the period selection box.

![Related indicators analysis of the ANC 1-3 Drop out rate; for ANC Coverage from 1st visit to 4th visit](../content/scorecard/resources/images/image75.png)

Related indicators analysis charts can be downloaded. For more
information about downloading and printing charts on the scorecard app
refer to chapter 8.6.3.

> **CAUTION**
>
> Related indicators currently only support single period selection, as
with multiple period selection, indicator relation lose its meaning for
its use cases.

### Pivot table analysis

Pivot table further analysis, visualizes the data in tabular manner. You
can switch between organization unit and periods but also you can change
the table layout.

![Pivot table analysis on the ANC 1 Coverage column](../content/scorecard/resources/images/image61.png)

### Chart analysis

Chart further analysis, visualizes the data in graphical manner. You can
switch between organization units and periods but also you can change
the chart layout and switch between various chart types (i.e. bar chart,
stacked bar chart, line chart etc.).

![Chart analysis on the ANC 1 Coverage column using the combined chart analysis](../content/scorecard/resources/images/image63.png)

### Map analysis

Map further analysis, visualizes the data on map. You can switch between
organization unit and periods but also you can switch between various
base maps  that your data would be drawn on base layer. Currently
supported base layers includes Map surfer, OSM Dark, Topography Maps,
Earth Imagery,OSM Black and White, OSM Hot and Stamen Toner.

![Map analysis on the ANC 1 Coverage column  using topographic base map](../content/scorecard/resources/images/image65.png)

### Data dictionary

When performing further analysis, you can open the data dictionary for
the data selection item of the column/cell by clicking the info button.

![Information of the data selection item of the column/cell on the data dictionary](../content/scorecard/resources/images/image67.png)

### Operations on Further analysis

You can perform more operations within the further analysis module, such
as downloading scorecard, printing it or switching of layout.

#### Layout selection

On further analysis you can change layout for pivot table by drag-n-drop
across filters, row dimensions, and column dimensions.

Similarly, you can change layout for chart by drag-n-drop across
filters, category (y-axis content), and series (the x-axis content)
dimensions.

![Panel for switching the further analysis pivot table layouts across filters, column and row dimensions (dragging data selections from row dimensions to column dimensions)](../content/scorecard/resources/images/image68.png)

![Layout panel with data selections on column dimensions](../content/scorecard/resources/images/image70.png)

#### Downloading data of the pivot table further analysis

You can download the column or cell data observed during further
analysis by pivot table into excel format by clicking, the “Excel”
button located on the bottom of the further analysis button. This shall
download the data in csv format and you can perform any desired
operations on an excel file handling application offline.

![Excel download button that can be found on the bottom of the further analysis modal](../content/scorecard/resources/images/image53.png)

![Downloading pivot table data into csv format.](../content/scorecard/resources/images/image55.png)

#### Downloading and printing of chart on further analysis

To print or download the further analysis chart, clicking on the chart
context menu this will give options for downloading the further analysis
chart.

To download just pick a file format of interest and click on it to
initiate download.

To print simply click the word “Print”.

![Print preview of Scorecard as PDF](../content/scorecard/resources/images/image56.jpg)

> **NOTE**
>
> To hide headers and footer containing page url or page name, and get
colored PDF document.
>
>  - On Chrome browsers, Expand “More settings” and untick headers and
>    footer,  choose destination printer to “Save as PDF” to download
>    colored PDF document.
>  - On Firefox, open “Options” tab and set header and footer to
>    “--blank--”, choose destination printer to “Print to file” to
>    download colored PDF document.



## Creating and managing scorecard <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/creating-and-managing-scorecard.md -->

Scorecard can be created via creation interface, which is accessible to
“create” button on the top right corner while on home/listing page.

Click “create”, to open scorecard creation interface. If not on home
page, to access create button from any page, go back to home/listing
page.

![Interface for creating scorecard](../content/scorecard/resources/images/image98.png)

Once on the scorecard creation interface, scorecard can be created
quickly in three simple steps

1.  Labeling and branding of scorecard  

2.  Selecting data for the scorecard  

3.  Managing layout and saving  

### Labeling/Branding scorecard

Labeling of scorecard involves and branding involves filling in three
main fields.

  - Name, used for future search  
  - Description, used for detailed/deep search  
  - Custom header, for branding by placing banner on top of scorecard

#### Labeling of scorecard

Start by labeling scorecard with name and description, that can be done
by entering title and description of scorecard on the middle left side
of the scorecard. Title and description of scorecard are mandatory
fields to allow proper description of scorecard as well as allowing
search in the future.  

![](../content/scorecard/resources/images/image100.png) 

Figure 9.1.1-A: Section for labeling of scorecard with name and
description.

> **NOTE**
>
> Scorecard can not be saved without name and description filled in.

 

#### Branding of scorecard

Branding of scorecard is optional, by default scorecard uses name as
heading of the scorecard, which will be displayed on top of scorecard,
custom header field is available to allow more advanced customization
and tailoring of scorecard.

Custom header, uses what you see is what you get(WYSIWYG) interface to
allow complex designs of headers supporting formatting of texts,
alignments and insertion of images.

To edit custom header, locate “customize header” button, on the top
center of the scorecard, where header of scorecard will be displayed.

![Button for customizing of scorecard header with WYSIWYG](../content/scorecard/resources/images/image103.png)

![Customizing Scorecard header with WYSIWYG editor.](../content/scorecard/resources/images/image104.png)

### Choosing your data selections

To choose type of data in your scorecard simply locate the section next
to title and description for selecting type of metadata, choosing group
and picking metadata of interest.

Select all indicators/data elements/reporting rates/program
indicators/event data items/ custom functions of your choices, to insert
them in scorecard columns.

Selection of score-card is simplified, what you see is what you get
interface, with real-time simulation of scorecard layout.

Basic selection operations includes:

  - Select an item to add it, or un-select to remove if from scorecard
    columns  
  - Drag and drop an item from the data selection to scorecard columns
    to add  
  - Click trash/delete icon on “Cell customization” area to remove it
    from scorecard columns  

![Data selections for scorecard](../content/scorecard/resources/images/image105.png)

Scorecard supports all data selections available in analytics
applications, and supports more, such as custom functions. Among the
supported metadata selections includes:

  - Indicator selection, selection of indicators is done by available
    groups  
  - Data element selection, selection of data elements is done by
    available groups  
  - Data Sets selection, selections in data sets includes, Reporting
    rates, Reporting rates on  time, Actual reports submitted, Actual
    reports submitted on time, Expected reports  
  - Program indicator selections, selection of program indicators is
    done by available  programs  
  - Event data items, selection of data items is done by available
    programs  
  - Custom functions, selection of custom functions is done by available
    functions  

#### Standard analytics data selections  

Standard analytics data selections are the selections available by
default on all DHIS2 analytics tools, such as pivot table, visualizer
and GIS. These includes indicators, data elements, data set, program
indicators and event data items. All standard data sections, depend on
the data sources, thus possible period selections for given data
selections should always be taken into consideration

> **NOTE**
>
> Selection of data items who’s reporting frequency is smaller than
default period selection of the scorecard will cause the given
indicators to always return empty(e.g. Monthly scorecard will always
return empty on indicators from quarterly data source) 

#### Functions selections

Functions selections are extended analytics calculations supporting a
more open-ended logic of computation, such as logical operations,
predictors and other complex analytics use cases.  To create functions
to work with scorecard download, download function maintenance
application from this link:
[https://play.dhis2.org/appstore/app/dXX2Fk6jwCX](https://play.dhis2.org/appstore/app/dXX2Fk6jwCX) 
Functions makes use of pure good old JavaScript(vanilla JavaScript)
logic to do calculations purely on the browser, without the need for
server, this is accomplished by execution of JavaScript codes that
expects period and data selections and return standard DHIS2 analytics
results.  

Functions comprises of three key building blocks

1.  Input/Selection parameters. Function expects standard DHIS2 periods
    and organization units selections.  
2.  Computation logic. This is an open-ended workspace for writing of
    calculation logic to work on given period and organization unit
    selections, computation logic is usually classified into rules
    dimensions, thus allowing one function to support different use
    cases by defining multiple rules that will control the computation
    logic. Possibilities are limitless, among major operations done
    includes

    1.  Fetching data from aggregate and event analytics and modifying
        results with custom logic, and reformat the results back in standard
        analytics format.  
    2.  Fetching data from existing sql Views, performing custom logics and
        formatting results in standard analytics format  
    3.  Fetching data from other DHIS2 API endpoints(such as data-value and
        events api) and other data sources(including external sources),
        performing custom logic and formatting results in standard analytics
        format.  


3.  Output/Returned analytics. This is the end-result output from
    functions, formatted in standard analytics format, to allow
    compatibility with standard DHIS2 analytics applications.

To support open-ended support for any level of complexity, function
maintenance application has been developed, to allow any developer with
basic JavaScript knowledge to quickly develop custom calculations either
not supported natively by DHIS2 or to allow developer to work-around
limitations or miscalculations from standard analytics.

Main requirements for developing functions includes:

  - Basic web programming knowledge with JavaScript (jQuery is an
    advantage)  
  - Understanding of DHIS2 Web API and analytics  
  - A working installation of Functions maintenance application. When a
    function maintenance application is installed for the first time, it
    creates five standard functions  with generic use cases as example
    functions to allow reuse of codes to create other functions.  The
    auto created functions will also be listed in functions selection
    list.

> **NOTE**
>
> The six generic functions that comes standard with functions
maintenance, are auto generated if no function exists in the system.

### Managing layouts and saving  

Once done with scorecard data selection process, a list of all
selections will be appearing as columns on the scorecard layout area.
Scorecard will be in its most basic layout, and is ready to be saved.
Among the layout standards observations includes:  

  - All columns are grouped in single default group. Group label for
    default single group is not displayed for simplicity.  
  - Values, colors and arrows for each column are auto-generated. Values
    are auto generated to provide real-time what you see is what you get
    (WYSIWYG).  
  - Column labels picks default name of the selected metadata, labels
    can be changed, see section “Customization of cells” section of this
    documentation.  

![Standard layout of scorecard, with what you see is what you get interface](../content/scorecard/resources/images/image111.png)

#### Changing layout of scorecard

To change scorecard layouts, simply click on column labels(text), to
select column to move, then simply drag and drop that column to a new
position

![Rearranging column order of a scorecard by drag and drop](../content/scorecard/resources/images/image110.png)


> **NOTE**
>
> Click area for drag and drop feature is only active with the text inside
the header field, clicking outside the text doesn’t activate the click
area.



## Customizations and editing of scorecard <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/customizations-and-editing-of-scorecard.md -->

You customize scorecard via the create/edit interface. Customization
involves giving scorecard custom headers, grouping cells, setting up the
starting period and organization unit of scorecard, setting access
privilege to users and groups, adding custom labels and legend colors.

### Access sharing settings

The scorecard give user to set sharing who has access to their scorecard
and the privilege (view only/edit) to the particular group of people
that the share with.

Scorecard sharing can be done through the access sharing select option
box, by clicking an image representing a privilege for a group of
interest.

When a privilege has been chosen for a group the color of the icon of
the privilege will change to blue.

![Access sharing privilege setting settings across user groups](../content/scorecard/resources/images/image109.png)

> **CAUTION**
>
> Sharing settings from 2.28 going back is only implemented on the
interface, access control is not strictly enforced, it is for simplicity
in management of scorecards only.

> **NOTE**
>
> User groups appearing on the access sharing list should exist in the
user groups that are were created in the “Users” app.

### Startup period and organization unit selection

To set the startup period selection, head over to the period type select
option button and click it, this lists all the period types, from which
you can select the desired period type and then add the period range
from the available list into the selected list.

In order to set the startup organization unit selection, head over to
the organization unit select option button and click it, this lists the
organization units in hierarchical order.

More details on how to select the org units can be found under
Organisation unit selection in the Analysis with the scorecard chapter.

![Selection of the startup period](../content/scorecard/resources/images/image108.png)

![Selection of the startup organisation unit](../content/scorecard/resources/images/image107.png)

### Grouping of cells in scorecard

Grouping of cells in scorecard can achieved in two steps.

  - Creation of a group

To create a group click the word “Add” will appear on the rightmost
column and a new group will be created.

You can give the group a name by editing the words “New Group”

![“Add” Icons that enable user to create a new group and data selections to the group](../content/scorecard/resources/images/image92.png)             

![Placeholder (default name) of new group can be replaced with a desired group name](../content/scorecard/resources/images/image91.png)

  - Adding data selections into the group

To add data selections into a group, make sure the group has been
selected (has a gray background/fill color) then follow the procedures
to make data selection as explained under Choosing your data selections
in Chapter 9. 

To delete a cell grouping just click the trash icon next to the group
name. 

### Customization of cells

The scorecard app, gives user the ability to customize cells by giving
them the tools that enable them to choose:

  - whether to display the color legends
  - what colors to display on the scorecard and their cut point values
  - the effective gap
  - what labels display on the columns (headings of data selections)

![Cell Customization section on the scorecard app](../content/scorecard/resources/images/image89.png)

#### Column & cell labels

The scorecard app allows the user to customize the column/cell labels.

By default, the column label is the name of the data selection. To
customize the column label, edit the value on the box adjacent to the
words “Label”

![Column and cell labels text box](../content/scorecard/resources/images/image90.png)

#### Cell Effective(Minimum) gap

To set the effective gap value of increase/decrease write the number in
the input box adjacent to the words “effective gap” and save changes.

![Cell Effective (Minimum) gap text box](../content/scorecard/resources/images/image90.png)

#### Cell cut-of points range

To set the effective cell cut-of points range for a data selection
(column), edit the min – max values under the legend information of the
data selection.

![Cell cut-of points range](../content/scorecard/resources/images/image89.png)

> **NOTE**
>
> Minimum of upper class should be equal to the maximum of lower class, no
gap should be left between classes, to leave open ended upper limit for
topmost class and lower limit for lowest class use dash “-”. The
classification of values between intervals behaves as follow:
  - Lowest and middle classes, values limit range from lower limit
    inclusive, to upper limit exclusive(excluding upper limit itself,
    i.e. value equal to upper limit will be accounted in next upper
    class)
  - Highest class, values limit range from both lower and upper limit
    inclusive(i.e. values of both lower and upper limit will be
    accounted in the same class, upper limit won’t be excluded)

The ranges are automatically generated evenly between 1 and 100 range,
divided by total number of classes(default is three).

#### Display effective gap arrows

To display effective gap arrows of increase/decrease make sure the
checkbox adjacent to the “Display arrows” label is ticked. To hide
effective gap arrows simply make sure the check box is unticked.

![Opting to show effective gap arrows](../content/scorecard/resources/images/image90.png)

#### Show legend colors

To show legend colors make sure the checkbox adjacent to the “Show
Colors” label is ticked. To hide Legend colors simply make sure the
check box is unticked.

![Opting to show the legend colors](../content/scorecard/resources/images/image89.png)

### Stack two cells in single column

To pair two cells in one single column, add one of the data items of
interest scorecard in, click it and make sure it is grayed (to indicate
that it is the active data selection), then on data selection area
navigate to the second data item of interest and right click on it and
select pair with current.

![Clicking “Pair With Current” stacks the active data selection to the new data selection](../content/scorecard/resources/images/image88.png)

![Column stacking demonstration with the PHU delivery rate (by ANC1) against the PHU delivery rate (by expected pregnancies)](../content/scorecard/resources/images/image106.png)

> **NOTE**
>
> Pairing of indicator is useful when presenting two indicators measuring
same goal(e.g. ANC 4th visit coverage by 1st visit and ANC 4th visit by
total population of women of childbearing age), or placing many
indicators in single page(e.g. A4 paper comfortably fits around 15
columns on portrait, thus with stacking can fit up-to 30 indicators)

### Color codes for cut-off points

The scorecard application allows you to customize the color code for
cut-off points by changing the existing color codes or by creating new
color codes and defining their range.

To change an existing color code, navigate to the legend definition
section, click on the color of interest and pick another color from
color picker.

![The legend definition section with a list of color codes.](../content/scorecard/resources/images/image99.png)

![To change color code of an existing legend color.](../content/scorecard/resources/images/image97.png)

![To change the value of the cut-off points for a color code.](../content/scorecard/resources/images/image102.png)

To add a new color code definition, navigate to the the “New legend”
section. To define color of legend  click button on the left and pick
color  from the color picker.

> **WARNING**
>
> Adding new color definition resets all defined value ranges for all
indicators back to default range(i.e. ranging from 1 - 100 divided
evenly by new number of classes). Always revisit all indicators after
adding/removing classes to update new class ranges based on new classes.

### Additional labels

The scorecard app allows the user to add additional labels that will
appear under the organization unit. Such labels can be used for variety
of purposes, common usage includes

  - Source of indicator

![The additional labels section showing a listing of the additional labels](../content/scorecard/resources/images/image94.png)

![The Added Additional labels appearing on the scorecard.](../content/scorecard/resources/images/image93.png)



## Related Indicators Analysis in DHIS2 <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/related-indicators-analysis-in-dhis2.md -->

This chapter focuses on utilization of scorecard indicators to perform
related indicators analysis, related indicators analysis can be used for
a wide range of use cases, among them being causality analysis( also
referred to as the bottleneck analysis).

While this documentation will delve into the use case of related
indicators for bottleneck analysis, this chapter shall introduce you to
the basics of bottleneck analysis and how to use the related indicators
feature for any suitable/relevant use case.

Bottleneck analysis is a systematic way to look at the main determinants
of effective coverage for selected interventions to identify problem
areas and purposely act on them

There are six coverage determinants, from supply to demand side that
analyze where health system bottlenecks exist. A bottleneck is a loss of
system efficiency

![The six coverage determinants, from supply to demand side which analyze where health system bottlenecks exist](../content/scorecard/resources/images/image96.png)

The combination of bottlenecks identified  determines the quality, and
hence the effectiveness, of coverage in any given setting.

### Measuring Determinants

Among the modifications made on the efforts to adapt the Tanahashi
approach for use in Marginal Budgeting for Bottlenecks tool in the 21st
Century include focusing determinants of effective coverage.

Each determinant was analogous to a Tanahashi stage that leads towards
the goal of effective coverage. In addition, ‘availability’ was divided
into two determinants: availability of commodities and

availability of human resources

Ultimately the combination of bottlenecks identified  determines the
quality, and hence the effectiveness, of coverage in any given setting.

This modified model was easier for practitioners to use since it
reflected the types of data that were available and permitted the
identification of bottlenecks through a step-wise approach that
evaluates six determinants of the effectiveness of coverage of an
intervention:

1. Availability of essential health commodities

2. Availability of human resources

3. Accessibility of distribution points for the interventions

4. Initial utilization of interventions

5. Continuity/completeness in the continuous utilization of interventions

6. Quality of interventions delivered.

The first three determinants focus mainly on supply side constraints,
while the final three focus largely on demand side barriers.

![Block diagram grouping the Measuring Determinants in three categories and detailing the relationship between the six determinants of the effectiveness](../content/scorecard/resources/images/image95.png)

While there are many national policies and guidelines for effective
interventions to reduce maternal and child mortality, these
interventions do not always reach those who need them most due to
bottlenecks within and outside the health system.

The scorecard app allows for the user to add related indicators to an
indicator so that they may inspect the impact of the relating indicators
by further analysis. The next subchapter explains how the use can do
this.

![A bar graph of bottlenecks identification.](../content/scorecard/resources/images/image66.png)

### Related indicators

In scorecard related indicators are associated with scorecard
indicators, and can be added to scorecard indicators on the indicator
cell customization area. Related indicators are used sometimes as
minimal drop in support for bottleneck analysis.

The relations between indicators in scorecard and indicators for
analysis are initiated in the edit interface.

> **NOTE**
>
> Related indicators like scorecard indicators, can be any existing
metadata in DHIS2, from data elements, indicators, reporting rates,
program indicators, event data items as well as functions. If required
metadata is missing it has to be created

To add related indicators to a data selection, click the data selection
and navigate to the column customization section and click on the
Related indicators button

![Selection of related indicators](../content/scorecard/resources/images/image69.jpg)

Related indicators in chart visualization, can be implemented in two
simple visualizations, this includes

1.  Multiple indicators per determinant, using determinant as a group,
    with indicators names for each bar and determinant name as group in
    the chart x-axis.
2.  Individual indicator per determinant, where one determinant have one
    indicator

#### Individual indicator selections

For individual indicator selection in related indicators for scorecard,
If the related indicators belong to a group of the same context, then
they can be added as individual indicators.

![Making selections of related indicators on the data selection section](../content/scorecard/resources/images/image60.png)

In related indicators analysis, where each determinant have single
indicator for measurement, individual indicator selection is the best
choice for data analysis.

Among use cases of individual indicator selection includes causality
analysis across six measurement determinants to assess potential
fluctuation of trends across determinants (notice each determinant have
one indicator used).

![Causality analysis fluctuation of trends across the six measurement determinants](../content/scorecard/resources/images/image58.png)

To add individual related indicator selections, click “Use Individual
Items” and make your data selections.

When a selection is made a card will appear to right with the name of
the Indicator, the display name, baseline and target. Also a real-time
related indicators chart shall be displayed on the bottom.

Display Name, Baseline and target can be edited.

![Selection of individual indicator selections together with a real-time related indicators chart](../content/scorecard/resources/images/image64.png)

#### Grouped indicator selections

For  grouped indicator selection, If the related indicators belong to
different groups, then they should be added as group indicators.

In related indicator analysis, where one determinant can have multiple
indicators, grouped indicator selection is the best choice for analysis,
where determinants can be created as groups and indicators can be
inserted to given determinants.

##### Managing groups

To add group related indicator selections, click “Use Groups”. There are
to ways of creating grouped indicators :

  - Generating groups
  - Manually creating group

For grouped indicator analysis following standard built-in determinants,
determinant groups can be auto-generated by clicking “Generate Groups”
button which will generate determinant groups ready for inserting
indicator per each determinant.

![The generate groups button](../content/scorecard/resources/images/image62.png)

To create a group manually, click the “Add Group” button

![The add group button](../content/scorecard/resources/images/image54.png)

To make data selections to the groups, first click the group click on
the group name the click the data selection of interest on the data
selections section.

![A group of related indicators](../content/scorecard/resources/images/image52.png)

You can sort/rearrange indicators within a group by dragging them from
their current position to a destination position.

![Sorting of indicators by dragging and drop](../content/scorecard/resources/images/image57.png)

To delete data selections click the trash icon on the Group Title then
click the tick icon.

![The trash icon](../content/scorecard/resources/images/image83.png)
![To complete the delete action click the tick icon](../content/scorecard/resources/images/image81.png)

> **CAUTION**
>
> The deleting process is irreversible and deleting a group will delete
all the data selections that have been made to the group of the group as
well.

##### Managing labels of grouped indicators

When a selection is made a card will appear to right within its group
with the name of the Indicator, the display name, baseline and target.
Display Name, Baseline and target can be edited.

![Editing labels of an indicator](../content/scorecard/resources/images/image85.png)

##### Color coding indicator by their groups

The related indicator groups are color coded so as the user can easily
distinguish between indicators of different groups. The color codes can
also be changed by simply clicking the color bar above the group name
input box, and selecting a color of interest.

![Selection of color scheme for indicator selections that belong to a group](../content/scorecard/resources/images/image77.png)

##### Real-Time Related Indicators Chart

When a selection is made a real-time sample related indicators chart
shall be displayed on the bottom of the section.

![Selection of grouped indicator selections together with a real-time related indicators chart](../content/scorecard/resources/images/image76.png)

### Action tracker on Bottleneck analysis

#### Introduction

The Action Tracker is a mechanism through which decision makers and
actors track progress in implementing priority interventions designed to
address root causes of bottlenecks in RMNCH performance at different
levels of the health system from national, regional, district and
sub-district level. The action tracker represents an important tool for
documenting and assessing progress towards implementation of locally
owned and led solutions to RMNCH performance issue.

The action tracker is part of coverage, and bottleneck analysis that
utilizes DHIS2’s analytical features to track and assess national and
sub-national level performance for purposes of improving health service
delivery.

#### How to track action in DHIS2

Performance on interventions is reviewed through Quarterly District
Review Meetings (QDRM), mid-term or annual programme reviews to assess
progress, identify bottlenecks, their causes and suggest possible
solutions/actions to address gaps at district, health sub-district and
facility levels.

To ensure effective and efficient service delivery, these
actions/solutions are monitored/tracked on a routine basis, and
designated persons within the District Health Management Team (DHMT)
provide updates/progress on prospective actions.  Routine monitoring of
actions/solutions to bottlenecks on various interventions is done in
consultation with other District Health Teams (DHT) and other national
and development stakeholders. Once actions are agreed upon,
documentation and reporting follows which can be done either using the
DHIS2 system or district activity monitoring log books.

#### How to setup event capture for action tracking

The current setup in the DHIS2 is based on a demo concept planned to be
progressively improved to create linkages with scorecards and related
indicators analysis features. The tool is currently implemented as a
single event without registration using DHIS2 event capture tools. The
demo App is setup on the scorecard-dev instance at
https://scorecard-dev.dhis2.org with the username and password provided
on the login page

#### How to use event capture for data entry of action tracker

##### Browsing event capture

To browse the action tracker demo app, access the scorecard-dev instance
with your login, at the main menu page, search for “Event capture”

![How to browse event capture](../content/scorecard/resources/images/image80.png)

Using the event capture app;

1.  Use the organizational unit tree to drill down to district level
2.  You will notice that selection in the registering window changes to
    the selected organization unit
3.  If there are more than one program, use the drop down window to
    select the preferred program

    ![Listing showing tracked action with event capture](../content/scorecard/resources/images/image35.png)

4.  Click on the register button to begin
5.  Select the “Report date” window to begin entering data

##### Data entry with Action tracker

Data entry in the action tracker is based on identified bottlenecks in
health service delivery at sub-national level, their root causes and
planned actions. The bottlenecks are classified using Tanahashi’s six
determinants of coverage. To begin data entry;

![](../content/scorecard/resources/images/image72.png)

1.  Select the category of the issue identified and the root causes
2.  State if any reviews have been done regarding the issue, progress
    and the responsible persons to follow-up
3.  Click on the “Save and Add New” buttons to save the issue for
    follow-up

    ![](../content/scorecard/resources/images/image71.png)

4.  Click on the “Cancel” button to return to the list of bottlenecks
    and actions.  

##### Data Review and editing

Using the Event capture app, data on the bottlenecks, root causes and
actions can be reviewed, printed and edited. This is important
especially during follow-up on progress of actions as stated and
discussed in previous sub-national level review meetings.

![](../content/scorecard/resources/images/image35.png)

To edit a record,

1.  Click on the record to access the record edit menu

    ![](../content/scorecard/resources/images/image29.png)

2.  The data will open in an edit window, edit the record by stating the
    actions taken to avert bottleneck, also state the progress

    ![](../content/scorecard/resources/images/image27.png)

3.  Click on the “Update” button to save the changes

    ![](../content/scorecard/resources/images/image32.png)



## Scorecard and bottleneck analysis implementation <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/scorecard-and-bottleneck-analysis-implementation.md -->

This chapter provides high level guidance for implementation of
scorecard and Bottleneck Analysis (BNA) who audience include District
Health Management Teams (DHMT), Ministry of Health (MoH), Implementing
and Development Partners in health.  This text aims to guide any country
or organization using DHIS2 for their aggregate reporting at multiple
levels of the system and also implementing individual records using
event capture, action tracker and Dhis2 tracker capture App. This guide
takes into consideration that DHIS2 has been customized to support
reporting requirements and the need to further analyze data using a
scorecard and Bottleneck analysis tools, as well as provide
opportunities for enhanced use of data to improve programs supported by
the scorecard and BNA tools/frameworks.  


### Overview

Effective and timely use of HMIS data by managers at all levels of
health system is critical to inform and improve health service delivery.
 HMIS dashboards have the potential to enhance the use of data for
decision making and planning, by displaying information for managers in
an accessible and actionable manner. Managers who have competing demands
and limited time, resources and training to conduct data analysis, are
often left to organize HMIS data themselves, making HMIS a less
user-friendly and effective tool than it might be otherwise.  

Building data visualization features that reflect a systematic theory of
change / workflow within the DHIS2 software allows end users to
effectively use data for action. Scorecards and Bottleneck analysis
dashboards in DHIS2 help users to produce meaningful visualizations to
identify low performing districts, monitor high impact interventions
that are lagging behind and pinpoint  bottlenecks to effective health
service delivery including identification of  root causes and solutions,
with the aim of guiding operational planning, tracking progress and
performance over time and strengthening accountability for better
results.  

The scorecard was initially introduced by ALMA (Africa Leaders Malaria
Alliance) as a monitoring and accountability tool to boost malaria
control efforts and track progress against malaria indicators. A number
of countries adopted the tool at country level to implement the RMNCAH
(Reproductive, Maternal, Newborn, Child and Adolescent Health) scorecard
to enhance accountability and transparency. However inadequate linkages
with the HIS (timely data availability) caused delays on effective
program monitoring.  

The innovation here is the integration of the scorecard functionalities
within DHIS2 through a specialized dashboard that not only helps to
track progress but also provides tools to perform in-depth analysis, to
identify causes of lack of performance in order to drive actions.

### Planning implementation of scorecard and bottleneck analysis

#### Defining strategy

The scorecard is an effective tool to enhance accountability and track
progress and actions towards health and nutrition outcomes. The
scorecard uses tracer indicators for reproductive, maternal, newborn,
child and adolescent health interventions to monitor progress national
and global targets. It displays data on table using different color
coding (green to red) and arrows to show the direction of progress over
the monitoring period (quarter, semester or annual). The scorecard
alerts program managers and decision makers to be aware of areas which
continuously record low performance and lack of progress as well as
those needing more attention and actions.  

![Example of standard scorecard for RMNCAH.](../content/scorecard/resources/images/image30.png)


The bottleneck analysis consists of a structured analysis of the
determinants of coverage for key reproductive, maternal, newborn, child
and adolescent health interventions. It’s based on Tanahashi’s Health
Service Coverage Evaluation methodology \[Tanahashi, T. “Health Service
Coverage and its Evaluation.” Bulletin of the World Health Organization.
56: (2): 295-305. 1978\], which examines supply, demand and quality
determinants that contribute to effective intervention coverage. The
analysis looks at six determinants of coverage across the supply, demand
and quality determinant categories which include:

1.  Availability of Essential Commodities
2.  Availability of Trained Human Resources
3.  Geographic Access
4.  Initial Utilization
5.  Continuous Utilization
6.  Effective Coverage

It aims at understanding root causes of weak effective coverage by
analyzing supply and demand side indicators to identify obstacles or
bottlenecks hindering high effective coverage. Specific strategies and
actions could be taken to address the causes in order to mitigate or
remove bottlenecks. Below and illustration graphic showing bottleneck
analysis using the interactive scorecard.

![Example of Bottleneck analysis using ANC 4th visit coverage](../content/scorecard/resources/images/image23.png)


#### Identify stakeholders and motivations

It’s good to take a look at the main motivations of the stakeholders and
how to mitigate risks resulting from potential diverging interests.

  - Central MoH Departments such as M\&E & Planning often are the main
    stakeholders for standardisation and specification of indicators and
    IT Systems
  - Central IT departments have a general interest over (often locally
    controlled) technology choices and ownership, hardware and software
    purchases. They are often dealing with network and hardware issues
    but lack experience dealing with complex web-based architectures and
    data exchanges.
  - Specialized disease programs are often under pressure to deliver
    very program specific indicators, both for their own management but
    also responding to donor driven approaches. They may also feel more
    comfortable controlling their proper IT system to be sure their
    needs are prioritized.
  - Specialized functional areas (such as Human Resources, Logistics,
    Hospital Management) are often in a sandwich position, having to
    cater to the information needs of several different stakeholders,
    while trying to achieve operational efficiency with limited
    resources.

By identifying who is interested to provide or utilize the data, the
lead implementers can start to form a project team to inform the design
and implementation. One method for characterizing stakeholders involves
grouping interested parties by their functional roles.

#### Opportunities and challenges

Key to the successful implementation of the scorecards and Bottleneck
analysis is a buy-in from national and subnational level stakeholders
including ALMA that has been very instrumental in the support and
implementation of the RMNCAH scorecard. At the Ministry of health,
consensus needs to be reached on who will monitor and follow-up the
implementation. At the district level, the DHT (District Health Team)
and other facility and community level staff need to be included in the
implementation process.  

Scorecard and Bottleneck analysis implementation need to make use of
existing national infrastructure and performance management systems.
Countries where DHIS2 is being used for reporting national health
indicators find this process a bit easier for implementing scorecards
because most of the indicators required for scorecards are already
captured /collected and aggregated in the HMIS.  

Existing challenges,  for example data availability in existing DHIS2
system, follow-up on routine district review meetings to address
bottlenecks and corresponding actions, may hamper analysis and use of
the scorecards and Bottleneck analysis tools. These challenges would
have to be addressed in an inclusive rather than exclusive process.
Other challenges including availability of infrastructure and support at
district  level need to be addressed by putting in place mechanisms that
ensure sustainability of the process.

#### Organization and stakeholder considerations

Engaging stakeholders as part of the implementation process creates a
dynamic team that ensures the support for the scorecards and bottleneck
analysis. Identifying  teams to support the different components of
implementations both technical and policy is key to this process.

### Identify user and system specifications

Identify the different thematic areas for the different scorecards, this
should be guided by the different health programs in a country or
project. Reproductive Health , Maternal, Neonatal and Child Health,
etc.. could have different indicators and scorecards. Additionally
specifying the frequency of reporting, the lowest level of data analysis
should also be specified. This may also be determined by the DHIS2
reporting frequencies implemented by the existing national or parallel
system.

#### Defining interventions

Identification and inclusion of interventions into a scorecard should be
aligned with national priorities, as reflected in national plans and
strategies.  In practice RMNCAH indicators cover the full continuum
care.

Country experiences have shown that effective selection of indicators is
guided by an inclusive process involving all stakeholders in addition to
the ability of the HMIS to capture the most relevant indicators for
program monitoring.

Experience has shown that an average of 20 tracers indicators is a best
balance to keep the scorecard manageable.

It’s important to set up a core working team to oversee the whole
process and decide on indicators. This core team should encompass all
those directly concerned on program implementation and monitoring.

#### Identify Data sets and data elements

The core team will ensure that the national database contains required
data elements for program monitoring. It should be part of their role to
decide on the revision of HMIS data collection tools in order to reflect
program management needs.

#### Indicator selection and definitions

  - Constitute a technical team to define indicators for key
    interventions for the scorecard (definitions, numerators and
    denominators including source - data elements) including potential
    indicator categories such as Maternal and Newborn Health, Child
    Health, Nutrition, health Systems, etc.
  - For each intervention to include on the scorecard, identify and
    define related  determinants of coverage indicators for supply,
    demand and quality using the determinants framework (refer to annex
    1). These indicators will constitute the cornerstone of the
    Bottleneck analysis.
  - Document and map selected indicators with data elements/program
    indicators (See annex I)
  - Customize both scorecard and Bottleneck analysis indicators in
    DHIS2; defining indicators types, numerators and denominators.

> **NOTE**
>
> Most of the Bottleneck analysis indicators
may not be reported in DHIS2 such as commodities and human resources so
integration and interoperability between systems may be required, refer
chapter 12.4 for more details on interoperability considerations.

#### Document user stories

Collecting user stories from the national and subnational level plays a
key role in documenting and deciding workflow processes for scorecards
and BNA.

This process may include the DHT and other facility and community level
staff directly responsible for implementing and monitoring health
interventions.

Documenting the process of data collection, aggregation and analysis,
will help to streamline implementation of scorecards and BNA.

### Consideration for integration and interoperability

In many countries a national HMIS is often the first system to be rolled
out to a large number of facilities and to manage a large number of data
on a monthly or quarterly basis. When countries start to develop their
health system architecture further, DHIS2 often will be connected to
some other systems. This connection is done directly through a simple
script, which automates a data transfer.  

We talk of a 1:1 connection because it is limited to two systems. In the
case of an LMIS/HMIS integration, one LMIS (e.g. openLMIS as is the case
in Tanzania) will transfer data to DHIS2 as defined in the script. In
case a second logistics system would want to transfer data to DHIS2
(e.g. commodity data for a specific disease program), a second script
would have to written, to perform this task. These two scripts would
then run independently from another, resulting in two separate 1:1
connections.  

This hands-on approach often represents a first step and is one of the
most common use cases on the way to an interoperable openHIE
architecture.  

DHIS2 can assume different roles in interoperability scenarios. A common
interoperability scenarios is for DHIS2 to receive aggregate data from
an operational system, in which case the operational system adds up the
transactions before passing it on to DHIS2. However, DHIS2 may to a
certain extent also be configured to store detailed transactional data,
receiving it from external systems or through direct data entry in
DHIS2.  

On this basis we try making a comparative overview, comparing aggregate
DHIS2 data management with data management of external specialized
system. This can serve as a rough orientation, but is not static since
both the capabilities of DHIS2 and its interpretation by implementers
are broadening with almost each release.

|Area|Aggregate DHIS2|External specialized systems|
|--- |--- |--- |
|Logistics|Aggregate data, e.g. end-of-month facility stock levels can be send through DHIS2. DHIS2 can produce simple stock level and consumption reports.|Supply chain management systems can track detailed stock movements (receiving, return, transfer, destruction) and record details such as production batch numbers. At HQ level, SCM systems typically create forecasting, replenishment and elaborate control reports.|
|Finance|Aggregate data, e.g. on total expenditure or cash level can be send through DHIS2. DHIS2 can produce simple finance overview reports, e.g. on remaining budgets.|Finance management systems allow fully traceable recording of financial transactions according to legal requirements, including budgeting, transfers, cancellations, reimbursements etc. Multi-dimensional tagging of transactions allows for analytical reports.|
|Patient tracking|Disease or program related data are collected by DHIS2, DHIS2 Tracker also allows a simplified longitudinal view on medical records, including patient history and multi-stage clinical pathways.|Specialized hospital management systems can cover and optimize complex workflows between different departments (e.g. reception, payment counter, wards, OPD, IPD, laboratory, imaging, storeroom, finance and HR administration, medical device maintenance, etc.).|
|Human Resource|Human resource related indicators are collected through dhis2, for example planned positions and vacancies per facility.|A specialized HR management system can track detailed status information and changes for a Health Worker (accreditation, promotion, sabbatical, change of position, change of location, additional training, etc.). It comes with pre-designed reports for both operational oversight and planning.|

#### Steps for successful data and system integration

The purpose of this chapter is to provide a methodology for implementers
to create and support a DHIS2 integration scenario.  The guide is based
on the best practices and lessons learned form field experiences.  The
guide advocates for a country driven, iterative, and agile approach that
begins with collecting user stories and functional requirements.  

The guide is intended as a framework that can be adapted to the specific
context of each country. The content describes specific examples for
each step detailing user stories, data specifications, job aids and
checklists to guide the use of the reference implementation software.
The implementation process includes the following steps:

Step 1: Identify Stakeholders and Motivations for Improved Facility Data

Step 2: Document Facility Registry Specifications and User Stories

Step 3: Set Up Initial Instance

Step 4: Identify Gaps & Iterative Development via User Testing

Step 5: Scaling the Registry Implementation

Step 6: Provide Ongoing Support

|Step 1|Step 2|Step 3|Step 4|Step 5|Step 6|
|--- |--- |--- |--- |--- |--- |
|![](../content/scorecard/resources/images/image26.png)|![](../content/scorecard/resources/images/image24.png)|![](../content/scorecard/resources/images/image19.png)|![](../content/scorecard/resources/images/image51.png)|![](../content/scorecard/resources/images/image50.png)|![](../content/scorecard/resources/images/image44.png)|
|Stakeholders & Motivations|Document Specifications|Set Up Initial Instance|Iteration and Testing|Scale the Implementation|Ongoing Support|


> **NOTE**
>
> Integration between DHIS2 and other systems
may range from automated to manual and regular import of data from other
systems to DHIS2. More information on interoperability can be found from
DHIS2 Implementer’s guide, see
[https://www.dhis2.org/documentation](https://www.dhis2.org/documentation).
Also support on can also be acquired from DHIS2 Expert community. For
DHIS2 Experts near your region See expert list
[https://www.dhis2.org/expert-community](https://www.dhis2.org/expert-community).

#### Training and roll out of scorecard and Bottleneck analysis in DHIS2

Quite often training  and rolling out of the scorecard and BNA dashboard
in DHIS2 requires prior knowledge and skill in using DHIS2 tools. The
DHIS2 community has instituted an online training program
(http://academy.dhis2.org/) that builds the capacity and skills of all
users interested in the DHIS2. The online training program focuses on
basic functionality of DHIS2, which is a prerequisite to maximise the
benefits of using scorecards and BNA dashboards in DHIS2.  

The training needs may vary depending on the scope of the program
(Reproductive Health, Maternal Health, Neonatal and Child health) and or
implementation at various levels. For national programs, it is important
to first conduct a Training of Trainers (ToT) that will support the
implementation at lower levels. Individual organisations can focus on
training departments or program representatives who would in turn train
and support lower level units. Below are some considerations for
training and rollout;

1.  Selecting the team for training: team selection is critical to the
    proper use of scorecards and BNA dashboards. Program managers, M\&E
    experts, HIS analysts as well as data managers  should ensure to
    take part in training.
2.  Determining an appropriate training Schedule (See Annex II): Given
    the busy schedule of most implementers, it is important to select a
    date and venue that is suitable  for all participants. The training
    program should cover the topic of discussion comprehensively
    addressing general overview of the DHIS2, visualization tools as
    well as the scorecard and bottleneck analysis.
3.  Choosing to conduct short trainings (one day) has also proven
    advantageous given the busy schedule of most implementers.  
4.  Ensure that the training program is designed in such a way that
    sessions are practical and interactive to foster learning
5.  Participants must each have  functional laptop / desktop computer to
    enable access to practical sessions
6.  Provide adequate infrastructure for the training sessions including
    good accessibility to Internet,  Clear projector, ample spacing and
    any printed material for the training should be clear and visible.
7.  Allow short breaks within training sessions, to encourage
    participants to refresh and concentrate on the topic of discussion  
8.  At the end of each session, ensure to allow for discussion address
    any outstanding questions
9.  Provide feedback to participants at the end of training. This
    creates assurance that the participants expectations have been
    addressed and provide a way forward for any pending issues
10. Plan to follow up participants and provide support on areas that may
    not have been clarified during the training session.

### Factors for scale up

Beginning with a pilot is often good as it provides guidance on areas
that need most attention. Piloting provides cost estimates that can be
used for scaleup projections. Below some factors to consider for scaling
up implementation of the scorecards and bottleneck analysis;

1.  Availability of technical support: The scorecard and BNA are
    currently supported by UiO/HISP nodes in east africa. This support
    is critical to build local capacity for Scorecard and BNA
    customization, maintenance, and quality assurance
2.  Development of user friendly tools e.g. RMNCAH scorecard/s triggered
    national interest, leading to greater use of DHIS2 at district and
    national levels
3.  Bottleneck and causal analysis are useful for evidence based
    planning and can be used as a tool for resource mobilization
4.  Community engagements should be aligned to already existing
    community structures to ensure sustainability
5.  Political and technical district leadership is necessary to
    influence real change in the communities
6.  Aligning programs initiatives to the already existing national
    planning cycles and systems the planning process. This will

    1.  Foster Government buy in
    2.  Build local ownership
    3.  Lower costs of implementation.




## Help, tour guide & translation <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/help-tour-guide-translation.md -->

The scorecard offers a quick guidance to get the user started off with
using making use of the basic features of the app, user documentation
can be accessed from within the app as will be explained in this
chapter.

![Options available on clicking of the help button](../content/scorecard/resources/images/image47.png)

### Tour guide

To get a brief tour of navigation across the scorecard app simply click
the Help icon and choose “Take a tour” and a floating pop-up will appear
hinting on some basic navigation that user can use to analyze with
scorecard.

![The sample of a tour guide floating pop up showing where the user can make their organization unit selections](../content/scorecard/resources/images/image45.png)

### Help and documentation

The documentation of the scorecard app is accessible through clicking
the “User Manual” from the Help dropdown menu. This will open the
documentation of the scorecard app.

### Translations

The scorecard app offers basic translation for up to three languages,
French, Portuguese and English.

By default, the app opens up with English Language.

To change Language to French, click Fr.

To change Language to Portuguese, click Pt.




## Scorecard community and use cases <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/scorecard-community-and-use-cases.md -->

Scorecard development and implementation is community driven by HISP
Nodes and UNICEF Globally. As it is an open source software, it’s source
codes are available on github (https://github.com/hisptz/scorecard) for
contribution.

Contributions on scorecard community can be on the following areas:

1.  Development and Testing of scorecard application
2.  Documentation and translation of scorecard application
3.  Implementation of scorecard and experience sharing with community

### How to be part of the community

Scorecard development and implementation is a DHIS2 Community driven
development and implementation initiative comprising of collaborative
support of developers, implementers and translators from HISP Nodes,
Governments and Organizations using DHIS2. The best way to join the
DHIS2 Community is to sign up on the community of Practice.


<!-- PALD: this needs to be updated  -->
1.  If you are interested in the usage, setup or implementation of
    Scorecard you can sign up for [Dhis2 Jira](https://jira.dhis2.org/).
2.  If you have questions about or want to follow the development
    process you can sign up for the [Dhis2 Community of Practice](https://community.dhis2.org/).

Don't hesitate to get in touch if you are interested in using
Interactive scorecard for your organisation or government. We can be
reached through the contact details below. For technical questions or
questions related to scorecard implementation please sign up and use the
mailing lists as described above.

Email

  - HISP Tanzania <info@hisptanzania.org>
  - HISP Uganda <info@hispuganda.org>
  - DHIS2 - <post@dhis2.org>
  - DHIS2 Academies - <post@dhis2.org>
  - The DHIS2 Online Academy - <onlineacademy@dhis2.org>

Websites

[https://hisptanzania.org/](https://hisptanzania.org/)

[http://www.hispuganda.org/](http://www.hispuganda.org/)

[https://dhis2.org/](https://dhis2.org/)

### Development and implementation

Interactive scorecard uses [JIRA](https://jira.dhis2.org/) for
issue tracking. You can use it to report bugs and request new features.
You can search for features to get an overview of which features make it
into each release.

### Documentation and Translations

<!-- PALD: this needs to be updated  -->
The Scorecard app documentation is available in google docs from here
[https://goo.gl/miojZ4](https://goo.gl/miojZ4).
You can recommend your changes by commenting on the topic of interest in
the document and share back your copy with tracked changes.

The Scorecard user interface is translated to a range of languages
including English, French and  Portuguese. Efforts for improving the
existing translations or adding new languages are much appreciated.

The easiest approach to translation is to download the google doc,
revise the existing translations and share the translated copy with
tracked changes to <info@hisptanzania.org>. You can use the same email
to request scorecard build with your translations reflected.

### Data use academy scorecard setup and use cases

#### Rationale for adding scorecard app in data use academy

Scorecard has been added as one of the suite of analytics application in
DHIS2 array of analytics use cases, to enrich data use experience of
DHIS2 implementers.

The African Leaders Malaria Alliance is a groundbreaking coalition of 49
AFRICAN HEADS OF STATE AND GOVERNMENT working across country and
regional borders to eliminate malaria by 2030. They are leveraging
collective knowledge and influence to bring about action and
accountability as they fight one of their continent’s most devastating
diseases by:

  - Providing a forum to review progress and address challenges in
    meeting the malaria targets;
  - Implementing a monitoring and accountability system through the ALMA
    Scorecard for Accountability and Action to track results, identify
    bottlenecks, and facilitate appropriate action; and
  - Identifying and sharing lessons learned for effective implementation
    of national programs

Never before have African leaders come together in this way to solve a
crisis assailing our entire continent. The collaborative strategy has
proven itself to be an effective model for sustainable change as we
continue to engage new stakeholders, deepen relationships with key
decision makers, and work with ministers, NGOs, the private sector, and
other partners to maximize the value and impact of our work.

The overall objective of this the scorecard Info use academy is to
demonstrate how to analyze data using a scorecard using the scorecard.
Further the sessions:-

  - Demonstrates best practices of scorecard use
  - Explains the different features of the scorecard
  - Step by step use of scorecard

#### Topics covered in dhis2 academy

Scorecard utilises training land setup with select few set of indicators
based on global RMNCH use cases to allow implementers to get first hand
experience of scorecard use cases and how it can be used as a powerful
real time tool for data use discussion, bottleneck analysis as well as
formulation of action and tracking of progress.

  - Launching and navigating the Scorecard app.
  - Different features of the scorecard.
  - Analyzing data using a scorecard
  - Explaining the different functions in the scorecard app
  - Downloading scorecard (excel and pdf)
  - Creating a new scorecard
  - Adding BNA indicators to scorecard

#### Training materials and servers being used

The training materials used follow the standard DHIS2 Academy trainers
guides and in this case “Demo - Using a Scorecard.” The session follows
the standard Academy training approach with 1) a live demo session where
the trainer demonstrate and explain the features, and 2) a hands-­on
session with exercises where participants get to practice what they have
learned.

### Existing DHIS2 Scorecard app use cases

Countries and institution are slowly adopting use of interactive
scorecard application to leverage simplicity of scorecard creation
process as well as interactive user experience during analysis, among
the major functionalities cited as handy features that triggers adoption
of scorecard application uses includes:

1.  Ability to drill down and up the organization unit hierarchy, will
    supporting all possible organisation unit selections
2.  Ability to navigate scorecard across time as well as presentation of
    data with more than one period selection
3.  Ability to perform further analysis with charts, table and maps, as
    well as indicator dictionary overview on numerator and denominator
    definitions, calculations, data sources and related aspects of data
    quality such as deadlines of data sources.

Below are select few interactive scorecard application use cases across
various country implementation use cases.

#### Tanzania's RMNCAH Scorecard

The Tanzania RMNCH scorecard was first produced using the African
Leaders Malaria Alliance (ALMA) RMNCH scorecard tool from January 2014
to June 2016; and from July 2016 to December 2016 the RMNCH scorecard is
being produced using the HMIS/DHIS2 RMNCH scorecard tool.

The Ministry of Health, Community Development, Gender, Elderly and
Children with technical support from the University of Dar es salaam is
now utilizing generic scorecard tool to support customization of the
Ministry’s scorecards with focus on revised RMNCH scorecard.

Among goals of moving to utilizing generic scorecard includes:

  - To fast track the scorecard generation, dissemination and use cycles
    and thereby introduce room for more data use, transparency and
    accountability at all levels (Council, Region, National) during all
    cycles of the scorecard generation.
  - Addition of supports of generic functionalities such as drill down
    on organization units, navigation across period and further analysis
    supported by generic scorecard.
  - Facilitate the ministry’s initiative of generating scorecards for
    different types of health sector interventions within HMIS/DHIS2.

![RMNCAH Scorecard adopted from ALMA’s RMNCAH scorecard](../content/scorecard/resources/images/image39.png)

The above scorecard have been implemented utilizing all possible
functionalities such as presentation of twin and related indicators
under single column. More initiative expected to support incorporation
of impact indicators presented separately on scorecard header
originating from census and surveys opposed to the majority of routine
data source indicators enlisted in scorecard rows.

#### Tanzania's PMTCT Scorecard

The Ministry of Health and Social Welfare (MOHSW) through Prevention of
Mother to Child Transmission of HIV program (PMTCT) in its efforts to
improve PMTCT services at all levels, initiated development of PMTCT
scorecard with technical support from University of Dar es salaam. This
initiative aimed at improving quality of PMTCT services to active data
use with scorecard.

PMTCT scorecard contained 10 cascade indicators measuring PMTCT
interventions with the following rationales:

1.  To assess HIV Testing coverage among Pregnant women receiving ANC
    services at RCH
2.  To assess proportion of registered HIV positive women on ART.
    (Applicable for baseline values)
3.  Measure PMTCT retention and infant testing coverage
4.  Measures early MTCT, indicates effectiveness of PMTCT in the
    pregnancy period
5.  Coverage of testing at the end of breastfeeding
6.  To assess Impact of interventions up to the end of breastfeeding
7.  Measures overall MTCT rate up to the period of cessation of exposure
    to HIV virus through Breastfeeding

![PMTCT Scorecard measuring cascade indicators](../content/scorecard/resources/images/image37.png)

#### Tanzania's QIP Scorecard

The Ministry of Health and Social Welfare (MOHSW) through Quality
assurance division aims at improving quality of service provision at
health facilities through assessment of four domain areas of service
provisions.

Among the key objectives of Quality Improvement plan (QIP) scorecard
includes:

  - Creation of transparent mechanism for tracking implementation of
    formulated quality improvement plans across four quarters for each
    annual assessment.
  - Systematically identify facilities areas of implementation
    challenges and gaps for re-strategizing and reprioritization of
    plans
  - Provide appropriate suggesting improvement steps to effectively
    implement formulated quality improvement plans

QIP Scorecard presents facility performance based on most recent
facility assessment or routine follow up information about.

![QIP Scorecard for measuring quality improvement on gaps](../content/scorecard/resources/images/image41.png)

#### Uganda's RMNCH Scorecard

In November 2013, Uganda launched a Renewed, Sharpened and first
Integrated Reproductive, Maternal, Newborn and Child Health (RMNCH) plan
with clear goal, objectives, priorities and 5 strategic shifts in order
to employ new ways of combating RMNCH challenges. The plan aims to
accelerate reduction in maternal, newborn and child mortality and
improve on Uganda’s RMNCH indicators. In order, to track progress
against the ambitious goals and targets, a deliberate effort to track
performance must be invested.

Therefore, the endeavor of developing and implementing the Uganda RMNCH
Scorecard is in line with global initiatives including A Promise Renewed
(APR), UN Commission on Information and Accountability among others.
Under the APR initiative, the Ministry of Health progressively
institutionalizes a national and sub national RMNCH scorecard based on
routine Health Management Information System (HMIS) data and the
District Health Information System (DHIS2) platform.. The scorecard is
also aimed to facilitate health facilities to review their performance
within the quality improvement framework.

![Ugandan RMNCAH Scorecard](../content/scorecard/resources/images/image30.png)


## Annex <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/annex.md -->

### Annex I: Uganda RMNCH Scorecard Indicators and Definitions

Revised after Discussion with the Planning Unit at the Ministry of
Health


|Lifecycle stage|Indicators|Definition/ description|Data source|Assumption(s)|Numerator/ Denominator||
|--- |--- |--- |--- |--- |--- |--- |
|Pregnancy|% of  1st ANC visit within the 1st trimester|This is the percentage of all expected pregnancies in a given catchment population in a given period of time who have attended  their 1st ANC visit within the first trimester|HMIS||Numerator: #of pregnant Women attending 1st ANC visit within 1st trimester<br><br>Denominator: All expected pregnancies|Numerator: HMIS<br><br>Denominator: HMIS 107: 3.3C<br><br>National target = 45%<br><br>Color Coding:<br>>45% = green<br>35%-45% = yellow<br>< 35% = red|

### Annex II: Scorecard and BNA indicators

![](../content/scorecard/resources/images/image8.png)

### Annex III: Scorecard and BNA Training Program

|Time|Agenda|
|------------------ |--------------------------------------- |
|8:45 - 9:00 am|Registration|
|9:00 - 9:30 am|Introduction to DHIS2|
|9:30 - 10:00 am|HMIS 105: Data Elements versus Indicators|
|10:00 - 10:15 am|SHORT BREAK|
|10:15 - 11:00 am|How to use the Dashboards for your Programme - Interactive Session|
|11:00 - 11:30 am|Introduction to Pivot Tables|
|11:30 - 1:00 pm|Pivot Table Interactive Session - Designing Dashboards|
|1:00 - 2:00 pm|LUNCH|
|2:00 - 2:30 pm|Introduction to Data Visualization Tools|
|2:30 - 3:15 pm|Data Visualization Interactive Session - Designing Dashboards|
|3:15 - 3:30 pm|SHORT BREAK|
|3:30 - 4:00 pm|Introduction to Scorecards and BNA|
|4:00 - 4:45 pm|Scorecard Interactive Session - Designing Dashboards|
|4:45 - 5:00 pm|Wrap up and Conclusion|



## Bibliography <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/scorecard/bibliography.md -->

### References

 Tanahashi, T. “Health Service Coverage and its Evaluation.” Bulletin of
the World Health Organization. 56: (2): 295-305. 1978

