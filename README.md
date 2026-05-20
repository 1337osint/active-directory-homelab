# Active Directory Homelab

## Overview
Built a fully functional Active Directory environment from scratch using 
VirtualBox. Configured a Windows Server 2019 Domain Controller, joined 
Windows client machines to the domain, and implemented Group Policy, 
user management, and network segmentation through pfSense.

## Environment
- Host OS: Windows 11
- Hypervisor: VirtualBox
- Domain Controller: Windows Server 2019 Evaluation
- Client Machine: Windows 10/11
- Firewall/Router: pfSense
- Domain Name: mylab.local

## What I Built
- Installed and configured Windows Server 2019 as a Domain Controller
- Promoted server to DC and created a new AD forest
- Configured DNS integrated with Active Directory
- Created Organizational Units (OUs) for structured user management
- Created and managed multiple user accounts
- Configured Group Policy Objects (GPOs) for security settings
- Joined Windows client machines to the domain
- Configured pfSense as firewall and DHCP server for LAN segmentation
- Tested account lockout, password reset, enable/disable workflows

## Active Directory Tasks Performed
| Task | Description |
|------|-------------|
| User creation | Created multiple domain user accounts |
| Account disable/enable | Disabled and re-enabled user accounts |
| Password reset | Reset passwords and forced change at next login |
| Account lockout | Triggered and resolved account lockouts |
| OU structure | Organized users into logical Organizational Units |
| GPO configuration | Applied Group Policy for password complexity and lockout policy |
| Domain join | Connected Windows client machines to the domain |
| Security groups | Created and managed security groups |

## Network Architecture
- pfSense VM: LAN gateway at 192.168.1.1
- Domain Controller: 192.168.1.101 (static)
- Client machines: DHCP assigned via pfSense
- Splunk SIEM: 192.168.1.50 (receiving AD logs)

## Screenshots
[Screenshots to be added]

## Skills Demonstrated
- Active Directory administration
- Windows Server 2019 configuration
- Group Policy management
- DNS configuration
- Network segmentation with pfSense
- Domain user and group management
- Security policy implementation

- ## Screenshots

### AD DS and DNS Roles Installed
![Roles](AD%20%26%20DNS%20Roles%20Installed.png)

### Organizational Unit Structure
![OUs](3%20Different%20OUs.png)

### Admin Account Domain Admins Membership
![Admin](Admin-Domain-Admins.png)

### Password Policy GPO
![Password GPO](Password%20GPO.png)

### Account Lockout GPO
![Lockout GPO](Account%20Lockout%20GPO.png)

### Desktop Prevention GPO Enabled
![Desktop GPO](Desktop%20Prevention%20GPO%20Enabled.png)

### Security Baseline Policy at Domain Level
![Domain GPO](GPM%20Security%20Baseline%20Policy%20At%20Domain%20Level.png)

### User Security Policy Under _USERS OU
![Users GPO](GPM%20User%20Security%20Policy%20Under%20_USER%20OU.png)

### Security Group Creation (IT Staff)
![Security Group](Security%20Group%20Creation%20(IT%20Staff).png)

### whoami — Domain User Verified
![whoami](AD%20User%20(whoami%20command).png)

### Desktop GPO Active and Enforced
![GPO Active](Desktop%20GPO%20Active%20And%20Working.png)

### gpresult — User Security GPO Applied
![gpresult](gpresult%20Output%20user%20Security%20GPO%20applied%20to%20AD%20User.png)

### Password Reset Evidence
![Password Reset](Password%20Reset%20Evidence.png)

### Account Disabled Evidence
![Account Disabled](Account%20Disabled%20Evidence.png)

### Account Enabled Evidence
![Account Enabled](Account%20Enabled%20Evidence.png)

### Account Investigation Script
![Script](Account%20Investigation%20Script.png)

### Account Lockout Evidence
![Lockout](AD%20Account%20Lockout%20Evidence.png)

### Account Lockout Troubleshot and Resolved
![Unlocked](Account%20Lockout%20Troubleshooted.png)

### _COMPUTERS OU — Client Machine Moved
![Computers OU](Computers-OU.png)
