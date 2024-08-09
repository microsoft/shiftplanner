# Technical components
This document itemises the technical components that make up the solution
## Two (2) Canvas apps:
- “Shift Planner” – where a shift admin can configure and manager their own shift and teams
- “Shift Planner – Mobile” – where a user can view their shifts and request for swap or time-off
## One (1) Model Driven App:
- “Shift Planner Administrator” – where an admin can manage all reference data
## Three (3) Security roles:
- Shift Planner Administrator
- Shift Planner Shift Administrator
- Shift Planner End User
##  Two (2) Environment variables:
- Mobile App Link – holds the link to the mobile app
- Shared Calendar Name – holds the name of the used calendar for the calendar invites
## Two (2) Choices:
- Change Type
	1. Time off
	2. Swap
- Invite Action
	1. Add
	2. Unpublished
	3. Remove
	4. Swap
## Fifteen (15) tables
1. App Setting
2. Change Request
3. Email Log
4. Email Template
5. Facility
6. Role
7. Shift Booking
8. Shift Team
9. Shift Type
10. Team Position
11. User
12. User Affiliation
13. User Availability
14. User Role
15. Zone
## Four (4) Connection References:
- Microsoft Power Accelerator – Approvals: Connection reference to Approvals
- Microsoft Power Accelerator – Content Conversion: Connection reference for Content Conversion
- Microsoft Power Accelerator – Dataverse: Connection reference to Dataverse
- Microsoft Power Accelerator – Outlook: Connection reference for Outlook
## Ten (10) Power Automate flows
1. Cancel Time-Off and Swap Request
2. Get Staff Mode Table
3. Populate Email Logs Table
4. Populate Shift Booking Table
5. Send Calendar Invite
6. Swap Initial Approval
7. Swap Final Approval
8. Time-Off Approval and Rejection
9. Week Status Calendar Invite
10. Week Status Email Notification