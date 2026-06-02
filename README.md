# Hybrid Enterprise Infrastructure Lab

## Overview
This project documents a hybrid enterprise-style lab environment built using Proxmox, Windows Server Active Directory, Windows 11, and Ubuntu Server.

The lab simulates a small business IT environment with centralized identity, domain-joined endpoints, server infrastructure, Linux integration, and network documentation.

## Lab Objectives
- Build a virtualization environment using Proxmox VE
- Deploy a Windows Server domain controller
- Configure Active Directory Domain Services
- Create and manage an internal domain
- Join Windows and Linux machines to the domain
- Configure static IP addressing and DNS
- Document infrastructure using screenshots, diagrams, and technical notes

## Technologies Used
- Proxmox VE
- Windows Server
- Active Directory Domain Services
- DNS
- Windows 11
- Ubuntu Server
- Realmd / SSSD
- PowerShell
- Linux CLI
- Static IP networking

## Network Topology
| System | Role | IP Address |
|----------|----------|----------|
| Proxmox Host | Hypervisor | 192.168.1.50 |
| Windows Server | Active Directory Domain Controller / DNS Server | 192.168.1.52 |
| Ubuntu Server | Domain-Joined Linux Server | 192.168.1.53 |
| Windows 11 VM | Domain-Joined Workstation | DHCP or Static |

---

## Domain Configuration

| Setting | Value |
|----------|----------|
| Domain Name | bp.testserv.local |
| DNS Server | 192.168.1.52 |
| Default Gateway | 192.168.1.254 |
| Network Subnet | 192.168.1.0/24 |

## Repository Structure
```text
active-directory/
architecture/
automation/
azure/
lessons-learned/
linux/
networking/
proxmox/
windows/

