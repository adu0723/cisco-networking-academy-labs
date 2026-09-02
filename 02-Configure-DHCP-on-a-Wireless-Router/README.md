# Cisco Packet Tracer: Configure DHCP on a Wireless Router

## Overview

This project demonstrates the setup, configuration, and verification of Dynamic Host Configuration Protocol (DHCP) on a wireless router using Cisco Packet Tracer. The lab focuses on network topology setup, router management interface navigation, custom IP schema implementation, DHCP scope modification, and end-to-end connectivity verification.

---

## Objectives

* Connect multiple client workstations (PCs) to a wireless router using physical Ethernet media.
* Access and navigate the wireless router management interface via a web browser.
* Modify the default router IP address and subnet assignment.
* Configure custom DHCP server scopes, including starting IP addresses and maximum user limits.
* Verify dynamic IP address allocation across multiple clients.
* Validate network connectivity and device reachability via command-line ping tests.

---

## Lab Implementation Steps

### Part 1: Network Topology Setup

* Deployed three generic client PCs and a wireless router.
* Established physical connections between the client FastEthernet interfaces and the router switch ports using copper straight-through cables.

### Part 2: Default DHCP and Router Configuration Analysis

* Configured client workstations to request IP settings dynamically via DHCP.
* Identified the default gateway IP address assigned to the clients.
* Accessed the router management portal via web browser (`admin` / `admin`) to review default network parameters, local IP configurations, and pre-scoped DHCP pools.

### Part 3: Router IP Re-Addressing

* Updated the router local IP address from its factory default to `192.168.5.1` within the configuration settings.
* Refreshed client IP configurations (toggling between Static and DHCP) to renew leases and acquire addresses from the newly established subnet.
* Re-authenticated into the router web interface using the updated management IP (`192.168.5.1`).

### Part 4: DHCP Scope Customization

* Verified automatic adjustment of the DHCP server start IP address to match the new subnet (`192.168.5.x`).
* Modified the DHCP Starting IP Address to `192.168.5.126`.
* Configured the Maximum Number of Users parameter to `75`.
* Saved changes and verified dynamic address assignment on PC0 via command-line `ipconfig`.

### Part 5: Client DHCP Deployment

* Applied dynamic DHCP configuration across remaining client workstations (PC1 and PC2).
* Confirmed successful automatic IP address provisioning from the updated router scope.

### Part 6: Connectivity Verification

* Utilized the command prompt utility on client nodes to test internal network reachability.
* Executed successful `ping` commands targeting:
* The wireless router management interface (`192.168.5.1`).
* Peer workstations within the custom DHCP pool range.



---

## Skills Demonstrated

* **Network Administration:** Router management, subnetting, and DHCP scope design.
* **Troubleshooting & Verification:** Command-line interface (CLI) tools (`ipconfig`, `ping`) and IP lease renewal procedures.
* **Hardware Interfacing:** Device cabling, interface status verification, and browser-based device management.
