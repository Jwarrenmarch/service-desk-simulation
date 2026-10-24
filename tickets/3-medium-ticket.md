# Ticket 02 - Employee Off boarding / Account Deprovisioning

**Ticket ID:** INC300944

**Priority:** MEDIUM

**Category:** Account Deprovisioning - Employee Off boarding

**Status:** Resolved

**Business Impact:** Security compliance requirement - must complete before end of business Friday



## User Request

Mike Reeves (Facilities, Floor 3) submitted an HR-approved off boarding request for Sarah Mitchell (smitchell), Marketing Department, whose last day is this Friday. Required actions per off boarding checklist:

- Disable account
- Rest password
- Remove all group memberships
- Revoke all software licenses
- Recover and unassigned all IT assets

The manager had been notified. HR Director approval was confirmed in ticket.


[Ticket Received]
<img width="1445" height="671" alt="Screenshot 2026-09-25 at 7 49 05 PM" src="https://github.com/user-attachments/assets/ec4f35df-d906-4505-98b1-e4099bf3d0cf" />
Initial ticket showing full off boarding request, employee details, and business impact: security compliance deadline.

[User Located And Account Disabled]
<img width="1445" height="667" alt="Screenshot 2026-09-25 at 7 50 09 PM" src="https://github.com/user-attachments/assets/b48e38ef-071d-420d-bd78-d8411f3a0ccd" />
Located smitchell in the directory. The Authentication tab confirmed the account was already disabled. MFA status: Enrolled. Password expired: No.


[Password Reset]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 51 27 PM" src="https://github.com/user-attachments/assets/c91e9fa4-3115-462a-a1b9-3195f629cf58" />
Reset the password to prevent any residual access. A temporary password was generated. The system noted the account is locked and the password will not work until the account is unlocked, confirming full access revocation.

[Group Memberships]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 53 26 PM" src="https://github.com/user-attachments/assets/05597d2e-b28b-4599-b53c-cab80bca1cd4" />
Reviewed group memberships and found three groups: Domain Users, Marketing, and Printer-Users.

[Remove Marketing Group]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 53 48 PM" src="https://github.com/user-attachments/assets/1189a2e8-7b95-4196-b4b2-f11dba1b92b3" />
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 54 02 PM" src="https://github.com/user-attachments/assets/421a2c74-3583-4a91-86b9-738291109656" />
Removed Marketing group membership and confirmed removal.

[Remove Printer-Users Group]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 54 15 PM" src="https://github.com/user-attachments/assets/1ea46866-0075-4b8c-9248-db18ac153a44" />
Removed Printer-Users group membership and confirmed removal. Domain Users was retained because it is the base system group and cannot be removed.

[Licenses Before Removal]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 55 55 PM" src="https://github.com/user-attachments/assets/49df95c8-3373-43bd-9477-f255c4f6d2af" />
Found four active software licenses assigned, all requiring revocation: Office Suite E3, Video Meet Pro, Team Messenger Business, and Design Suite.

[Licenses After Removal]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 7 56 11 PM" src="https://github.com/user-attachments/assets/a3ae789b-a811-4cfe-af20-da3852b8822a" />
All four licenses were successfully removed, confirmed by the "no licenses assigned" message.

[Asset Management Search]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 8 36 07 PM" src="https://github.com/user-attachments/assets/088de8ec-ba32-4d1b-af29-a4c2de5863b2" />
Search Asset Management for Sarah Mitchell and found 5 deployed assets:
- HS1066 - USB office headset
- KB1066 - Wireless Office Keyboard
- MN1066 - Clearview 24” Monitor
- SD1066 - Standard Workstation Laptop

[Laptop Unassigned]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 8 36 51 PM" src="https://github.com/user-attachments/assets/cda38e9b-b242-47e6-b61c-3093a4bc482f" />
Opened the SD1066 laptop record and unassigned it from Sarah Mitchell. Updated the status to "Ready to deploy" to return the asset to available inventory.

[Ticket Closed]
<img width="1445" height="640" alt="Screenshot 2026-09-25 at 8 39 05 PM" src="https://github.com/user-attachments/assets/d50f2d25-c11c-46ca-89cf-1778b36b8ee5" />
Ticket closed with resolution notes confirming all off boarding steps completed per HR checklist.

##

Resolution Steps

1. Located user account smithell in the directory by searching “Sarah” and cross-referencing department and username against ticket details. 
2. Navigated to the Authentication tab and confirmed the account was already disabled.
3. Reset the password to prevent any residual access using saved credentials or session tokens.
4. Navigated to the Groups tab and identified three group memberships: Domain Users, Marketing, and Printer-Users.
5. Removed Marketing group membership.
6. Removed Printed-Users group membership.
7. Retained Domain Users as the base system group, since standard practice is not to remove it.
8. Navigated to the Licenses tab and identified four active software licenses.
9. Removed all four licenses: Office Suite E3, Video Meet Pro, Team Messenger Business, and Design Suite.
10. Opened Asset Management and searched by user name, Sarah Mitchell.
11. Located five deployed assets assigned to the user.
12. Opened laptop record SD1066, unassigned it from the user, and updated the status to Ready to deploy.
13. Closed ticket with resolution notes referencing HR checklist completion.

##

Key Skills Demonstrated

- Employee off boarding and account de provisioning
- Active Directory / directory services - account management and group administration
- Security compliance - understanding why prompt off boarding matters for data protection
- Software license management - identifying and revoking assigned licenses
- IT asset management - locating, reviewing, and un assigning hardware from departing employees
- Methodical checklist approach - working through multiple interdependent tasks systematically
- Clear resolution documentation for HR and audit trail.

##

What I learned
Employee off boarding is more complex than it appears - it requires coordinating across multiple systems simultaneously: directory services, licensing, and asset management. Missing any step creates a security risk, as a former employee could retain access to systems, software, or physical hardware. This ticket reinforced the importance of following a structured checklist approach and documenting every action taken for compliance and audit purposes. In a real environment this process would typically also include data backup, email forwarding configuration, and handover of any shared accounts or passwords held by the departing employee.


