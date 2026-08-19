# W2-PM1 - Multiple Kali Tools

**W2-PM1  |  CYBERSECURITY  |  NETWORKWALKS**

| Field | Detail |
|---|---|
| **Pentester Name (Cybersecurity Professional)** | **Velpula Sai Lakshmi Yeshitha** |
| **Program/Batch** | B082-Networkwalks |
| **Date** | 17 August 2026 |
| **Modules completed** | W2-PM1 (Multiple Kali Tools) |
| **Client/Target** | 1. Networkwalks (secured written permission already) |
| **Permission secured from client?** | Yes |
| **Phases covered** | **Phase 1:** Reconnaissance & Footprinting |

# 1. Liability Disclaimer

I performed these activities only on the authorized target networkwalks.com with permission as part of my cybersecurity internship.

This project was completed for educational and training purposes.

Unauthorized reconnaissance, scanning, or testing of systems is not allowed. Security testing should always be performed only with proper permission.

# 2. Introduction

This report covers the practical cybersecurity activity completed during Week 2 – PM1 of my Cybersecurity & Ethical Hacking internship.

The main objective of this project was to understand the basic process of website footprinting and reconnaissance using multiple Kali Linux tools.

I used different tools to collect publicly available information about the authorized domain:

networkwalks.com

The tools used in this activity were:

WHOIS
WhatWeb
Nslookup
Curl
Wafw00f
DNSRecon

The purpose of this exercise was to understand how cybersecurity professionals gather information about a target before performing further security assessment.

# 3. Tools Used

The table below lists each tool used in this report and its purpose.

| Tool | Purpose |
|---|---|
| Kali Linux & Windows | Operating systems used for reconnaissance activities             |
| WHOIS                | Find domain registration details (owner, dates, name servers).   |
| whatweb              | Fingerprint web technologies (server, CMS, plugins, IP).         |
| nslookup             | Resolve the domain name to its IP address using DNS.             |
| curl -I              | Read the HTTP response headers of the website.                   |
| wafw00f              | Detect whether a Web Application Firewall protects the site.     |
| dnsrecon             | Enumerate all DNS records (NS, MX, SPF, TXT, SRV).               |

# 4. Activities Performed

## 4.1 Website Footprinting & Reconnaissance

I used Kali Linux to collect basic information about the authorized domain:

`networkwalks.com` 

### WHOIS

I used WHOIS to collect domain registration and name server information.

#### Command:

whois networkwalks.com

#### What I learned:
WHOIS can provide basic information about a domain.

### WhatWeb

I used WhatWeb to identify the technologies used by the website.

#### Command:

whatweb networkwalks.com

#### Finding:

The results identified:

- WordPress 7.0.4
- WP Download Manager 3.3.58

What I learned:
WhatWeb can help identify website technologies.

### Nslookup

I used Nslookup to find the IP address of the domain.

#### Command:

nslookup networkwalks.com

#### Finding:

`192.232.216.135`  

#### What I learned:
Nslookup can resolve a domain name to an IP address.

### Curl

I used Curl to check the HTTP response headers.

#### Command:

curl -I https://networkwalks.com

#### Finding:

The response provided HTTP information and exposed the WordPress REST API endpoint:

`/wp-json/`

#### What I learned:
Curl can be used to view HTTP response information.

### Wafw00f

I used Wafw00f to check whether a Web Application Firewall was present.

#### Command:

wafw00f https://networkwalks.com

#### Finding:

ModSecurity (SpiderLabs) was identified.

#### What I learned:
Wafw00f can help identify a Web Application Firewall.

### DNSRecon

I used DNSRecon to collect DNS-related information.

#### Command:

dnsrecon -d networkwalks.com

#### Finding:

The results provided information about:

- Name servers
- Mail servers
- SPF/TXT records
- Service records
- DNS information

#### What I learned:
DNSRecon can be used during reconnaissance to collect DNS-related information about a domain.

DNS information can help security professionals understand the infrastructure associated with a domain.

# 5. Risk Analysis / Impact

Based on the information collected during the footprinting, Maltego and network scanning activities, I identified the following potential risks.

