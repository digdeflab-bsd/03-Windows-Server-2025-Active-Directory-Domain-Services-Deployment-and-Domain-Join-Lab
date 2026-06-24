# Active Directory Domain Services Deployment and Domain Join Lab

![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=flat&logo=youtube&logoColor=white)

https://youtu.be/Vw0njgm2QDw

## Summary
![Active Directory](https://img.shields.io/badge/Active_Directory-5E5E5E?style=for-the-badge&logo=microsoft&logoColor=white)

This lab focused on deploying Active Directory Domain Services (AD DS) and DNS on Windows Server 2025, promoting the server to a Domain Controller, designing an organizational unit (OU) structure, creating users and groups, joining client machines to the domain, and validating domain functionality.

## Goal

To build a basic Active Directory environment by configuring a new forest, deploying core directory services, organizing administrative structures, and connecting client workstations to the domain.

## What I Did

### 1. Installed Active Directory and DNS Roles

* Added the Active Directory Domain Services (AD DS) server role.
* Added the DNS Server role.
* Monitored and verified the role installation process until completion.

### 2. Promoted the Server to a Domain Controller

* Started the AD DS deployment configuration process.
* Created a new forest named **digitaldefence.local**.
* Completed the prerequisite checks successfully.
* Continued with the domain controller promotion process.
* Allowed the server configuration and installation tasks to complete.
* Confirmed the server was successfully configured as a Domain Controller.
* Signed out and rebooted the server as required.

### 3. Verified and Configured DNS

* Opened the DNS management console after reboot.
* Verified the Forward Lookup Zone configuration.
* Created a Reverse Lookup Zone to support reverse name resolution.

### 4. Configured Active Directory Administrative Structure

Using Active Directory Sites and Services:

* Renamed the default site to **Africa**.

Administrative usability tasks:

* Pinned commonly used management tools to the taskbar for easier access during administration.

### 5. Designed and Created Organizational Units (OUs)

Created the following top-level Organizational Units:

* South Africa
* Zimbabwe

Under **South Africa**, created:

* Pretoria

  * Computers
  * Servers
  * Groups
  * Users
* Johannesburg

  * Computers
  * Servers
  * Groups
  * Users

Under **Zimbabwe**, created:

* Harare

  * Computers
  * Servers
  * Groups
  * Users
* Bulawayo

  * Computers
  * Servers
  * Groups
  * Users

### 6. Created Users and Security Groups

Using Active Directory Users and Computers:

* Created user accounts.
* Moved users into their designated Users OUs.
* Created a group named **IT Security**.
* Added selected users to the IT Security group.

### 7. Joined Client Machines to the Domain

* Logged on to the client machines.
* Joined the clients to the **digitaldefence.local** domain.
* Logged on using the domain user accounts that had been created.

### 8. Verified Domain Connectivity and Functionality

Performed basic validation tests from the client systems using Command Prompt:

* `ipconfig /all`
* `set`
* `nslookup digitaldefence.local`
* `ping 192.168.60.80`
* `ping 8.8.8.8`

These checks were used to verify domain connectivity, DNS resolution, network configuration, and general communication.

### 9. Created VM Snapshots

* Created snapshots of all virtual machines after configuration and testing.
* Retained snapshots as recovery points for future lab activities.

## Tools and Technologies

* Windows Server 2025
* Active Directory Domain Services (AD DS)
* DNS Server
* Active Directory Users and Computers
* Active Directory Sites and Services
* VMware virtual machines
* Windows Command Prompt

## Skills Demonstrated

* Active Directory deployment
* Domain Controller promotion
* DNS configuration
* Active Directory organizational design
* Organizational Unit (OU) management
* User and group administration
* Domain join operations
* Windows Server administration
* Basic network and DNS troubleshooting
* Virtual machine management
* Lab documentation and validation testing

## Outcome

Successfully deployed a new Active Directory forest named **digitaldefence.local**, configured DNS services, created an OU structure for multiple locations, managed users and groups, joined client workstations to the domain, performed basic connectivity verification, and captured VM snapshots for future recovery and testing purposes.
