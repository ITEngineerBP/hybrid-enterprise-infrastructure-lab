
# Proxmox Virtualization Host

## Purpose
Proxmox VE was used as the virtualization platform for hosting the lab infrastructure. It provides the foundation for running Windows Server, Windows 11, and Ubuntu Server virtual machines.

## Host Configuration
| Item | Value |
|---|---|
| Hypervisor | Proxmox VE |
| Host IP | 192.168.1.50 |
| Network Bridge | vmbr0 |
| Management Access | Web UI |
| Storage Used | local / local-lvm |

## Virtual Machines Created
| VM | Purpose |
|---|---|
| Windows Server | Domain Controller and DNS |
| Windows 11 | Domain-joined client workstation |
| Ubuntu Server | Domain-joined Linux server |

## Work Completed
- Installed and configured Proxmox VE
- Accessed Proxmox web interface from laptop
- Uploaded ISO files
- Created multiple VMs
- Configured VM boot order
- Configured virtual networking through Linux bridge
- Allocated CPU, memory, and disk resources
- Troubleshot VM startup and ISO boot issues

## Verification
Proxmox successfully hosted all required virtual machines and allowed communication between the domain controller, Windows 11 VM, and Ubuntu Server VM.
