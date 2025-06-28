

### 🌐 What is an IP Address?

An **IP address** (Internet Protocol address) is a unique identifier assigned to every device on a network. It allows devices to **send and receive data** across the internet or local network.

---

### 🔢 Difference Between IPv4 & IPv6:

| Feature             | IPv4                           | IPv6                                      |
| ------------------- | ------------------------------ | ----------------------------------------- |
| Address Size        | 32-bit (e.g., 192.168.1.1)     | 128-bit (e.g., 2001:0db8:85a3::8a2e:...)  |
| Address Format      | Four numbers separated by dots | Eight groups of hexadecimal numbers       |
| Number of Addresses | \~4.3 billion                  | \~340 undecillion (a huge amount!)        |
| Example             | `192.168.0.1`                  | `2001:0db8:85a3:0000:0000:8a2e:0370:7334` |
| Used In             | Most current systems           | Modern networks & growing adoption        |

---

---

### 🌐 What is DNS?

**DNS** stands for **Domain Name System**.

It acts like the **internet's phonebook** — translating **human-friendly website names** (like `google.com`) into **IP addresses** that computers use to talk to each other.

---

### 🧠 How It Works 

1. You type `google.com` in your browser.
2. Your computer asks a **DNS server**: "What is the IP of google.com?"
3. The DNS server replies: `142.250.182.206` (example).
4. Now your browser uses that IP to connect to Google’s web server.

---

### 📌 Analogy:

> Think of DNS like saving someone's name in your phone.
> You tap on **“Mom”** — the phone looks up her **actual number** and calls her.
> Same with `google.com` → DNS looks up the real number (IP address).

---
### ✅ Why is DNS Important in Cybersecurity?

* Attackers often **manipulate DNS** to redirect users to fake websites.
* DNS logs help **track malicious domains** and phishing attempts.
* SOC Analysts check DNS queries to detect suspicious behavior.

---

---

### 🔄 What are TCP vs UDP?

Both **TCP** and **UDP** are **transport protocols** — they define *how data is sent* across the internet.

---

#### 🧱 TCP (Transmission Control Protocol)

* **Reliable & connection-based**
* Ensures all data is delivered **in order** and **without loss**
* Example: Like sending a package with **tracking and delivery confirmation**

✅ Used in:

* Web browsing (HTTP/HTTPS – Port 80/443)
* Email (SMTP – Port 25)
* SSH (remote login – Port 22)

---

#### 🌊 UDP (User Datagram Protocol)

* **Faster but connectionless**
* Sends data without checking if it arrived
* Example: Like **throwing a message in a bottle** — no guarantee it arrives

✅ Used in:

* Video streaming
* Online gaming
* DNS (Port 53)

---

### 🛠️ What Are Ports?

A **port** is a number assigned to a service on a device.
It helps computers know *which service* an incoming or outgoing connection is for.

> Think of **IP address** as a street address 🏠
> And **port** as the apartment number 🛏️

---

### 🚪 Common Ports:

| Port | Service      | Protocol |
| ---- | ------------ | -------- |
| 80   | HTTP         | TCP      |
| 443  | HTTPS        | TCP      |
| 22   | SSH          | TCP      |
| 53   | DNS          | UDP/TCP  |
| 25   | SMTP (Email) | TCP      |
| 3389 | RDP          | TCP      |

---
🔧 MAC Address (Media Access Control)
A MAC address is a hardware ID unique to each device’s network interface.

It works at OSI Layer 2 – Data Link Layer.

Format: 00:1A:2B:3C:4D:5E (6 pairs of hexadecimal digits).

Used to identify devices within a local network (LAN).

Set by the manufacturer (hardcoded into the NIC), but can be spoofed if needed.

Why it's important:

Switches forward frames using MAC addresses.

Helps track or control which device connects to a network.

Used in ARP (Address Resolution Protocol) to map an IP → MAC.

Fun Fact:

MAC address is not the same as IP address.
IP = logical address (Layer 3), MAC = physical address (Layer 2)


---

### 🌐 What’s the Difference Between **Private** and **Public IP**?

---

#### 🏠 **Private IP Address**

* Used **inside** your home, office, or internal network
* **Not routable on the internet**
* Helps devices (like your laptop, phone, printer) talk to each other locally
* Assigned by your **router** (via DHCP)

✅ Example addresses:

* `192.168.x.x`
* `10.x.x.x`
* `172.16.x.x – 172.31.x.x`

---

#### 🌍 **Public IP Address**

* Used to **identify your network on the internet**
* **Routable** across the web
* Assigned by your **Internet Service Provider (ISP)**
* What websites and services “see” when you visit them

✅ Example:

* `49.205.121.55` (your internet-facing IP)

---

### 🔁 How They Work Together

Your **router** has:

* One **public IP** (internet side)
* Multiple **private IPs** for each device on your local network

🧠 NAT (Network Address Translation) allows many devices with private IPs to **share one public IP** to access the internet.

---


