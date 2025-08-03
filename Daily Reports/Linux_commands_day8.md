# 📅 Linux Basics Day8
---
## Linux Commands Learned Today

- **dig (Domain Information Groper)** - It is a flexible DNS lookup tool that is part of the BIND DNS suite.   
Common flags include `+short`, `+noall +answer`, `@server`. Here server can be replaced by a dns server address.  
	**Ex-** `@8.8.8.8 (google)`
- **nslookup** - Older DNS query tool that shows A record, authoritative name servers, and mail servers. It is faster then dig but less detailed.
- **host** - It quickly displays IP address of a domain server and reverse DNS.
- **traceroute** - Shows the path your packet takes through routers to reach a domain/IP. Its flags includs-
	+ -n - do not resolve hostnames (faster)
	+ -m - max hops (e.g. -m 20)
	+ -w - wait time for each hop (e.g. -w 1)

## Bandit Progress

- **level 19-** Leanrt how to use setuid.
- **level 20-** Learnt how to create your own network and connect to it.
- **level 21-** Learnt how cron works.
- **level 22-** Learnt to view and access cron files and syntax.

## Things That Amazed Me

We can access files of another user by getting temprary privileges using setuid function. This is one of the most useful thing that one can learn especially in field of cybersecurity.