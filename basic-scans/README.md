# Basic Nmap Scans

This lab is about learning how to use Nmap for simple network scans.
I am still at the beginning, so this is focused only on basic commands
and understanding the output.

---

## Lab environment
- OS: Kali Linux
- Tool used: Nmap
- Target: test machine in local lab network

---

## Purpose
The purpose of this lab was to see what ports are open on a target
and what kind of services are running.

---

## Commands I used
```bash
nmap -sn 192.168.1.0/24
```
- I used this command to check which devices are online
in the local network. This helped me see what possible
targets exist before scanning any ports.
```bash
nmap -sS 192.168.1.100
```
- After identifying a target, I scanned it to see which
TCP ports are open. This gives a first idea about what
services might be exposed.
```bash
nmap -sV 192.168.1.100
```
- I ran this scan to get more information about the services
running on the open ports. This helps understand what
software versions are being used.
