# Shift Planner Getting Started Guide
This document describes the process of configuring and using the Shift Planner Power Platform Template for your team or organisation.

This involves the following Parts:
1. Loading **Email Templates** for communications the system will perform
2. Setting up **Facilities** for which you will roster E.g. Main site
3. Establishing the unique **Roles** that users will perform E.g. 
4. Setting up the **Shift types** that you will staff E.g. Morning Shift, Afternoon Shift, Night Shift

## Load Reference Data
The first step is to load reference data into the system. 

### Part 1: Email Templates
1. Download the email templates from [here](Default-Email-Templates.xlsx)
2. Navigate to [make.powerapps.com](https://make.powerapps.com/)
3. Click on **Apps** in the left navigation
4. Click on the play button next to **Shift Planner Administrator** to play the app
> [!NOTE]
> If the play button is disabled or not visible, you need to publish all customisations. Navigate to **Solution** in the left navigation and press the **Publish all customisations** button. Once this is complete, the playu button should be visible
5. Click on the **Email Templates** left menu option
> ![image](https://github.com/user-attachments/assets/4a32de37-8a8d-47a3-bca8-ecf7a37fc1c6)
6. From the toolbar, click on the Import From Excel button
> ![image](https://github.com/user-attachments/assets/71df4b4e-e22e-4f2e-8a70-1a6f8baabab2)
7. Select the file you downloaded from [here](Default-Email-Templates.xlsx)
8. Click **Next**
9. Click **Finish Import**
10. Click **Track Progress** and monitor the import using the Refresh button on the toolbar. When 15 records are successfully loaded, the import is complete
11. You can navigate back to the **Email Templates** menu option and edit any email templates to suit your organisation.

### Part 2: Setting up Facilities
Facilities are the the primary grouping for locations to which will plan shifts for. Each facility is divided into Zones. Shifts occur at the Zone level. To setup the facilities, perform the following steps.

1. From the **Shift Planner Administrator** App, navigate to **Facility**
2. Click **New** to create a new Facility, populate the Name and Description, then press **Save**
3. Click on the **Zone** tab of the newly created facility
4. For each zone you plan to roster for, click the  **+New Zone** button, populate the name and click **Save**
![image](https://github.com/user-attachments/assets/65376b2a-426d-4793-a0be-477a712b9a39)

5. Repeat this process for each facility you wish to create

### Part 3: Setup Roles
Roles are the distinct functions users are qualified and/or authorised to perform (e.g. a triage nurse or receptionist). To setup the roles, perform the following steps.

1. From the **Shift Planner Administrator** App, navigate to **Roles**
2. Click **New** to create a new Role, populate the Name and Description, then press **Save**
3. Repeat step 2 for each new Role
   
### Part 4: Setup Shift Types
Shift types classify the various types of shifts, such as morning, evening, and night shifts. These classifications aid in the organization and assignment of shifts based on specific time slots and requirements.

1. From the **Shift Planner Administrator** App, navigate to **Shift Types**
2. Click **New** to create a new Shift Type, populate the Name, Start Date, and End Date then click **Save**
> [!NOTE]
> Start Date consists of a Date component and a Time component. The date component is the first date from which the shift will become available for scheduling. The Time component is the time of day that the shift will start.
> End Date consists of a Date component and a Time component. The date component is the last date on which the shift will be available for scheduling. The Time component is the time of day that the shift will end.
4. Repeat step 2 for each new Role
> Here is an example of shifts covering a 24 hour period
> ![image](https://github.com/user-attachments/assets/2f292777-1e7f-4985-8bbe-7f305d00b795)


