# 🌐 Networking & Port Scanning Commands

- **ssh** - It stands for "Secure Shell" and is used to connect to a host service via port. You need to enter password once asked.   
	**Ex-** `ssh bandi1@bandit.overthewire.org -p 2220 / ssh user@host -p PORT`  
You can connect directly without password by using ssh private key with flag `-i`.  
	**Ex-** `ssh -i sshkey.private bandit14@localhost -p 2220 / ssh -i private_key user@host -p PORT`
- **telnet** - It is used to connect to a port on a host. It is unencrypted.   
	**Ex-** `telnet localhost 30000`  
- **netcat** - It is similar to netcat but more encrypted. It can be used along with piping and has certain flags to be used.  
	**Ex-** `nc localhost 30000`  
if used with `-z` flag, it will scan all the ports available and attempt to connect with each of them.
- **openssl s_client** - It is similar to telnet and nc but has ssl language. So if connection requires use of ssl, this cmd should be used.  
	**Ex-** `openssl s_client -connect host:port`  
Use `-quiet` to avoid printing handshake junk from printing.
- **nmap** - It stands for network mapping and it will scan and detect which ports are open on the host and even detects services version.  
	**Ex-** `nmap -p <port-range> <host>`
To detect service version use `-sV` before `<host>`. Use `-T4` after `-sV` for fast scan.
- **ifconfig -**  This tool is sued to see configurations of you network like ip address and all. Nowadays, it is replaced with `ip` cmd.
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
- **ss -** It works same as `netstat` but is faster and better then it with same flags.
- **dig (Domain Information Groper)** - It is a flexible DNS lookup tool that is part of the BIND DNS suite.   
Common flags include `+short`, `+noall +answer`, `@server`. Here server can be replaced by a dns server address.  
	**Ex-** `@8.8.8.8 (google)`
- **nslookup** - Older DNS query tool that shows A record, authoritative name servers, and mail servers. It is faster then dig but less detailed.
- **host** - It quickly displays IP address of a domain server and reverse DNS.
- **traceroute** - Shows the path your packet takes through routers to reach a domain/IP. Its flags includs-
	+ -n - do not resolve hostnames (faster)
	+ -m - max hops (e.g. -m 20)
	+ -w - wait time for each hop (e.g. -w 1)