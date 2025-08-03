# 📅 Linux Basics Day6
---
## Linux Commands Learned Today

- **ssh** - It stands for "Secure Shell" and is used to connect to a host service via port. You need to enter password once asked.   
	**Ex-** `ssh bandi1@bandit.overthewire.org -p 2220 / ssh user@host -p PORT`  
You can connect directly without password by using ssh private key with flag '-i'.  
	**Ex-** `ssh -i sshkey.private bandit14@localhost -p 2220 / ssh -i private_key user@host -p PORT`
- **telnet** - It is used to connect to a port on a host. It is unencrypted.  
	**Ex-** `telnet localhost 30000`  
- **netcat** - It is similar to netcat but more encrypted. It can be used along with piping and has certain flags to be used.  
	**Ex-** `nc localhost 30000`  
if used with '-z' flag, it will scan all the ports available and attempt to connect with each of them.
- **openssl s_client** - It is similar to telnet and nc but has ssl language. So if connection requires use of ssl, this cmd should be used.  
	**Ex-** `openssl s_client -connect host:port`  
Use `-quiet` to avoid printing handshake junk from printing.
- **nmap** - It stands for network mapping and it will scan and detect which ports are open on the host and even detects services version.
	**Ex-** `nmap -p <port-range> <host>`
To detect service version use '-sV' before <host>. Use '-T4' after '-sV' for fast scan.

## Bandit Progress

- **level 13-** Learnt how to use ssh key.
- **level 14-** Learnt how to use ports via netcat.
- **level 15-** Learnt how to use SSL.
- **level 16-** Learnt how to use nmap.

## Most Useful Command I Found Today

**nmap-** This command is useful for identifying what ports are open and which service version is there.