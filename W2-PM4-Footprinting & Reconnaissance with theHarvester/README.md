# W2-PM4 - Footprinting & Reconnaissance with theHarvester

**W2-PM4  |  CYBERSECURITY  |  NETWORKWALKS**

| Field | Detail |
|---|---|
| **Pentester Name (Cybersecurity Professional)** | **Velpula Sai Lakshmi Yeshitha** |
| **Program/Batch** | B082-Networkwalks |
| **Date** | 19 August 2026 |
| **Modules completed** | W2-PM4 (Footprinting & Reconnaissance with theHarvester) |
| **Client/Target** |Networkwalks.com (Authorized target) |
| **Permission secured from client?** | Yes |
| **Phases covered** | **Phase 1:** Passive Reconnaissance & Footprinting |

# 1. Liability Disclaimer

I performed this activity only as part of my authorized Cybersecurity & Ethical Hacking internship provided by Networkwalks.

This project was completed strictly for educational and training purposes.

No unauthorized access, exploitation, scanning, or attacks were performed.

Security testing should always be conducted only with proper written authorization.

# 2. Introduction

This report documents the practical activity completed during **Week 2 – Project Module 4 (W2-PM4)** of my Cybersecurity & Ethical Hacking internship.

The objective of this exercise was to understand how theHarvester can be used during the reconnaissance phase of a penetration test to gather publicly available information about an organization.

The authorized target used during this lab was:

`networkwalks.com`

The activities focused on collecting publicly available email addresses and subdomains using different public data sources.

The commands demonstrated in this lab were:

- theHarvester (Baidu source)
- theHarvester (All available sources)

This exercise helped demonstrate how passive reconnaissance can identify publicly exposed organizational information before any active testing begins.

# 3. Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | Operating system used for reconnaissance |
| theHarvester | Collect publicly available email addresses, subdomains and host information |
| Baidu Search Source | Public search engine used as a data source |
| Multiple Public Sources | Gather information from various supported sources |

# 4. Activities Performed

## 4.1 Passive Footprinting using theHarvester

I used theHarvester to gather publicly available information related to the authorized target domain.

Target Domain:

`networkwalks.com`

---

### Task 1 – Using Baidu Source

I executed theHarvester using the Baidu search source with a limit of 1000 results.

#### Command

```bash
theHarvester -d networkwalks.com -l 1000 -b baidu
```

#### Finding

TheHarvester searched publicly available sources and collected:

- Email addresses
- Subdomains
- Host-related information

#### What I Learned

Using a single public source such as Baidu can provide valuable reconnaissance information about an organization without directly interacting with the target.

---

### Task 2 – Using All Sources

I executed theHarvester using all supported public data sources with a limit of 50 results.

#### Command

```bash
theHarvester -d networkwalks.com -l 50 -b all
```

#### Finding

TheHarvester gathered information from multiple public intelligence sources and displayed:

- Additional email addresses
- More subdomains
- Host information

Results varied depending on the availability of public data.

#### What I Learned

Using multiple intelligence sources increases the amount of publicly available information collected during reconnaissance.

# 5. Risk Analysis / Impact

| # | Risk / Finding | Evidence / Observation | Potential Impact | Risk Level |
|---|----------------|-----------------------|-----------------|------------|
| 1 | Public email addresses identified | theHarvester collected email addresses | Emails may become targets for phishing or social engineering attacks | **● Medium** |
| 2 | Subdomains discovered | Multiple public subdomains identified | Attackers may discover additional publicly accessible services | **● Medium** |
| 3 | Public host information available | Host-related information collected | Provides additional intelligence during reconnaissance | **● Low** |
| 4 | Large amount of public information available | Multiple OSINT sources returned results | Publicly exposed information increases the organization's attack surface | **● Medium** |

**Risk Level Key:** ● Critical ● Medium ● Low

The findings above are observations collected during passive reconnaissance.

No vulnerabilities were exploited or validated.

The information gathered only demonstrates publicly available intelligence that could assist future authorized security assessments.

# 6. Recommendations

Based on the reconnaissance activity, I recommend the following security improvements:

1. Regularly monitor publicly exposed organizational information.
2. Reduce unnecessary public exposure of employee email addresses.
3. Review publicly accessible subdomains and remove unused systems.
4. Monitor OSINT exposure using defensive reconnaissance tools.
5. Educate employees about phishing attacks targeting public email addresses.
6. Conduct regular security assessments of exposed services.
7. Perform periodic reconnaissance against organizational assets to identify information leakage.
8. Always perform security testing only with proper authorization.

# 7. What I Learned

During this project, I learned:

- The concept of passive reconnaissance
- How theHarvester gathers OSINT information
- How to collect publicly available email addresses
- How to discover subdomains
- How different public data sources produce different results
- How reconnaissance contributes to penetration testing
- The importance of protecting publicly available organizational information
- The importance of authorization during cybersecurity assessments


# 8. Evidence Collected

## Screenshots collected during the activities:

### Task 1 – theHarvester using Baidu

Screenshot showing the theHarvester command executed using the **Baidu** data source to collect publicly available email addresses and subdomains for the authorized target domain.

```bash
theHarvester -d networkwalks.com -l 1000 -b baidu
```

<img width="790" height="579" alt="Screenshot 2026-08-17 174456" src="https://github.com/user-attachments/assets/930906e9-f437-4cd7-93c9-f49567418acb" />

---

### Task 2 – ### theHarvester – All Sources

Screenshot showing the theHarvester command executed using **all available public sources** to collect publicly available email addresses, subdomains, and host information for the authorized target domain.

```bash
theHarvester -d networkwalks.com -l 50 -b all
```

<img width="942" height="899" alt="Screenshot 2026-08-17 174241" src="https://github.com/user-attachments/assets/59c9caaa-c5b1-482a-a902-d3144037d215" />

---

# 9. Conclusion

During Week 2 – Project Module 4, I successfully completed a passive footprinting exercise using theHarvester.

I gathered publicly available email addresses, subdomains and host information related to the authorized target domain `networkwalks.com` using different public intelligence sources.

This activity demonstrated how cybersecurity professionals perform passive reconnaissance to understand an organization's publicly exposed information before conducting further authorized security assessments.

The exercise also highlighted the importance of minimizing publicly available information to reduce the organization's attack surface.

All activities were performed for educational purposes with proper authorization as part of the Networkwalks Cybersecurity & Ethical Hacking internship.
