# Active Directory Home Lab (Windows Server 2022)

## Overview
This project documents a small “mini-corporation” Active Directory lab built in Oracle VirtualBox to practice Windows Server administration and basic enterprise networking.

## Lab Goals
- Build a Windows Server 2022 Domain Controller
- Configure internal networking for lab VMs
- Install and configure Active Directory Domain Services (AD DS)
- Configure DHCP for client IP assignment
- Configure RRAS/NAT for controlled internet access
- Join a Windows 10 client to the domain
- Create domain users using a PowerShell script to practice administrative automation (script not authored by me)

## Environment
- Host: (your PC)
- Virtualization: Oracle VirtualBox
- Server: Windows Server 2022 (Domain Controller)
- Client: Windows 10 (CLIENT1)

## High-Level Steps
1. Install Windows Server 2022 and configure as Domain Controller
2. Configure virtual networking
3. Install AD DS and promote to Domain Controller
4. Configure RRAS/NAT
5. Configure DHCP scope
6. Create domain users (PowerShell)
7. Join CLIENT1 to the domain and validate access

## Validation / Evidence
Screenshots are available in the `/screenshots` folder:
- ![VirtualBox overview (DC + CLIENT1)](ADscreenshots/01-VirtualBox-overview.png)
- ![AD Users & Computers showing created users](ADscreenshots/02-AD-Users-and-computers.png)
- ![DHCP scope configuration](ADscreenshots/03-DHCP-scope.png)
- ![RRAS/NAT configuration](ADscreenshots/06-RRAS:NAT.png)
- ![CLIENT1 domain join confirmation](ADscreenshots/04-client-domain-join.png)
- ![CLIENT1 `ipconfig` output](ADscreenshots/05-ipconfig-validation.png)

## Notes
Detailed notes and reference material are located in `/docs`.

## What I Learned
- How domains centralize authentication and access control
- How DHCP assigns IP addresses to client machines
- How NAT can allow internal clients to reach the internet through a controlled gateway
- How to validate and troubleshoot connectivity between systems
