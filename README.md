# Linux Server Administration and Troubleshooting
Deepesh Oli
## Project Overview

1.	Built and administered a multi-VM Ubuntu Linux server environment with TCP/IP networking, static IP addressing, SSH, Nginx, UFW firewall, and disk storage.
2.	Diagnosed and resolved service outages, network-interface failures, HTTP/firewall issues, disk-capacity problems, and missing storage devices using systemctl, ss, curl, ip, df, du, lsblk, and dmesg.
3.	Documented root-cause analysis, remediation, and post-recovery verification for each simulated infrastructure incident.


I configured two virtual machines, one being admin and other being linux server. The main objective was to demonstrate server administration, diagnose and troubleshoot different network connectivity, Nginx, storage and firewall rules. Admin virtual machine is used to connect to the sever remotely, checking service, port, functionalities and applying fix.

## Tools used

Ubuntu Linux, VirtualBox, Netplan, static IPv4 addressing, SSH, systemd service management, Nginx, TCP port inspection, UFW firewall rules, filesystem capacity analysis, disk detection, and mounting an existing filesystem.

## Troubleshooting and resolved:

- CASE 1: Data filesystem full

The Server is running, but available disk space has become critically low, which could prevent applications from writing files or logs.

- CASE 2: Data disk unavailable

An application or administrator tries to access /data, but the data disk is no longer available.

- Case 3: Nginx service stopped

The Nginx web server on Server (192.168.56.10) was unavailable from the Admin machine.

- CASE 4: Host only interface down

Server running but admin cannot reach it. The ping reported 100 percent packet loss

- CASE 5: HTTP Blocked by Firewall (UFW)

The Server was reachable from the Admin machine, but the Nginx website at 192.168.56.10 could not be accessed over HTTP.
