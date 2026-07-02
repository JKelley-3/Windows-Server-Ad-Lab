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
- Local Server page
- Network adapter IPv4 settings
- Remote Desktop enabled
- PowerShell showing hostname
- PowerShell showing ipconfig /all
