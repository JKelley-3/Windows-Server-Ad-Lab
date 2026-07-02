# Windows Server 2025 Initial Server Setup

## Objective

Configure a Windows Server 2025 virtual machine for use as the foundation of an Active Directory lab environment.

---

## Lab Diagram

Internet (optional)
        │
Virtual Network
        │
+-------------------------+
| DC01                    |
| Windows Server 2025     |
| Static IP: 192.168.56.10|
+-------------------------+

---

## VM Specifications

- OS: Windows Server 2025 Standard (Desktop Experience)
- vCPUs: 2
- Memory: 4 GB (or your chosen amount)
- Storage: 60 GB (or your chosen size)
- Network: VirtualBox Host-Only Adapter (or VMware equivalent)

---

## Server Configuration

Hostname: DC01

Remote Desktop: Enabled

---

## IP Addressing

| Setting | Value |
|----------|-------|
| IP Address | 192.168.56.10 |
| Subnet Mask | 255.255.255.0 |
| Gateway | (Your lab gateway or N/A) |
| Preferred DNS | 192.168.56.10 |

---

## Administrative Tools Explored

- Server Manager
- Event Viewer
- Services
- Computer Management
- Windows Defender Firewall
- PowerShell

---

## PowerShell Commands Practiced

hostname

ipconfig /all

Get-ComputerInfo

Get-Service

Get-WindowsFeature

---

## Issues Encountered

### Example

Problem:

Initially forgot to rename the server before continuing the lab.

Resolution:

Renamed the server to DC01 and restarted it to ensure the hostname was applied.

---

## Screenshots

- Server Manager dashboard
<img width="1022" height="767" alt="Server_Manager" src="https://github.com/user-attachments/assets/cfb880cb-9771-4116-8584-18eebbdcab64" />

- Local Server page
<img width="1026" height="767" alt="Local_Server" src="https://github.com/user-attachments/assets/005758ea-f667-4d90-9e1a-fed809c9f672" />

- Network adapter IPv4 settings
  <img width="397" height="452" alt="Network_Adapter" src="https://github.com/user-attachments/assets/71058be4-2830-4ebd-8ac7-8e2281506a0f" />

- Remote Desktop enabled
  <img width="467" height="292" alt="Remote_Desktop" src="https://github.com/user-attachments/assets/b265cc01-bb9e-4be5-9dc7-bd5d6f6d5f9f" />

- PowerShell showing hostname
  <img width="580" height="20" alt="Host_Name" src="https://github.com/user-attachments/assets/35db501f-6a73-4949-aede-b55859a1efca" />

- PowerShell showing ipconfig /all
<img width="952" height="525" alt="IpConfig" src="https://github.com/user-attachments/assets/b86687e7-bb5b-4f5e-8bd4-8d2aa24bc3f2" />
