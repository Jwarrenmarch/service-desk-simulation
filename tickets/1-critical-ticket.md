# Ticket 04 - Critical Hardware Failure / PC Replacement and Deployment

**Ticket ID:** INC0012871
**Priority:** CRITICAL
**Category:** Hardware Failure - Complete PC Replacement and Deployment
**Status:** Resolved
**Business Impact:** Customer Support agent completely offline - calls queueing with no agent available to answer
##

User Report

Quinn Adams (qadams@servicedesk-simulator.com), Customer Support Department, Floor 1, reported their desktop PC was completely dead with no response whatsoever: no lights, no fan, no beep on power button press.


User troubleshooting already performed:
- Pressed power button multiple times - no response
- Tested wall outlet with another device - outlet confirmed working
- Confirmed completely dead - no signs of life

Diagnosis: Complete hardware failure. Repair not viable, immediate replacement required.

## Screenshots

[Critical Ticket Received]
<img width="1445" height="673" alt="Screenshot 2026-09-27 at 1 03 17 PM" src="https://github.com/user-attachments/assets/b2f9daea-bf96-43b3-af79-58be9216215c" />
Critical priority ticket: complete hardware failure with immediate business impact confirmed. Customer Support calls actively queueing with no agent available.

[Documentation Search - Server Imaging]
<img width="1423" height="673" alt="Screenshot 2026-09-27 at 1 11 49 PM" src="https://github.com/user-attachments/assets/80799954-a881-40b4-a1c4-8af4f608564a" />
Consulted Documentation Station to identify the correct deployment procedure and located the Hardware and Assets deployment guide covering PC setup and replacement workflows.


[Physical Setup - Cables Connecting]
<img width="1423" height="673" alt="Screenshot 2026-09-27 at 1 14 27 PM" src="https://github.com/user-attachments/assets/8b127c5e-e8fd-44cf-a35d-e817d489bb62" />
Initiated physical setup of the replacement workstation, connecting all required cables: power, ethernet, DisplayPort, USB keyboard, and USB mouse (0/5 connected).


[Physical Setup - Complete]
<img width="1423" height="673" alt="Screenshot 2026-09-27 at 1 15 09 PM" src="https://github.com/user-attachments/assets/76080fdc-db6e-4fdd-95eb-fd32f095a2b5" />
All 5 cables successfully connected, and the system was confirmed Ready to Boot. All peripherals online, monitor active.


[Documentation - Deployment Credentials]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 6 55 02 PM" src="https://github.com/user-attachments/assets/b6d085a0-c28d-4006-9df1-6b6faf7cb0fe" />
Referenced the deployment credentials documentation and confirmed the domain (servicedesk-simulator.local), task sequence password, and domain join procedure before proceeding with imaging.


[Task Sequence Wizard - Authentication]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 6 55 46 PM" src="https://github.com/user-attachments/assets/8432fe79-1e72-4038-8e9d-7d774f29cf27" />
Authenticated to deployment share using task sequence password - Step 6 of 11 in deployment process.

[Computer Name Variable - SD1042]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 6 56 02 PM" src="https://github.com/user-attachments/assets/9e25ca3f-9cc8-4ff8-8c0e-38e938507fed" />
Set the OSDCOMPUTERNAME variable. The initial attempt used SD1042.


[Computer Name Variable - Corrected To SD2036]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 42 01 PM" src="https://github.com/user-attachments/assets/9ab85feb-9c74-4e33-aa17-2a137d2e3fbe" />
Corrected OSDCOMPUTERNAME to SD2036 - ensuring correct asset tag assigned to replacement machine.

[Computer Name Confirmed - SD2036]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 42 30 PM" src="https://github.com/user-attachments/assets/fbc6ea23-9db9-4b86-9dd8-a79996df860a" />
OSDCOMPUTERNAME confirmed as SD2036, then proceeded to the next deployment step.

[Task Sequence Running]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 43 33 PM" src="https://github.com/user-attachments/assets/554c5eda-c42a-49e3-b7f2-f09e22a188ec" />
Imaging task sequence running: Setup Workstation OS and Imaging Server in progress. The system automatically joined servicedesk-simulator.local.

[Domain Login Screen]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 45 31 PM" src="https://github.com/user-attachments/assets/6d30d8c3-e2c5-4931-a838-59f7890d07c4" />
Post-imaging login screen showing the machine domain joined to SERVICEDESK-SIMULATOR.LOCAL. Signed in with domain credentials to verify successful deployment.

[Deployment Successful]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 45 49 PM" src="https://github.com/user-attachments/assets/f44bf066-c6fb-434b-bbe5-add86e9e4814" />
Deployment confirmed successful: SD2036, Server Imaging, Desktop. Machine ready to register in Asset Manager and ship to the user.

