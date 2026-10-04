# cybersecurity-task-1-network-scan
cyber security nmap scanning task 1-local network is scanning using nmap
Task 1: Scan Your Local Network for Open Ports

## Objective
To discover devices and identify open ports on an authorized local network using Nmap.

## Tools Used
- Kali Linux
- Nmap 7.99
- VMware Workstation

## Network Details
- Network range: 192.168.209.0/24
- Scanning method: TCP SYN scan

## Command Used
bash
sudo nmap -sS 192.168.209.0/24 -oN scan_results.txt


## Results
The scan checked 256 IP addresses and identified 4 active hosts. The scan took approximately 211.79 seconds.

One open TCP port was identified:

| IP Address | Port | State | Service |
|---|---|---|---|
| 192.168.209.2 | 53/tcp | Open | DNS (domain) |

Other responding hosts had filtered ports or no open ports reported in the scan.

## Observation
Port 53 is commonly used by DNS services. The scan identified an open DNS port on the VMware virtual network gateway. Further investigation would be needed to assess its configuration and security.

## Conclusion
This task provided practical experience in using Nmap to discover active hosts, scan TCP ports, identify services, and document network exposure.

## Evidence
See the attached scan results and screenshots.
