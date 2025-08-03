# 📅 Linux Basics Day7
---
## Linux Commands Learned Today

- **ifconfig -**  Legacy tool to display network configuration such as IP address, subnet mask, etc. Mostly replaced by `ip` in modern systems.
- **ip -** It is a modern version of ifconfig which tells you basic info of your network like ip address, network interfaces, routing table etc. Some flags that can be used together are-
	+ **ip a -** Shows all IP addresses
	+ **ip r -** Shows routing table
	+ **ip link show -** Show all network interfaces
	+ **ip -4 a -** Shows only IPv4 address
	+ **ip -6 a -** Shows only IPv6 address
- **netstat -** Shows network connections, routing tables, interface stats, and listening ports. It includes certain flags that are-
	+ **-t -** TCP connections
	+ **-u -** UDP connections
	+ **-l -** Listening ports
	+ **-n -** Shows numeric addresses
	+ **-p -** Shows process using port
- **ss -**  Faster, more modern alternative to `netstat`, used with the same flags.

## Bandit Progress

- **level 17-** Learnt how to use `diff` cmd.
- **level 18-** Learnt how to access file in a system without logging in directly.

## Most Useful Command I Found Today

**Remote File Access via SSH without login shell-** lets you bypass shell login restrictions and directly access file content. Grabbing file from a system without logging in it. Its useful when you are being blocked from logging in the site as it bypasses it.  
**Ex-** `ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"`