# Shift Planner Installation Guide

## Installation Steps
### Prepare Connectors
The following connections must be created prior to importing the solution:
- Microsoft Dataverse
- Office 365 Outlook
- Approvals
- Content Conversion
> [!NOTE]
> Note: We recommend using a system account to create the connections and import the solution, although this is not required.

Any user with the **System Administrator** security role can perform the following steps:
1. Go to the Power Apps portal https://make.powerapps.com/
2. Click on the **Environments** tab and select the environment where the solution will be installed.
3. Using the left navigation, click on **More**, **Connections,** and then click on **New connection.**
4. Look for **Microsoft Dataverse**, **Office 365 Outlook**, **Approval** or **Content Conversion**.
5. Click on **Create.** This step will create a new connection with the logged-in user's credentials.

### Importing the solution into the new system
1. Go to https://make.powerapps.com/.
2. Go to the environment where you want to install the solution.
3. Click on Solution from the left navigation.
4. Click import Solution from the top of the screen.
5. Import solution screen will appear.
6. Click browse and open **mpa_ShiftPlanner_1_0_0_1.zip** (unmanaged) or
**mpa_ShiftPlanner_1_0_0_1_managed.zip** for managed solution.
7. Click Next.
8. Validate the detail and click on Import Button
9. Verify that the tables exist as shown in the image below.

### Assign Security Roles to the Users
The solution includes three (3) new security roles described in the **Security Role Descriptions** section above.

Assign **Shift Planner End User** to users who need access to the Mobile Canvas app to view their assigned shifts
and to request for time-off or swap shifts.

Assign **Shift Planner Shift Admin** to users who will need access to the Desktop Canvas app to configure their
shift’s schedule and team.

Assign **Shift Planner Admin** to users who will manage the data within the Model-driven app, including creating,
updating facilities, zones, shift types, roles, and email templates for the management of the shift schedule.

Roles can be assigned from the admin portal using the following steps:
1. Go to the admin portal https://admin.powerplatform.microsoft.com/
2. Click on the **Environment** tab and select the environment where the solution was installed.
3. Click on Users > See all
4. Select the user(s), click **Manage security roles,** and select the appropriate role.
5. Click Save

### To publish the canvas application:
1. Go to the power apps portal https://make.powerapps.com/
2. Click on the **Environments** tab and select the environment where the solution was installed.
3. Click on **Solutions** in the left navigation, find the **Shift Planner** solution under the managed/unmanaged
(depending on the type of solution installed) tab, then click the **Apps** in the navigation and select **Shift
Planner.**
4. Click on the three dots and click on Share.
5. Look for the user(s) that you want to share the app with
	a. For users that should have access to edit the app, check the **Co-owner** box.
	b. For regular users of the app, leave that checkbox empty.
	c. If everyone in the company should be able to use the app, you can look for **Everyone** in the **Enter a name** box.
5. When you’re done, click Save.
6. Publish the App.
## Initial Configuration
The canvas applications feed the data on Dataverse and need the environment variables set up to work. There
are also flows that run as part of the applications’ functionalities and capabilities. Please ensure these flows are
turned on before using the applications.
### Fill in the environment variables:
The solution includes two (2) environment variables that must be filled in first:
- Mobile App Link – The link to the Shift Planner mobile app when played
- Shared Calendar Name – Name of user’s regular calendar (the default name is **Calendar**)

To get the Shift Planner mobile app link environment variable:
-  On the left navigation, go to Apps. Look for the Shift Planner Mobile app, click on the 3 dots next to the
name, and select Details.
- You can find the Shift Planner Mobile app link under Web Link and copy it.
- Go to Environment variables and click on Mobile App Link to open it.
- Then paste your mobile app link under Current Value and click save.

### Populate the reference data:
To configure the application and populate the necessary reference data, open your environment and go to your
model-driven app labeled **Shift Planner Administrator**. As populating the reference data is done in the MDA,
please refer to the Shift Planner_Model Driven App Documentation.pdf for the comprehensive guide on
navigating the MDA and populating the needed reference data.

### Other Important Details
