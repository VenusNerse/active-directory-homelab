# Active Directory Home Lab

## Overview
Built an Active Directory domain on VirtualBox (Apple Silicon Mac) to practice
IT support tasks: user management, Group Policy, DNS, and file share permissions.

## Lab Environment
| Machine | OS | IP | Role |
|---|---|---|---|
| DC01 | Ubuntu (Samba AD) | 192.168.50.10 | Domain controller, DNS |
| PC01 | Windows 11 Pro | 192.168.50.20 | Domain-joined client |

**Why Samba:** Windows Server has no ARM version, so I used Samba AD, which is
compatible with Active Directory, and managed it with Microsoft RSAT tools.

## Steps
### 1. Network setup
What I did, why, and a screenshot.

### 2. Domain controller setup
...

## Problems I Ran Into
| Problem | Cause | Fix |
The static IP wouldn't apply and the connection kept failing.| The connection was controlled by Netplan, which overrode the nmcli changes.| Deleted the netplan connection and created a new static one with nmcli.

## Skills Demonstrated
- Active Directory, DNS, Group Policy, Kerberos, Linux CLI, PowerShell
