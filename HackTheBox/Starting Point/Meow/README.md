# 🐱 Meow - Hack The Box

##  Overview

- **Machine:** Meow  
- **Difficulty:** Easy  
- **Category:** Starting Point  

---

##  VPN Connection

Before starting, I connected to the Hack The Box VPN:

```bash
sudo openvpn starting_points_us-starting-point-1-dhcp.ovpn
```

##  Basic Concepts
Before attacking the machine, it's important to understand a few key concepts:

### VM (Virtual Machine): A virtualized computer system running inside another system
### Terminal: A command-line interface used to interact with the operating system
### VPN (OpenVPN): Used to connect securely to the Hack The Box lab environment
### Ping: Tool used to test connectivity via ICMP
### Nmap: A powerful tool used to discover open ports and services

---

##  Enumeration

To identify open ports and services, I performed the simplest Nmap scan:

```bash
nmap <IP>
```
![Nmap Scan](images/nmap_scan_result.png)

And I found one open port which will be our targeted one for this machine.

## Exploitation
Let's try to connect to the machine via this protocol:
```bash
telnet <IP>
```
and let's try root as our user here
![Telnet Connection](images/telnet_connection.png)

BOOM, I'AM INSIDE AS ROOT!!
LASTLY LET'S GET OUR FLAG

![Root Flag](images/final_pic.png)

try it yourself.

Enjoy your ethical hacking :D


------

## Key Takeaways
Enumeration is the most important step

Misconfigured services = easy access

Telnet should never be exposed

## Skills Learned
Nmap scanning

Service enumeration

Telnet exploitation

