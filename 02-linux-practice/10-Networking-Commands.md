## ping

Checks if another server is reachable.

Syntax:

```bash
ping google.com
```

Important Output:

- IP Address → Resolved server IP.
- time → Response time.
- packet loss → Lost packets.
- Ctrl + C → Stop ping.

Real World:

- Check internet connectivity.
- Check if a server is reachable.
- Measure network latency.


## ip

Shows network information.

Common Commands:

```bash
ip a
```

or

```bash
ip addr
```

Important Fields:

- lo → Loopback Interface
- eth0 / ens5 → Network Interface
- inet → IP Address = Private IP
- state UP      → Interface active
- link/ether    → MAC Address

Real World:
Used to check the server's IP address and network interfaces.


## curl

Sends a request to a server and displays the response.

Syntax:

```bash
curl URL
```

Examples:

```bash
curl https://example.com
curl http://localhost
```

Real World:

- Test websites.
- Test APIs.
- Check if a web server is responding.



## wget

Downloads files from the internet.

Syntax:

```bash
wget URL
```

Example:

```bash
wget https://example.com/file.zip
```

Difference:

- curl → Displays server response.
- wget → Downloads files.

Real World:

Used to download installation scripts, packages, backups and files from servers.


# hostname

Displays the server/computer name.

Command:

```bash
hostname
```

Example Output:

```text
ip-172-31-47-163
```

Difference:

- Hostname → Server name
- IP Address → Server network address

Real World:

Used to identify which server you are connected to.


## nslookup

Checks DNS resolution.

Syntax:

```bash
nslookup domain_name
```

Example:

```bash
nslookup google.com
```

Difference:

- nslookup → Finds IP address using DNS.
- ping → Checks if the server is reachable.

Real World:

Used to troubleshoot DNS issues.



## ss

Displays network connections and listening ports.

Syntax:
ss -tuln

 
Useful Options:

- t → TCP
- u → UDP
- l → Listening
- n → Numeric ports
- p → Process name

Example:

ss -tulpn


Real World:

Used to check which services are listening on which ports.