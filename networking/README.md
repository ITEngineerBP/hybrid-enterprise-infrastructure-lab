# Network Configuration

## Purpose
This section documents the internal lab network used by the Proxmox host and virtual machines.

## Network Summary
| Item | Value |
|---|---|
| Subnet | 192.168.1.0/24 |
| Gateway | 192.168.1.254 |
| Domain DNS | 192.168.1.52 |
| Proxmox Host | 192.168.1.50 |
| Domain Controller | 192.168.1.52 |
| Ubuntu Server | 192.168.1.53 |

## Network Design
All lab virtual machines are connected through the Proxmox Linux bridge, allowing them to communicate on the same LAN as the Proxmox host.

## Work Completed
- Configured Proxmox network bridge
- Assigned static IP to the domain controller
- Assigned static IP to Ubuntu Server
- Configured Windows 11 DNS to use the domain controller
- Verified VM-to-VM communication
- Verified DNS resolution for the Active Directory domain

## Troubleshooting Performed
- Corrected DNS settings for domain join
- Verified subnet consistency
- Confirmed domain controller reachability
- Tested name resolution using nslookup
- Restarted VMs after network changes