[PC Shelf]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 47 17 PM" src="https://github.com/user-attachments/assets/41e5b0f4-a1a3-4a95-8cb1-97e756387e79" />
PC Shelf showing SD2036 (Server Imaging) ready alongside SD1066, confirming 2 machines ready to ship.

[Ship Manager - User Communication]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 50 36 PM" src="https://github.com/user-attachments/assets/6dab0beb-19d9-4613-9457-197621463fc9" />
Contacted Quinn Adams via chat to obtain a shipping address for the replacement machine. User confirmed address: 7286 Willow Way, Raleigh, NC 27601.

[Ship Manager - Shipment Configured]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 51 16 PM" src="https://github.com/user-attachments/assets/9f03e7e2-52f4-4f0d-8921-650686c89adf" />
Shipment configured: recipient Quinn Adams, SD2036 Server Imaging Desktop, Rush Priority (instant) shipping, return label included for failed hardware.


[User Confirmation Received]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 51 41 PM" src="https://github.com/user-attachments/assets/dfb32289-bc4f-4676-b215-7257191024ee" />
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 52 49 PM" src="https://github.com/user-attachments/assets/e67c61d3-2581-4186-a406-2a3ad024e141" />
Quinn Adams confirmed the replacement was received and working: "OMG that was SO fast, it already got here! Plugged it in and it's working perfectly. Thank you so much!!"


[Ticket Closed]
<img width="1440" height="690" alt="Screenshot 2026-09-28 at 10 58 57 PM" src="https://github.com/user-attachments/assets/242ae2fd-1974-4c37-8a63-5987033a8d70" />
Ticket closed with resolution notes documenting PXE boot deployment and shipment to the Customer Support floor.


## Resolution Steps

1. Received CRITICAL ticket - assessed symptoms and confirmed complete hardware failure based on user troubleshooting already performed (outlet confirmed working, no response whatsoever)
2. Determined repair not viable - immediate replacement machine required
3. Consulted Documentation Station for correct deployment procedure - located server imaging and deployment credentials guides.
4. Initiated physical setup of replacement workstation SD2036 - connected all 5 required cables and confirmed Ready to Boot
5. Booted replacement machine and entered deployment Task Sequence Wizard
6. Authenticated to deployment share using task sequence credentials from documentation 
7. Set OSDCOMPUTERNAME variable to SD2036 - ensuring correct asset identity assigned to replacement machine
8. Ran imaging task sequence - OS setup and domain join complete automatically to servicedesk-simulator.local
9. Signed in with domain credentials at Step 11 to verify successful deployment
10. Confirmed deployment successful - SD2036 ready in PC Shelf 
11. Opened Ship Manager - contacted Quinn Adams via chat to obtain delivery address
12. Configured shipment: SD2036, Rush Priority (Instant), return label included for failed hardware recovery
13. Shipped replacement machine to Quinn Adams, 7286 Willow Way, Raleigh, NC 27601
14. Received user confirmation - replacement received and working correctly
15. Closed ticket with resolution notes

## Key Skills Demonstrated

- CRITICAL incident management - correct prioritization and rapid response to business-stopping issue
- Hardware failure diagnosis - correctly identifying complete hardware failure vs repairable fault based on symptom analysis
- PC deployment and imaging - full end-to-end workstation deployment using PXE boot and server imaging task sequence
- Domain join process - understanding of domain authentication and workstation provisioning to Active Directory domain
- Documentation usage - consulting internal SOPs and credentials documentation before proceeding with deployment - following correct procedure
- Asset management - assigning correct asset tag (OSDCOMPUTERNAME) during deployment
- Hardware shipping and logistics - configuring replacement shipment with correct details including return label for failed hardware recovery
- User communication under pressure - maintaining professional, calm communication with user during a CRITICAL business-stopping incident
- End-to-end ownership - managed the entire incident from initial diagnosis through deployment, shipping, and user confirmation

## What I learned

This was the most complex and high pressure ticket in the simulation, a CRITICAL priority incident with direct business impact requiring a full hardware replacement and deployment rather than a simple fix. The key lesson was recognizing immediately that repair was not an option and pivoting directly to replacement, which minimized downtime for the user.

Consulting the documentation before proceeding with imaging was critical; without the correct task sequence credentials and OSDCOMPUTERNAME variable the deployment would have failed or created an incorrectly named asset in the system. Following procedure and documentation even under pressure is essential in real IT environments.

The user communication element was also significant: maintaining a calm, professional tone with a frustrated user whose entire workflow was blocked, and keeping them updated on progress, is as important as the technical resolution itself.

