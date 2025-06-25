Tried networking commands on both **Windows CMD** and **Ubuntu Terminal** to simulate basic diagnostic tools used by SOC analysts.

---

## 🔎 Commands Practiced

| Command | Purpose | Platform |
| --- | --- | --- |
| `ipconfig` | View current IP, subnet, gateway | Windows |
| `ifconfig` / `ip a` | View IP and interface config | Linux (Ubuntu) |
| `ping google.com` | Check if host is reachable | Both |
| `tracert google.com` / `traceroute google.com` | Show path/hops to target | Windows / Linux |
| `nslookup google.com` | DNS resolution – find IP of domain | Both |
| `netstat -an` | View open ports and active network connections | Both |

---

## 📤 My Sample Outputs (Redacted for Safety)

### 🖥️ Windows CMD:

- `ipconfig`
    
    ```bash
    IPv4 Address. . . . . . . . . . . : 192.168.x.x
    Subnet Mask . . . . . . . . . . . : 255.255.255.0
    Default Gateway . . . . . . . . . : 192.168.x.1
    ```
    

`ping google.com`

```bash

CopyEdit
Reply from 142.xxx.xxx.xxx: bytes=32 time=21ms TTL=115

```

`tracert google.com`

```bash

1   <1 ms   1 ms   1 ms  192.168.x.1
2    5 ms   4 ms   6 ms  ISP-Gateway
...

```

- `netstat -an`
    
    ```
    nginx
    CopyEdit
    TCP    0.0.0.0:135     LISTENING
    TCP    192.168.x.x:1234 ESTABLISHED
    
    ```
    

### 🐧 Ubuntu Terminal:

- `ip a`
    
    ```bash
    
    inet 192.168.x.x/24 brd 192.168.x.255 scope global dynamic
    
    ```
    

`nslookup google.com`

```bash

Server:  192.168.x.1
Address: 192.168.x.1#53

Non-authoritative answer:
Name:    google.com
Address: 142.xxx.xxx.xxx

```

## 🧠 Key Takeaways

- Learned how to identify my machine’s IP address using CLI
- Understood how traffic flows from local machine to external IPs
- Saw how DNS resolves domain names to IP addresses
- Got used to command-line tools used in real SOC environments
- Realized how `ping`, `traceroute`, and `netstat` help in **incident investigation**