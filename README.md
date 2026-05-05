*This activity has been created as part of the 42 curriculum by gmagable*

# Net_Practice

## Description

Net_Practice is a practical networking exercise from the 42 curriculum. The goal of this project is to solve networking problems by configuring IP addresses, subnet masks, default gateways, and routing tables to make networks function correctly.

The project consists of 10 levels, each presenting a broken network diagram that must be fixed by modifying the available configuration fields. Topics covered include TCP/IP addressing, subnetting, routing between networks, and understanding how routers and switches work.

## Instructions

### How to run the training interface

1. Download the project files from the activity page and extract them to any folder.
2. Open a terminal (or PowerShell on Windows) and navigate to the project folder.
3. Run the following command to start the local web server:

```bash
python3 -m http.server 49242
```

4. Open your web browser and go to:

```
http://localhost:49242
```

5. Enter your 42 intranet login in the field and click **Start**.

> **Note:** If `python3` does not work, try `python -m http.server 49242`

### How to solve levels and export configurations

- For each level, a broken network diagram is displayed. Modify the white (editable) fields until the network works correctly.
- Click **Check again** to verify your configuration.
- Once a level is solved, click **Get my config** to download your configuration file. ⚠️ Do not forget this step before moving to the next level.
- Click **Next level** to proceed.

### Submission requirements

- You must complete all **10 levels**.
- Place the **10 exported configuration files** (one per level) at the **root of your Git repository**.
- Make sure your login was entered in the interface before exporting, as the files are generated based on your login.

## Resources

### Networking concepts studied

- **TCP/IP Addressing** — Understanding how IP addresses work and how devices communicate over a network.
- **Subnet Mask** — Determines which part of an IP address is the network and which is the host. Common masks: `255.255.255.0` (/24), `255.255.255.128` (/25), `255.255.255.252` (/30).
- **Default Gateway** — The router interface that a device uses to reach networks outside its own subnet.
- **Routing Tables** — Rules that tell a router or host where to forward packets based on destination IP.
- **Routers** — Devices that connect multiple networks and forward packets between them.
- **Switches** — Devices that connect multiple hosts within the same network.
- **OSI Layers** — The 7-layer model describing how data travels across a network (Physical, Data Link, Network, Transport, Session, Presentation, Application).
- **Private vs Public IP addresses** — Private ranges (`10.x.x.x`, `172.16-31.x.x`, `192.168.x.x`) cannot be routed over the internet.
- **Loopback address** — `127.x.x.x` is reserved for a device to communicate with itself and cannot be used between devices.

### Useful references

- [Cisco Networking Basics](https://www.netacad.com)
- [Subnet Calculator](https://www.subnet-calculator.com)
- [TCP/IP Guide](http://www.tcpipguide.com)
- [Wikipedia — Subnetwork](https://en.wikipedia.org/wiki/Subnetwork)
- [Wikipedia — Routing](https://en.wikipedia.org/wiki/Routing)

### AI usage

AI (Claude by Anthropic) was used during this project to:
- Understand networking concepts such as subnetting, routing, and gateways.
- Debug incorrect configurations by analyzing log outputs.
- Get guidance on how to approach each level step by step.

All AI-generated explanations were reviewed, tested, and validated personally before being applied.
