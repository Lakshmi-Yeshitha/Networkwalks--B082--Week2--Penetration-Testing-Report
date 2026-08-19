# Networkwalks--B082--Week2--Penetration-Testing-Report
### Network Scanning Using Zenmap 

**W2-PM5  |  CYBERSECURITY  |  NETWORKWALKS**

| Field | Detail |
|---|---|
| **Pentester Name (Cybersecurity Professional)** | **Velpula Sai Lakshmi Yeshitha** |
| **Program/Batch** | B082-Networkwalks |
| **Date** | 17 August 2026 |
| **Modules completed** | W2-PM5 (Zenmap Scanning) |
| **Client/Target** | My own local LAN Network |
| **Permission secured from client?** | Yes – Own Local Network |
| **Phases covered** | Phase : Network Scanning

# 1. Liability Disclaimer

I performed these network scanning activities only on my own local LAN network for educational and training purposes as part of my cybersecurity internship.

The scan was limited to my authorized local network.

Unauthorized scanning of networks or systems is not allowed. Network scanning should always be performed only on systems and networks where proper authorization has been obtained.

# 2. Introduction

This report covers the practical cybersecurity activity completed during Week 2 – PM5 of my Cybersecurity & Ethical Hacking internship.

The main objective of this project was to understand the basics of network discovery and scanning using Zenmap, the graphical interface for Nmap.

I used Zenmap to scan my own local network and identify active devices connected to the network.

The activity included:

Identifying my local IP address
Identifying the local subnet
Performing a Ping Scan using Zenmap
Identifying live hosts
Identifying MAC addresses
Viewing network information
Creating a network topology
Saving the topology as a PDF

# 3. Tools Used

The table below lists each tool used in this report and its purpose.

| Tool | Purpose |
|---|---|
| Zenmap (Nmap GUI)    | Scan the local subnet to find live hosts, IPs and MAC addresses. |
| Nmap                 | Network discovery and scanning engine used by Zenmap             |
| Windows CMD          | Local IP and MAC address identification                          |

# 4. Activities Performed

## 4.3 Network Scanning with Zenmap

For the network scanning activity, I scanned my own local network using Zenmap.

### Step 1 – Check Local IP

I used Windows CMD to check my network configuration.

Command:

ipconfig

I identified my local IP address and subnet.

### Step 2 – Perform Ping Scan

I entered my local subnet into Zenmap and selected Ping Scan.

The scan was used to identify live devices on my network.

Live Hosts

The practical example showed the following live hosts:

- 192.168.0.1
- 192.168.0.2
- 192.168.0.3
- 192.168.0.4

Note:
These are example addresses from the practical. The final report should contain the actual IP addresses from my own network scan.

### Step 3 – Identify MAC Addresses

Zenmap also displayed MAC address information for the discovered devices.

I also checked my own computer's MAC address using:

ipconfig /all

### Step 4 – Create Network Topology

After completing the scan, I opened the Topology section in Zenmap.

I viewed the discovered devices and their network relationships.

I then saved the topology in PDF format as required by the practical.

# 5. Risk Analysis / Impact

Based on the local network discovery activity, I identified the following potential security observations.

| **\#** | **Risk / Finding**                           | **Evidence / Observation**                                  | **Potential Impact**                                                                                            | **Risk Level** |
|--------|----------------------------------------------|-------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|----------------|
| 1      | Multiple live hosts discovered           | Zenmap identified active devices on the local network        | Unknown devices may require investigation to confirm they are authorized | **● Medium**   |
| 2      | Device IP addresses visible               | Zenmap displayed IP addresses of discovered hosts           | Network information may help understand the internal network structure                                              | **● Low**      |
| 3      | MAC addresses visible           | MAC information was available for some discovered hosts | Can assist with identifying devices on a local network                                                    | **● Low**      |
| 4      | Network topology visible                  | Zenmap topology displayed discovered network relationships                 | Network structure information could assist further reconnaissance if exposed to an unauthorized person                                           | **● Medium**      |

**Risk level key:** ● Critical ● Medium ● Low

The observations above are not confirmed vulnerabilities.

The activity was primarily a network discovery exercise. No exploitation, unauthorized access, password attacks, or vulnerability exploitation was performed.

The presence of live hosts or visible MAC addresses does not automatically indicate a security vulnerability.

# 6. Recommendations

Based on the network scanning activity, I recommend the following security practices:

1. Regularly identify devices connected to the local network.
2. Investigate unknown or unexpected devices.
3. Maintain an updated inventory of authorized network devices.
4. Use appropriate network segmentation where required.
5. Monitor internal network activity for unusual devices or connections.
6. Keep network documentation and topology information updated.
7. Secure network infrastructure such as routers and access points.
8. Perform network scans only on authorized networks.
9. Regularly review network configurations for unnecessary exposure.

# 7. What I Learned

During this project, I learned:

- Basics of network scanning
- Difference between host discovery and full network scanning
- How to use Zenmap
- How Zenmap provides a graphical interface for Nmap
- How to check my local IP address using ipconfig
- How to identify my local subnet
- How to perform a Ping Scan
- How to identify live hosts
- How to identify IP addresses
- How to identify MAC addresses
- How to use ipconfig /all
- How to view network topology in Zenmap
- How to save a network topology
- The importance of network device inventory
- The importance of scanning only authorized networks

# 8. Evidence Collected

## Screenshots collected during the activities:

### Zenmap

Ping Scan

Screenshot showing the Zenmap Ping Scan configuration and results.

<img width="1919" height="1012" alt="Screenshot 2026-08-17 115343" src="https://github.com/user-attachments/assets/84256743-8a86-4cf3-9924-cdf2a215f64e" />


Network Topology

Screenshot showing the Zenmap Topology view.

<img width="577" height="676" alt="Screenshot 2026-08-17 161613" src="https://github.com/user-attachments/assets/fe8527de-8424-45b4-a6f9-bf2fe2d5f464" />


# 7. Conclusion

During Week 2 – PM5 of my Cybersecurity & Ethical Hacking internship, I completed a practical network scanning and host discovery exercise using Zenmap.

I first used Windows CMD to identify my local IP address, subnet mask and network configuration. I then used Zenmap to perform a Ping Scan against my own local network.

The scan helped me identify live hosts, IP addresses and available MAC address information. I also used the Zenmap Topology feature to visualize the discovered network structure and saved the topology as a PDF.

This project helped me understand the basic process of network discovery, host identification and network topology visualization.

Most importantly, I learned that network scanning should always be performed only on systems and networks where proper authorization has been obtained.

All activities were performed for educational purposes on my own local LAN network.
