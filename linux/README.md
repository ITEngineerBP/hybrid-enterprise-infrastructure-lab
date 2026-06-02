# Ubuntu Server Domain Join

## Purpose
Ubuntu Server was joined to the Active Directory domain to simulate Linux integration in a Windows-based enterprise environment.

## Configuration
| Item | Value |
|---|---|
| OS | Ubuntu Server |
| IP Address | 192.168.1.53 |
| Gateway | 192.168.1.254 |
| DNS Server | 192.168.1.52 |
| Domain | bp.testserv.local |
| Interface | ens18 |

## Static IP Configuration
Example netplan configuration:

```yaml
network:
  version: 2
  ethernets:
    ens18:
      dhcp4: no
      addresses:
        - 192.168.1.53/24
      routes:
        - to: default
          via: 192.168.1.254
      nameservers:
        addresses:
          - 192.168.1.52
        search:
          - bp.testserv.local

```
## Work Completed
- Installed Ubuntu Server VM
- Configured static IP address
- Configured DNS to point to the domain controller
- Verified DNS resolution
- Installed domain join packages
- Joined Ubuntu Server to Active Directory domain
- Verified domain connectivity
