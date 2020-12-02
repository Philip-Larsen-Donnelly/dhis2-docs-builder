# Introduction and Usage

## Bottleneck Analysis Dashboard and Demo server <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/bna/bottleneck-analysis-dashboard-and-demo-server.md -->

### Introduction to the BNA App

Bottleneck analysis (BNA) is a structured analysis of the determinants
of coverage for a wide range of interventions delivered through the
health sector, useful to supporting targeted operational planning. It is
a systematic, outcome-based approach to equitable health programming and
real-time monitoring that strengthens the health system, complementing
and building on what exists.

The BNA App is developed and maintained by the HISP Community (UiO,
HISP-Tanzania and HISP Uganda) in collaboration with UNICEF. The BNA app
is available
[here](https://apps.dhis2.org/) for
download.  It is currently compatible with DHIS2 2.28 and above.   

![Standard layout of the BNA App dashboard](../content/bna/resources/images/image001.png)


### Rationale for the BNA App

Health managers have competing demands resulting in limited time,
resources and training to conduct data analysis. Collecting data from
multiple sources and preparing it for analysis themselves can be a
barrier to effectively using data for planning.  While the growing trend
of building dashboards into DHIS2 is encouraging, too often the
information displayed in dashboards is a collection of related (or
sometimes unrelated) indicators rather than a well thought out process
(or framework) of how a workflow or intervention actually works.  The
bottleneck analysis app helps address these issues by automating data
gathering and presentation within DHIS2 and displaying it in a manner
that facilitates systematic analysis for programming.

Effective and timely use of DHIS2 data by stakeholders at all levels of
health system is critical for health service delivery. DHIS2 dashboards
have the potential to enhance the use of data for decision making and
planning by displaying information for managers in an accessible and
actionable manner. This visualization is made possible by using the
bottleneck analysis model integrated with the causality and tracking
actions/solutions to effect interventions.


### Advantages of the BNA App

The bottleneck analysis and planning approach contribute to existing
national and sub-national planning and monitoring cycles by offering a
strategic, rapid and systematic approach to analyzing key health systems
barriers to reaching intervention coverage targets.

This approach can help save time and increase the efficiency of
resources available by identifying where the greatest pockets of unmet
needs or poor service outcomes exist and, in those places, identifying
key bottlenecks, prioritizing what should be addressed immediately, what
should be deferred (prioritization of most effective actions) and
ensuring that resources are programmed to tackle priority bottlenecks
with evidence-informed solutions.

### About demo server and the BNA App meta-data

The BNA demo server is setup to support both development, testing,
training and ensuring quality of features and functions of the demo
server. Additionally, the demo server is also setup to host both demo
data and metadata across various interventions to give chance to users
of the system to explore and learn system features and functions. The
current demo server can be accessed on :
[https://hisp.apps.dhis2.org/training/](https://hisp.apps.dhis2.org/training/)

The server is hosted in the cloud and can be accessed on the
internet via a browser from anywhere as long as there is availability
of internet.

#### Accessing the BNA App                                           

This user guide is documented using the linked BNA App which is available on the
[DHIS2 demo server](https://hisp.apps.dhis2.org/training/). The BNA app is set
up in the DHIS2 Demo server and with linkages to the Scorecard, Root Cause
Analysis and Action Tracker Apps. The current demo server can be accessed
on: [https://hisp.apps.dhis2.org/training/](https://hisp.apps.dhis2.org/training/)
with the username and password provided on the login page..

![Logging and accessing the BNA demo server ](../content/bna/resources/images/image1.png)

#### Indicator Management

The BNA app borrows its meta-data from the general DHIS2 data source and uses
this to create a data store for ease of analysis. Bottleneck analysis metadata
such as indicators and indicator groups are managed using the DHIS2 Indicator
maintenance App.

![Indicator maintenance App](../content/bna/resources/images/image28.png)

Complex indicators that require additional calculations are maintained
using the function maintenance app. These include but are not limited to
indicators on stock data, Human resources.

#### Functional Maintenance App

The BNA App is also integrated with function maintenance App, used to
create custom indicators. Custom Indicators are indicators whose
definition and calculation cannot easily be created using the Indicator
maintenance app in the DHIS2. The app can be easily used by developers
to create custom codes to retrieve and  use indicators with complex
calculations. To use the app, find it
[here](https://apps.dhis2.org/)

![Function maintenance app](../content/bna/resources/images/image27.png)


## BNA App architecture <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/bna/bna-app-architecture.md -->

The BNA Application is built on architecture that eases the user
interactions by having a design concept that promotes the user to follow
their intuition complemented with high performance that considers the
lowest internet connection scenarios with descriptive notification
messages if the user misses a step along the way.

### BNA App Design concepts

#### Do more with less steps

Most of the operations in the application can be achieved in three steps
or less. The BNA App gives a district user or any user at any level with
no administrative privilege the ability to perform operations without a
need to switch between modules or drop ongoing activities. Users can
bookmark interventions, filter interventions by organization unit or
period and more with everything being just a click away.

#### Trust your intuition

The BNA App has been built from the ground app, to make functionalities
more accessible, more intuitive and most importantly more capable. The
App follows a minimalistic design that minimizes any chances of the user
getting lost in the middle of performing their usual operations.

### Layout of the BNA App

The BNA App is flexible to adapt to any number of user journeys depending on the
country's implementations. The primary two users are:

1. ___Administrators:___ can manage interventions with operations such as creating
   interventions, applying data filters for interventions, making legend definitions
   and many more administrative operations.
2. ___District users:___ analyzing the bottlenecks can switch through their
   interventions, bookmark their favorite interventions and perform root cause
   analysis through the root cause analysis widget.

Other bottleneck App users can be national, and regional/counties  users who
can only analyse bottlenecks, sub-nation analysis, route causes for each
bottleneck and their solutions.

### Global DHIS2 Menu

To browse the BNA app, access the DHIS2 demo server with the login credentials
provided on the page. Once logged in, search for Bottleneck Analysis App on the
Search bar.

![Accessing DHIS2 Global Menu while using BNA App in DHIS2](../content/bna/resources/images/image_36.png)(width=50%)

Search for Bottleneck Analysis application and click on it
![Figure 2.3.-B: Searching for the Bottleneck Analysis App on apps list or by typing full or part of app name “Bottleneck Analysis App](../content/bna/resources/images/Imgsearch.png)

### Interventions list

Upon loading the BNA App, users will have access to available interventions and an option to search for more interventions which may not be displayed upon loading. Accessing the shared interventions is limited to the access level they are shared.

![Figure 2.4-A: List of Interventions accessible to logged in user in the BNA App](../content/bna/resources/images/image40.png)

![Figure 2.4-B: Bottleneck analysis chart of the intervention selected from figure 2.4-A](../content/bna/resources/images/image40_.png)

### Interventions Global filters

Right under the interventions list there are controls for the active
interventions. The filter control when clicked expands to offer the user
an ability to make data selections, period selections, organisation unit
selections, and legend configurations. However, all users except
administrators have access to Period Organisation unit filters only.
More details on these operations can be found on chapter 4 section 4.

![Global filter controls in one of the selected Interventions in the BNA App](../content/bna/resources/images/image002.png)

### Intervention items

All interventions in the BNA App contains three items, namely:

1. The Bottleneck Analysis Chart
2. The Sublevel Analysis Table
3. The Root Cause Analysis Widget

These intervention items will be empty when an intervention is created.
The administrator is expected to configure the intervention items by
making selections on the global filters. More details on how to
configure interventions can be found on Chapter 4 Section 5. The
district user is expected to enter data into the root cause analysis
widget as explained in the next chapters.


## BNA App interventions configurations <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/bna/navigating-the-bna-app.md -->

The BNA interventions management (settings) options are only available to users who are created with the administration privileges

Bottleneck analysis application can be found in the Apps menu. if the
application has not yet been installed in your DHIS2 instance or
installation has issues, refer to the installation instructions (Chapter
2) of this documentation for further guidance, or contact the
DHIS2 administrator for your instance.

![bottleneck analysis application on the DHIS2 app menu](../content/bna/resources/images/image34.png){width=50%}

### Starting an Intervention

Once open, the bottleneck analysis application will bring a list of
created interventions, or when no intervention exists, a quick create
button will display for the user to create and add a new intervention.

The new intervention dashboard will display blank templates pending data
selection and filtering.                        

![Bottleneck analysis dashboard with blank chart and table templates](../content/bna/resources/images/image003.png)

> **NOTE**
>
> If bottleneck analysis application is taking
too long to load, and you’re not slow on network, make sure you have
cleared your browser cache. See [BNA App Maintenance](#bna-app-maintenance) for
additional information on clearing browser cache.

The bottleneck app makes good use of cached files for better offline
experience, as a result, when installing higher versions, the bottleneck
app may use older version of cached files and thus break down while
loading.

### Intervention Settings
The administrator user can make data selections from the global filters by simply selecting Settings tab. Currently the  BNA Application supports data selections of Indicators and Functions. Clicking the Settings filter control opens a panel with a list of indicators complemented with a list of data dimension groups. When a user selects an indicator or a function from the list of available data items the selected data items will be populated to the active data dimension group.

![Settings tab for accessing BNA setting options](../content/bna/resources/images/image_set.png)

![BNA  Settings Layout](../content/bna/resources/images/image004.png){ width=70% } ![](../content/bna/resources/images/image43.png)

> **NOTE:**
> Long indicators can be shortened by entering alternative display names as indicated above. This will ensure your chart is readable and easily interpretable.

#### Period configuration

Each intervention to be analyzed must be linked with a specific period for which the determinants members will be analyzed.

To access option for configuring period for intervention’s bottleneck analysis click on “Bottleneck period type”

![Accessing option for configuring intervention period for analysis](../content/bna/resources/images/image_p.png)

![Selecting period type for intervention configuration](../content/bna/resources/images/image_t.png)

#### Legend Configurations

The administrative user can set legend for each indicator in every intervention to show low, medium and high bands with their cut-off points. An administrator can set colors for each band for visualization. Currently the BNA App uses three classes of colors to present indicator performance as per defined cut-off points. Red shows low performance, with yellow and green showing medium and good performance respectively. To manage the Legend, the administrator must can legend label and colour

![Managing Legends for Indicators in the BNA App](../content/bna/resources/images/image_l1.png)

![Adding color classes and  setting cut-off points in Legends management in BNA App ](../content/bna/resources/images/image_l2.png)

![Modifications made on the legend set management will require the  administrator to save the changes ](../content/bna/resources/images/image_l3.png)

> **NOTE:**
> For any changes made, administrative user must click update button displayed in the working window and save changes for persistence, or just close the message in case of rejecting the changes

#### Determinants members management

For each determinant (Commodities, Human resources, Geographic accessibility, Initial utilization and Continuous utilization) up to three members (indicators or functions) can be selected for analysis.

![Accessing option for adding an indicator for the determinants](../content/bna/resources/images/image_d1.png)


![Selecting members (indicators or functions) for each determinant](../content/bna/resources/images/image_d2.png)

After selecting the member, the administrator will get options for further configuration of the member selected which includes defining display label and setting up minimum and maximum values for sub level analysis.

![Defining member display label and minimum and maximum values for sub level analysis](../content/bna/resources/images/image_d3.png)

To save changes made, scroll to the bottom of the configuration screen and click Update

![Saving changes after configuring options for selected member of the determinant](../content/bna/resources/images/image_d4.png)

To add another member (maximum allowable is three) to the same determinant click on the + as shown on figure 3.2.3-E below

![Adding another member to the determinant or deselecting added members](../content/bna/resources/images/image_d5.png)

#### Sharing interventions configuration settings

The defined interventions can be shared and made accessible to multiple users within the system. To share the intervention settings click on Share with option and define people or groups you want to share the configuration with. Only people or groups who will be selected will have access to the configured intervention

![Accessing interventions sharing options](../content/bna/resources/images/image_s1.png)

![Selecting users or user groups and assigning access privileges for each shared intervention](../content/bna/resources/images/image_s2.png)

#### Deleting interventions configuration

To delete created interventions configuration click on delete icon and follow deletion steps

![Click on delete icon to delete configured intervention](../content/bna/resources/images/image_s3.png)

![Click on DELETE button to confirm deletion or CANCEL to reject deletion](../content/bna/resources/images/image_s4.png)


## BNA Analysis and Interpretation <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/bna/bna-analysis-and-interpretation.md -->


Once created for the first time a blank BNA analysis chart will be displayed. The chart will be filled with data automatically as data is made available from linked datasets in the DHIS2 instance.

For non-administrators (e.g. districts users) and administrators they will have options to access interventions configured and shared with them for viewing analysis charts. For each intervention shared to the users, users will be able to further select periods and organization units (locations) for which they want to view bottleneck analysis for.

> **NOTE**
> Users can only access interventions shared with them by the administrator(s) who configured the intervention.


![Click on Search apps or Apps icon to access Apps searching option](../content/bna/resources/images/image_36.png)

### Access intervention for analysis

Search for Bottleneck Analysis application and click on it
![Searching for the Bottleneck Analysis App on apps list or by typing full or part of app name “Bottleneck Analysis App”](../content/bna/resources/images/Imgsearch.png)

Upon loading the BNA App, users will have access to available interventions and an option to search for more interventions which may not be displayed upon loading. Accessing the shared interventions is limited to the access level they are shared.

![List of Interventions accessible to logged in user in the BNA App](../content/bna/resources/images/image40.png)

![Bottleneck analysis chart of the intervention selected from figure](../content/bna/resources/images/image40_.png)

### Selecting period for analysis

After selecting intervention to analyze, the user can specify which period he/she wants to view analysis for. To access option for selecting period for analysis display, click on Period tab

![Access options for period for analysis display](../content/bna/resources/images/image_p1.png)


![Selecting options  for period for analysis display](../content/bna/resources/images/image_p2.png)

### Organization units selection

The BNA App allows the user to make organization unit selections based on groups, levels and user organization units, these are known as selection modes.

![Accessing options for organization units selection](../content/bna/resources/images/image_g1.png)

![Selection of organization units selection](../content/bna/resources/images/image_g2.png)


#### Selection by levels and groups

From the list of Levels, under the input box that reads “Search Levels or groups”, users can then make their selections by clicking the desired levels to view the analysis on the BNA App.

![Selection of org units by levels or groups](../content/bna/resources/images/image_g3.png)

#### Selection by user organization unit

To the top of the selection by level there are buttons which are for selecting organization units relative to the user-assigned organization unit.  This gives flexibility for the users to view the data based on their assigned orgunits or suborgunits of their assigned orgunits.


![Selection of org units by user orgunit](../content/bna/resources/images/image_g4.png)

> **NOTE**
> After completing selection of organization units, user must click on Update button to save changes

> **NOTE**
> Selections by user organization unit disables selection by organization unit tree. To disable selection by user organization unit simply click the active option (the one which appears with gray background) to inactivate it and enable selection by organization unit tree.

> **NOTE**
> Editing and saving configurations of a shared intervention will reflect the new configurations to the district end user with whom the intervention has been shared with.



**4.4 Exporting/Downloading bottleneck analysis chart**

To download the displayed bottleneck analysis chart user can choose from the three available download options (image, MS Excel or PDF

![Bottleneck analysis chart download options](../content/bna/resources/images/image_g5.png)


### Bottleneck analysis Interpretation

Bottleneck analysis a systematic way to look at the main determinants of
effective coverage for selected interventions to identify problem areas
to purposely act on them. The Six coverage determinants, from supply to
demand side, provide a mechanism to analyze where health system
bottlenecks exist. A bottleneck is a loss of system
efficiency. (Adapted from [Tanahashi T. Bulletin of the WorldHealth Organization, 1978, 56\(2\)_295-303.pdf](http://whqlibdoc.who.int/bulletin/1978/Vol56-No2/bulletin_1978_56&#40;2&#41;_295-303.pdf)).

Each intervention in the bottleneck analysis application comes with
three intervention items, the bottleneck analysis chart and sublevel
analysis table, and root cause analysis widget which are there to assist
the district user in analysing the bottlenecks and enter the route
causes and solutions for each identified bottleneck.

### Bottleneck chart operations

The bottleneck analysis chart is a bar graph of the bottleneck
indicators sub-divided in groups of their determinants. The bottleneck
analysis chart can be configured through the global filters whereas the
national level administrator can make data selections and sort the
arrangement of the determinants, determinant group color, organization
unit and period filters for other national users who are not
administrators, regional, and district users to make changes on
organization unit and period filters.

![Options for administrative users to configure indicators, organization unit, period, and legends in BNA application](../content/bna/resources/images/image33.png){width=50%}


### Analyzing bottleneck Charts

![](../content/bna/resources/images/image13.png)

1.  Start from left to right: supply first, then demand, then quality
2.  Identify the lowest bar in the supply side (weakest determinant in
    the existing system)
3.  Identify the biggest drop in the demand side and quality

A bottleneck is a significant gap or drop in coverage determinant
between the expected and the observed. Services must be available first
before they are used. Therefore, bottlenecks are analyzed starting with
supply, followed by demand and finally by quality. The cascade rule
means that quality can not be higher than demand, and demand higher than
supply.

To highlight bottlenecks in the charts, simply click on the bar that
represents the identified bottleneck. The bar should change to color
RED.  This color is not saved as part of the values that represent the
different performances.

> **NOTE**
>
> To deselect the highlighted bars, click once
and the colors will be deselected to the default.

![Highlighting bottlenecks in the chart indicated by RED bars.](../content/bna/resources/images/image38.png)

![](../content/bna/resources/images/image37.png)

When the graph seems different from what we expect, care should be given
to assess common factors e.g. using different denominators for supply,
demand and quality.

### Sublevel Analysis

The sublevel analysis table makes use of the global filters that the
bottleneck analysis chart makes use of with an additional operation of
legend configurations for each indicator, that has been selected. It
presents sublevel analysis of performance each of the indicators in
determinant groups for selected intervention.

![Visualization of sublevel analysis in bottleneck analysis application](../content/bna/resources/images/image19.png)

In sublevel analysis table, user can transpose the layout  of the table
to exchange presentation of indicators and sublevels. To transpose the
table, you have to click an icon just before the download icon below the
sublevel analysis table.

![Sub-Level analysis layout Switch.](../content/bna/resources/images/image2.png){width=50%}

![Changing Layout of Sub-level analysis table](../content/bna/resources/images/image30.png)

### Additional Indicator dictionary

The BNA app is equipped with an indicator dictionary to provide
additional information on the indicators used in the definition and
creation of the BNA chart. To access the indicator dictionary, click on
the (i) icon in the sub-level analysis table.

![Sub-Level Analysis Indicator dictionary](../content/bna/resources/images/image15.png){width=50%}

![Sub-Level Analysis Indicator dictionary](../content/bna/resources/images/image7.png)

The indicator dictionary will display the list of indicators used in
creating the BNA chart, including numerators and denominators,
calculation details, and corresponding data elements. You can also click
on the “Export” button to export the indicator dictionary to excel. To
switch back to the table view, click on the Table icon.

![Sub-Level Analysis table view](../content/bna/resources/images/image16.png){width=50%}



### Root Cause analysis

After the district user has looked at the Bottleneck Analysis Chart and the Sublevel Analysis Chart and has identified the major bottlenecks, they are expected to proceed to the Root Cause Analysis Widget. In the root cause analysis widget they can document the Root causes and Solutions of determinants and indicators for the active intervention based on the period and organization unit filters applied.

At first glance the widget will come up empty and the user can create a new empty row by simply clicking the “Add New” button that is available right under the widget. The new empty row comes pre-populated with the row counter, Intervention Name, Period Name and Organization Unit Name.

![Creating new root cause for analysis](../content/bna/resources/images/image_r1.png)


The user can select determinants and indicators from the dropdown lists and use the free texts to document the root cause and solutions. Once done there is a tick icon on the solution column, the user will click this icon to save the data.

![Adding root causes and suggested solutions for identified bottlenecks in the bottleneck application](../content/bna/resources/images/image_r2.png)

The quality of the causality analysis is a critical determinant of the quality of the resulting plans and the impact on health system performance. It is important to have around the table people with the right knowledge and expertise.

Once a bottleneck is identified, the root causes need to be thoroughly assessed

It is important to know what to look for when facilitating a root cause analysis.

1. Common causes of bottlenecks in the health system (specific for each determinant)
2. Main environmental factors (Social Norms, Legislation/ Policy, Budget/ expenditure, Management/ Coordination)
3. Possible crisis/hazards (if relevant)

Once identified, proposed solutions/ actions need to be documented for follow-up and implementation.

To edit data the user can simply double click a row to make active for editing or right click a row to get a context menu. Currently the context menu has two operations Edit and Delete, whereas, selecting “edit” makes a column active for changes and selecting “delete” removes the data of the particular row from the system.

![Editing or deleting root cause in the specified bottleneck of the selected intervention in the bottleneck application](../content/bna/resources/images/image_r3.png)


## Visualization operations <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/bna/visualization-operations.md -->

### Downloading of visualization

To download the Visualization, hover over the chart, in the
b\]Bottom-left-corner, look out for the download icon below;

![](../content/bna/resources/images/image18.png){width=5%} Click on this Icon to download the chart using
the various formats available.
![](../content/bna/resources/images/image42.png){width=50%}

The Formats provided include, PNG, JPG, CSV, Excel & PDF.

### Basic/Full screen visualization

The BNA App support Basic and full screen views for all visualizations.
To view the chart in full screen, point your cursor in the
top-right-corner of the visualization and click on this icon: ![](../content/bna/resources/images/image26.png){width=7%}
The visualization should display in full screen.



