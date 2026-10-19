# Ticket 02 - Employee Offboarding / Account Deprovisioning

**Ticket ID:** INC300944
**Priority:** MEDIUM
**Category:** Account Deprovisioning - Employee Offboarding
**Status:** Resolved
**Business Impact:** Security compliance requirement - must complete before end of business Friday



## User Request

Mike Reeves (Facilities, Floor 3) submitted an HR-approved offboarding request for Sarah Mutcheel (smitchell), Marketing Department, whose last day is this Friday, Required actions per offboarding checklist:

Disable account
Rest password
Remove all group memberships
Revoke all software licenses
Recover and unassign all IT assets

The manager had been notified. HR Director approval confirmed in ticket.

—----

[Ticket received]
<img width="1445" height="671" alt="Screenshot 2026-09-25 at 7 49 05 PM" src="https://github.com/user-attachments/assets/ec4f35df-d906-4505-98b1-e4099bf3d0cf" />
Initial ticket showing full offboarding request, employee details, and business impact - security compliance deadline.

[User located and account disabled]
<img width="1445" height="667" alt="Screenshot 2026-09-25 at 7 50 09 PM" src="https://github.com/user-attachments/assets/b48e38ef-071d-420d-bd78-d8411f3a0ccd" />
Located smitchell in directory - Authentication tab confirmed account already disabled. MFA status: Enrolled.
Password expired: No

[Password reset]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 51 27 PM" src="https://github.com/user-attachments/assets/c91e9fa4-3115-462a-a1b9-3195f629cf58" />
Reset password to prevent any residual access - temporary password generated. System noted account is locked and password will not work until account is unlocked, confirming full access revocation.

[Group memberships]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 53 26 PM" src="https://github.com/user-attachments/assets/05597d2e-b28b-4599-b53c-cab80bca1cd4" />
Reviewed group memberships - found three groups:
Domain Users, Marketing, Printer-Users.

[Remove Marketing group]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 53 48 PM" src="https://github.com/user-attachments/assets/1189a2e8-7b95-4196-b4b2-f11dba1b92b3" />
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 54 02 PM" src="https://github.com/user-attachments/assets/421a2c74-3583-4a91-86b9-738291109656" />
Removed Marketing Group membership - confirmed removal.

[Remove Printer-Users group]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 54 15 PM" src="https://github.com/user-attachments/assets/1ea46866-0075-4b8c-9248-db18ac153a44" />
Removed Printer-Users group membership - confirmed removal.
Domain Users retained as this is the base system group and cannot be removed.

[Licenses before removal]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 55 55 PM" src="https://github.com/user-attachments/assets/49df95c8-3373-43bd-9477-f255c4f6d2af" />
Found four active software licenses assigned:
Office Suit E3, Video meet Pro, Team messenger business, Design Suite - all requiring revocation.

[Licenses after removal]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 56 11 PM" src="https://github.com/user-attachments/assets/a3ae789b-a811-4cfe-af20-da3852b8822a" />
All four licenses successfully removed - confirmed “no licenses assigned”

[Asset management search]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 8 36 07 PM" src="https://github.com/user-attachments/assets/088de8ec-ba32-4d1b-af29-a4c2de5863b2" />
Search Asset Management for Sarah Mitchell - found 5 deployed assets:
HS1066 - USB office headset
KB1066 - Wireless Office Keyboard
MN1066 - Clearview 24” Monitor
SD1066 - Standard Workstation Laptop

[Laptop unassigned]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 8 36 51 PM" src="https://github.com/user-attachments/assets/cda38e9b-b242-47e6-b61c-3093a4bc482f" />
Opened SD1066 laptop record - unassigned from Sarah Mitchell.
Status update to “Ready to deploy” - asset return to available inventory.

[Ticket closed]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 8 39 05 PM" src="https://github.com/user-attachments/assets/d50f2d25-c11c-46ca-89cf-1778b36b8ee5" />
Ticket closed with resolution notes confirming all offboarding steps completed per HR checklist

—-

Resolution Steps

Located user account smithell in the directory by searching “Sarah” and crossing-referencing department and username against ticket details 
Navigated to Authentication tab - confirmed account was already disabled
Reset password to prevent any residual access using saved credentials or session tokens
Navigated to Groups tab - identified three group membership: Domain Users, Marketing, Printer-Users
Removed Marketing group membership
Removed Printed-Users group membership
Retained Domain Users - base system group, standard practice not to remove
Navigated to Licenses tab - identified four active software licenses
Removed all four licenses: Office Suite E3, Video Meet Pro, Team Messenger Business, Design Suite
Open Asset Management - searched by user name Sarah Mitchell
Located five deployed assets assigned to the user
Opened laptop record SD1066 - unassigned from user, status update to Ready to deploy
Closed ticket with resolution notes referencing HR checklist completion.

Key Skills Demonstrated
Employee off boarding and account de provisioning
Active Directory / directory services - account management and group administration
Security compliance - understanding why prompt off boarding matters for data protection
Software license management - identifying and revoking assigned licenses
IT asset management - locating, reviewing, and un assigning hardware from departing employees
-Methodical checklist approach - working through multiple interdependent tasks systematically
-Clear resolution documentation for HR and audit trail.

What I learned
Employee off boarding is more complex than it appears - it requires coordinating across multiple systems simultaneously: directory services, licensing, and asset management. Missing any step creates a security risk, as a former employee could retain access to systems, software, or physical hardware. This ticket reinforced the importance of following a structured checklist approach and documenting every action taken for compliance and audit purposes. In a real environment this process would typically also include data backup, email forwarding configuration, and handover of any shared accounts or passwords held by the departing employee.


