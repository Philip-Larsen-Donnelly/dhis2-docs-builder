# Dashboard and Demo Server

## Linked Action Tracker Dashboard and Demo server <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/action_tracker/at-app-introduction.md -->

### Introduction to the Action Tracker App

Action Tracker is part of the bottleneck and scorecard cascade that utilizes
DHIS2 analytical features to assess national and sub-national level performance
of key priority interventions aimed at improving health service delivery and
health outcomes. It is a tool that helps improve effective coverage of priority
interventions at sub-national level by tracking actions taken to address the
root causes of key bottlenecks in the health interventions.

The Action Tracker App is developed and maintained by the HISP Community
(University of Oslo (UiO), HISP-Tanzania and HISP Uganda) in collaboration with
UNICEF. The Action Tracker v1.0.0.rc.0 is available for download on the
[Dhis app store.](https://play.dhis2.org/appstore/)  It is currently compatible
with DHIS2 2.28 and above.   

![Figure 1.1-A: Standard layout of the Action Tracker dashboard](../content/action_tracker/resources/images/image01.png){width=80%}

### Advantages of the Action Tracker App

The Action Tracker App helps track the status of key steps taken to address the
 root causes of key bottlenecks in priority interventions. It is built within
 DHIS2 along side the BNA, Scorecard and Root Cause analysis Apps allowing
 systematic analysis, status update and follow up of actions taken to address
 possible solutions to key bottlenecks in health service delivery.

### Rationale for the Linked Action Tracker App

The Linked Action Tracker enables health managers track progress on implementation
of actions for proposed solutions and allows for review and follow up of these
actions. Following the design of BNA, Scorecard and Root Cause Analysis Apps in
DHIS2, it was paramount to design the Action Tracker within DHIS2 to complete
the cascade of Bottle Neck Analysis.

> __NOTE__
> Linked Action Tracker App is dependent on BNA app implementation. All actions to be listed on Action Tracker App must be referencing bottlenecks identified using BNA app. You cannot implement Action Tracker App without a BNA app.

### 1.4 Accessing the Linked Action Tracker

This user guide is documented using the Linked Action Tracker App which is
available on the [DHIS2 demo server](https://scorecard-dev.dhis2.org/demo/).
The Action Tracker is set up in the DHIS2 Demo server and with linkages to the
BNA, Scorecard and Root Cause Analysis Apps. The current demo server can be
accessed on: <https://scorecard-dev.dhis2.org/demo/>
with the username and password provided on the login page.

![Figure 1.4-A: Logging and accessing the Action Tracker demo server](../content/action_tracker/resources/images/image02.png){width=50%}

The server is hosted in the cloud and can be accessed on the internet via a
browser from anywhere as long as there is availability of internet.


### Browsing the Action Tracker <!-- DHIS2-EDIT:https://github.com/hisptz/unicef-apps-docs/edit/master/src/commonmark/en/content/action_tracker/at-app-browsing.md -->

To browse the action tracker app, access the DHIS2 demo server with the login
credentials provided on the page. Once logged in, search for Action Tracker on
the Search bar.

![Figure 1.5.-A: Click on Search apps or Apps icon to access Apps searching option](../content/action_tracker/resources/images/image03.png){width=60%}

![Figure 1.5.-B: Searching for the Action Tracker App on apps list or by typing full or part of app name “Action Tracker](../content/action_tracker/resources/images/image04.png){width=60%}

Click on the Action Tracker to load the Action Tracker App and once loaded, the
user can select the intervention, period, organization unit or modify legend
accordingly;

![Figure 1.5.-B: Loaded Action Tracker App](../content/action_tracker/resources/images/image05.png){width=70%}

#### Selection of an Intervention

The user needs to select the intervention on which bottleneck analysis and root cause analysis were performed and would now like to track actions to improve that particular intervention.

1. Click on the intervention tab to display a list of all available interventions.
   ![Figure 1.5.1-A: Intervention tab providing access to intervention selection](../content/action_tracker/resources/images/image06.png){width=50%}

2. Click on the intervention for which a bottleneck was identified. This intervention will be selected and displayed to the right.

![Figure 1.5.1-B: List of available interventions for selection](../content/action_tracker/resources/images/image07.png){width=50%}

3. Click update to save the intervention

![Figure 1.5.1-A: Selection of an Intervention](../content/action_tracker/resources/images/image08.png){width=50%}

> __NOTE__
> Selection of the wrong intervention will not display the Root Cause Analysis data on the Action Tracker.

#### Period Selection

The Action Tracker allows you to make period selections for fixed periods, relative periods and extended relative periods. All period selections types begin with clicking the period tab.

Click on the period tab to display the options
![Figure 1.5.3-A: Click on period to access period selection options](../content/action_tracker/resources/images/image14.png){width=60%}

Click on the period type to select the desired type of period; either fixed periods or relative periods

![Figure 1.5.3-B: Click on selected period (default monthly) to access period options](../content/action_tracker/resources/images/image15.png){width=60%}

Select the desired period. This will appear to the right
![Figure 1.5.3-D: Selection of preferred period for tracking](../content/action_tracker/resources/images/image16.png){width=60%}

#### Organization Unit Selection

The orgunit selection allows you to select the org unit level for which actions will be tracked. This is the same level for which the root cause analysis was done.

Click on the Org unit tab to access organization unit selection options

![Figure 1.5.4-A: Accessing the Organization unit selection options](../content/action_tracker/resources/images/image19.png){width=60%}

Select the desired Orgunit  level

![Figure 1.5.4-B: Selection of the Organization unit](../content/action_tracker/resources/images/image20.png){width=60%}

Click update to save the selected Orgunit level

![Figure 1.5.4-C: Saving organization unit selected for display](../content/action_tracker/resources/images/image21.png){width=60%}

> __NOTE__
> Selection of the wrong organization unit level will not display the Root Cause Analysis data on the Action Tracker

Once the organization unit is selected and saved, data from the root cause analysis table is retrieved and the data entry module activated to allow entry and editing of the action tracker.

![Figure 1.5.4-D: Display of information from Root Cause Analysis in the Action Tracker](../content/action_tracker/resources/images/image22.png){width=60%}

#### Action Status Settings Configurations

The user can modify the legend based on the number of stages for tracking the action status. Currently the Action Tracker has 4 colour codes which indicate the levels through which the actions are tracked; Maroon indicates “Cancelled”, Yellow indicates “In Progress”, Green indicated “Completed”, Red indicates the action was “Not Done.”

Click on the settings icon in the right upper corner to edit the action status settings
![Figure 1.5.2-A: Accessing legend configuration tab](../content/action_tracker/resources/images/image10.png){width=40%}

![Figure 1.5.2-B: Selecting the Action Status Settings](../content/action_tracker/resources/images/image11.png){width=40%}

Click on the colour tabs to edit the colours

![Figure 1.5.2-C: Editing legend colour](../content/action_tracker/resources/images/image12.png){width=40%}

Edit the legend to the desired legend name.

![Figure 1.5.2-D: Editing legend name](../content/action_tracker/resources/images/image13.png){width=40%}

Set default legend by clicking on the pin. The pin will turn green. This will be the legend that appears once you start action tracking

![Figure 1.5.2-E: Setting default legend](../content/action_tracker/resources/images/image13a.png){width=40%}

Click update to save the changes made to the legend

![Figure 1.5.2-A: Saving changes to legend configurations done](../content/action_tracker/resources/images/image13b.png){width=40%}

__Note:__ 

> Access to configuration of legends depends on user’s access roles

#### 1.5.3 Mandatory Field Settings Configurations

Click on the settings icon in the right upper corner to edit the Mandatory Fields settings

![Figure 1.5.3-A: Accessing mandatory fields settings](../content/action_tracker/resources/images/image13c.png){width=40%}

![Figure 1.5.3-B: Selecting the Mandatory Field Settings](../content/action_tracker/resources/images/image13d.png){width=50%}

Select the mandatory fields that should be displayed on the list during Action tracking.

![Check mandatory fields.](../content/action_tracker/resources/images/image13e.png){width=50%}

![Click update to save the changes made to the mandatory fields settings.](../content/action_tracker/resources/images/image13f.png){width=50%}

__Note:__ 

> Access to configuration of Mandatory Field Settings depends on user’s access roles.