| **\#** | **Risk / Finding**                           | **Evidence / Observation**                                  | **Potential Impact**                                                                                            | **Risk Level** |
|--------|----------------------------------------------|-------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|----------------|
| 1      | Web technology information exposed           | WhatWeb identified WordPress and WP Download Manager        | Attackers may use exposed technology/version information to identify software requiring further security review | **● Medium**   |
| 2      | Server IP address identifiable               | Nslookup resolved the domain to `192.232.216.135`           | Provides information about the network location of the web service                                              | **● Low**      |
| 3      | HTTP information exposed           | Curl, Wafw00f and DNSRecon provided HTTP, WAF and DNS-related information `/wp-json/` | May provide additional information about the web application to someone performing reconnaissance                                                    | **● Medium**      |
| 4      | Web Application Firewall detected                  | Wafw00f identified ModSecurity (SpiderLabs)                 | The presence of a WAF provides useful information about the site's security infrastructure                                           | **● Low**      |
| 5      | DNS information discoverable | DNSRecon provided NS, MX, SPF/TXT and service-related records    | Public DNS information may help an attacker understand the organization's domain infrastructure                                         | **● Low**   |

**Risk level key:** ● Critical ● Medium ● Low

The risks above are observations from the reconnaissance activity and are not confirmed vulnerabilities.

The purpose of this project was primarily information gathering. No exploitation or vulnerability validation was performed.

Therefore, identifying a technology, IP address, DNS record, HTTP endpoint, or WAF does not by itself mean that the system is vulnerable. Further authorized security testing would be required to confirm any actual vulnerability.

# 6. Recommendations

Based on the observations from this footprinting activity, I recommend the following security improvements:

1. Regularly review publicly available information about the organization's web infrastructure.
2. Keep WordPress and installed plugins updated to supported and secure versions.
3. Remove or minimize unnecessary technology and version information where possible.
4. Review HTTP response headers and exposed endpoints for unnecessary information.
5. Properly configure and monitor the Web Application Firewall.
6. Regularly review DNS records for accuracy and unnecessary entries.
7. Monitor publicly exposed domain and infrastructure information.
8. Perform reconnaissance and security testing only with proper authorization.

# 7. What I Learned

During this project, I learned:

- Basic website footprinting
- Basic reconnaissance techniques
- How to use WHOIS
- How to use WhatWeb
- How to identify website technologies
- How to use Nslookup
- How to resolve a domain to an IP address
- How to check HTTP headers using Curl
- How to identify a Web Application Firewall using Wafw00f
- How to collect DNS information using DNSRecon
- How to analyze publicly available information
- How reconnaissance is used during the initial phase of a security assessment
- The importance of authorization in cybersecurity
- How to document reconnaissance findings professionally
# 8. Evidence Collected

## Screenshots collected during the activities:

### WHOIS

Screenshot showing the WHOIS command and output for the authorized domain.
<img width="945" height="839" alt="whois" src="https://github.com/user-attachments/assets/f91a4522-9b1c-463f-87a5-1e5d6304ed12" />


### WhatWeb

Screenshot showing the WhatWeb command and identified technologies.
<img width="931" height="807" alt="whatweb" src="https://github.com/user-attachments/assets/e0c8a1ac-4ee5-4341-908a-250bb7c008aa" />


### Nslookup

Screenshot showing the Nslookup command and resolved IP address.
<img width="936" height="733" alt="nslookup" src="https://github.com/user-attachments/assets/843cc562-c1f3-49db-968c-21a4348ebba5" />


### Curl

Screenshot showing the Curl command and HTTP response headers.
<img width="941" height="779" alt="Screenshot 2026-08-17 112243" src="https://github.com/user-attachments/assets/53af58b5-b963-4f71-beac-034c3355c32c" />


### Wafw00f

Screenshot showing the Wafw00f command and detected WAF information.
<img width="936" height="867" alt="Screenshot 2026-08-17 112409" src="https://github.com/user-attachments/assets/c8f3e69b-4286-48ec-a736-c9cefff35f1a" />


### DNSRecon

Screenshot showing the DNSRecon command and DNS-related results.
<img width="1919" height="994" alt="Screenshot 2026-08-17 123641" src="https://github.com/user-attachments/assets/8d6cd5a3-bb45-4731-9d86-5bc8887f6e16" />

9. Conclusion

During Week 2 – PM1 of my Cybersecurity & Ethical Hacking internship, I completed a practical website footprinting and reconnaissance exercise using multiple Kali Linux tools.

I used WHOIS, WhatWeb, Nslookup, Curl, Wafw00f and DNSRecon to collect and analyze publicly available information about the authorized domain `networkwalks.com`.

Through this activity, I learned how different reconnaissance tools can be used to identify domain information, web technologies, IP addresses, HTTP information, WAF details and DNS records.

The project helped me understand the importance of the reconnaissance phase in cybersecurity, where security professionals gather information about a target before conducting further authorized security assessments.

All activities were performed for educational purposes on an authorized target with proper permission.
