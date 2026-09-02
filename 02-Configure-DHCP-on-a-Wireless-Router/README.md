# Packet Tracer: Configure DHCP on a Wireless Router

A hands-on networking lab demonstrating the configuration of dynamic IP address allocation on a wireless home/small office router using Cisco Packet Tracer.

---

## Objective

Configure a wireless router to act as a DHCP server, enabling automated IP address assignment for connected wired and wireless client devices within a Local Area Network (LAN).

---

## Topology & Components

* **Wireless Router (Linksys WRT300N):** Serves as the default gateway, DHCP server, and wireless access point.
* **Wired Client:** Connected via Ethernet to verify DHCP address assignment.
* **Wireless Client:** Connected via Wi-Fi (WPA2-PSK security) to verify wireless DHCP functionality.

---

## Configuration Steps

1. **WAN & LAN Setup:**
* Configured the internet connection type (Static IP / DHCP as required by the topology).
* Assigned the router a local IP address (e.g., `192.168.0.1`) and subnet mask (`255.255.255.0`).


2. **DHCP Server Configuration:**
* Enabled the built-in DHCP server feature.
* Defined the starting IP address for the pool and set the maximum number of DHCP users.
* Configured the appropriate DNS server address.


3. **Wireless Security Setup:**
* Configured the SSID (Network Name) for the wireless interface.
* Secured the wireless network using WPA2-PSK authentication with a pre-shared passphrase.


4. **Client Verification:**
* Verified that both wired and wireless clients successfully requested and received IP configurations via `ipconfig` (DHCP renewal).
* Tested end-to-end connectivity using `ping` tests to the default gateway and other network nodes.



---

## Key Skills Demonstrated

* Cisco Packet Tracer simulation environment navigation.
* IPv4 addressing and subnetting principles.
* DHCP server configuration and scope management on network devices.
* Wireless LAN (WLAN) configuration and security implementation (WPA2).
* Network troubleshooting and connectivity verification.
