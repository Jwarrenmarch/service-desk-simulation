# Ticket 03 - Slow and Choppy Screen Performance

**Ticket ID:** INC920819
**Priority:** High
**Category:** Hardware/ Driver Issue - Display Performance
**Status:** Resolved 
**Business Impact:** Computer nearly unusable - Multiple engineering projects stalled


## User Report

Nina Patel (npatel@servicedesk-simulator.com), Engineering Department, Floor 2, reported that everything on her screen had become extremely slow and choppy. Symptoms included:

Scrolling stuttering
Videos unwatchable
Window movement appearing abnormal
Issue began after the weekend with no known trigger
User had already attempted a restart - no improvement

##
Initial Assessment

Symptoms pointed toward a display or graphics driver issue rather than a software or network problem. Key reasoning:

-Issue affected all visual output not just one application
-Restart made no difference - rules out temporary process issues
-Began after weekend - possible automatic update conflict or driver corruption
-No mention of new software installed - external cause likely

High priority assigned correctly - user completely unable to perform design and engineering work.

##
Screenshots
[Ticket received]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 54 49 PM" src="https://github.com/user-attachments/assets/2201589e-986c-402d-bbaf-a03488a167b7" />
Initial HIGH priority ticket - full symptom description and business impact confirm

[Remote desktop search]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 55 14 PM" src="https://github.com/user-attachments/assets/3762947f-47e6-4848-9b60-cda456a2cc0e" />
Initiated remote desktop session - searched for Nina, located SD1020 assigned to Nina Patel

[Remote login]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 55 51 PM" src="https://github.com/user-attachments/assets/e3da4e7d-b54b-432f-b7ee-359eb2f60ad2" />
Authenticated with admin credentials to access SD1020 remotely

[Desktop accessed]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 56 27 PM" src="https://github.com/user-attachments/assets/9bbe83f0-22d7-432e-9b7a-ba88addd5f79" />
Successfully connected to Nina Patel desktop - confirmed remote access established

[Setting search]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 56 47 PM" src="https://github.com/user-attachments/assets/5de74dd7-99e3-4972-b46e-e272ec1f5277" />
Opened Settings and searched for System Update to investigate driver and firmware status

[System information]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 58 24 PM" src="https://github.com/user-attachments/assets/e8834233-305f-4e6f-b9b1-d277fcc6487c" />
Reviewed system specs - 32GB RAM at 38% usage, storage at 62% - ruled out memory and storage as root cause. Noted BIOS version R1ZET55W 1.22

[Update available]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 58 47 PM" src="https://github.com/user-attachments/assets/1fe824db-97be-40bf-aa84-c91386c2e1de" />
Check for Update revealed 6 pending updates including
-BIOS Update v1.58 -> v1.62
- integrated Graphics Driver 31.0.101.4887 -> 31.0.101.5186
-Onboard Audio Driver
-System Firmware Update v2.1 -> v2.4
-Power Management Driver
-Vantix VG-7600 Driver 31.0.101.4887 -> 31.0.101.5186

The outdated Integrated Graphics Driver and Vantix VG-7600 Driver identified as the likely root cause of choppy display performance.

[Updates installed restart required]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 59 07 PM" src="https://github.com/user-attachments/assets/6b283cdf-a4a1-4662-b389-118871a404bb" />
All 6 updates installed successfully - system prompted restart to apply changes

[System restarted]
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 59 24 PM" src="https://github.com/user-attachments/assets/651eba85-cee5-4a48-bdf7-200c1b67423f" />
<img width="1440" height="690" alt="Screenshot 2026-09-30 at 7 59 33 PM" src="https://github.com/user-attachments/assets/f180c47d-9470-4ab9-b670-6afc693a7057" />
<img width="1440" height="715" alt="Screenshot 2026-09-30 at 8 00 13 PM" src="https://github.com/user-attachments/assets/85a88856-2008-442b-a003-5210714b80a9" />
System restarted successfully - confirmed device returned to login screen. Solution complete prompt confirmed correct resolution

[Ticket closed]
<img width="1440" height="715" alt="Screenshot 2026-09-30 at 8 01 54 PM" src="https://github.com/user-attachments/assets/9a2b8553-a5d3-488d-ab70-715fdd21b822" />
Ticket closed with resolution notes documenting remote desktop access and driver update

##

Root Cause

Outdated graphics drivers - specifically the Integrated Graphics Driver and Vantix VG-7600 Driver - caused the display rendering issues. Driver versions had fallen behind, likely causing incompatibility with the current OS build after a weekend system change, resulting in severely degraded visual performance across all display output.

##

Resolution Steps

Read ticket and assessed symptoms - identified likely graphics driver issue based on all-encompassing display degradation
- Initiated remote desktop session and located Nina Patel’s machine SD1020
- Authenticated using admin credentials
- Accessed Nina’s desktop remotely
- Opened Settings and navigated to System Update
- Reviewed system information - confirmed 32GB RAM at 38% usage and storage at 62% - ruled out hardware resource constraints as root cause
- Ran Check for updates - discovered 6 pending updates including critically outdated graphics drivers
- Installed all 6 updates including BIOS, integrated Graphics Driver, Vantix VG-7600 Driver, System Firmware, Audio Driver, Power Management Driver
- Initiated system restart as prompted to apply changes
- Confirmed Device returned to login screen - system operational
- Closed ticket with resolution notes

##

Key skills Demonstrated

-High priority incident management - appropriate urgency and response
-Remote desktop support - connecting to and troubleshooting a user’s machine remotely
- Systematic troubleshooting methodology - ruling out memory and storage before identifying drivers as root cause
-Driver and firmware update management - identifying outdated drivers as root cause of performance degradation
- System diagnostics - reading system specs to eliminate hardware resource issues
- Remote resolution without requiring physical access - fully resolved via remote desktop

##

What I learned

This ticket demonstrated the importance of systematic diagnosis before taking action. Rather than immediately updating drivers, I first checked memory and storage usage to rule out resource constraints as the cause. Only after eliminating those factors did I investigate driver status - where the actual root cause was found. Outdated graphics drivers are a common but easily overlooked cause of display performance issues, particularly after system updates that may introduce version incompatibilities. Remote desktop support allows IT engineers to resolve issues like this without requiring physical presence - particularly valuable in multi-site or hybrid working environments.

