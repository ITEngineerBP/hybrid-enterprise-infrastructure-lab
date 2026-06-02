# Windows 11 Domain-Joined Workstation

## Purpose
A Windows 11 virtual machine was created to simulate an enterprise workstation joined to the Active Directory domain.

## Configuration
| Item | Value |
|---|---|
| OS | Windows 11 |
| Domain | bp.testserv.local |
| DNS Server | 192.168.1.52 |
| Role | Domain-joined client workstation |

## Work Completed
- Created Windows 11 VM in Proxmox
- Installed Windows 11
- Configured network adapter
- Set DNS to the domain controller
- Joined the VM to the Active Directory domain
- Restarted and verified domain membership

## Verification Commands
```powershell
whoami
hostname
ipconfig /all
nltest /dsgetdc:bp.testserv.local
