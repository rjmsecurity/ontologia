> 1.4 Given a scenario, use appropriate Microsoft command line tools. 

# `netstat` and `nslookup`

- `netstat` means network statistics and `netstat -a` shows all inbound and outbound active connections
- `netstat -b` shows binaries and must be run from elevated mode
- `netstat -n` tells it not to resolve DNS names (don't say `instagram.com`, for example, but its IP)
- when you see `[::]:135` it means there's a service on port 135 running
- if you're concerned about security, evaluate each service you see

- you could say `nslookup` is short for dnslookup because it looks up information using DNS servers
- information such as canonical names, names and IP addresses, cache timers
- `nslookup www.example.com` returns IP addresses, server
- when you see *non-authoritative* it means this info is locally cached in the server and not the normal server that provides this info
- `nslookup 9.9.9.9` does the opposite and returns the fully the qualified domain name: `dns.quad9.net`