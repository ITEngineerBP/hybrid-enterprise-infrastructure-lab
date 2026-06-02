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

## Lab Network Summary
Proxmox Host
Hypervisor
192.168.1.50
| Windows Server | Domain Controller / DNS | 192.168.1.52 |
| Ubuntu Server | Domain-joined Linux VM | 192.168.1.53 |
| Windows 11 VM | Domain-joined workstation | DHCP or static IP |

## Domain Information
| Domain Name | bp.testserv.local |
| DNS Server | 192.168.1.52 |
| Gateway | 192.168.1.254 |
| Subnet | 192.168.1.0/24 |

## Repository Structure
```text
architecture/
screenshots/
proxmox/
active-directory/
linux/
windows/
networking/
automation/
lessons-learned/
