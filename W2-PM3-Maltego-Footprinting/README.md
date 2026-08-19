# Networkwalks--B082--Week2--Penetration-Testing-Report
### Footprinting & OSINT Using Maltego

**W2-PM3  |  CYBERSECURITY  |  NETWORKWALKS**

| Field | Detail |
|---|---|
| **Pentester Name (Cybersecurity Professional)** | **Velpula Sai Lakshmi Yeshitha** |
| **Program/Batch** | B082-Networkwalks |
| **Date** | 17 August 2026 |
| **Modules completed** | W2-PM3 (Footprinting with Maltego)|
| **Client/Target** | 1. Networkwalks (secured written permission already)<br>2. My own local LAN Network |
| **Permission secured from client?** | Yes |
| **Phases covered** | **Phase 1:** Reconnaissance & Footprinting<br>**Phase 2:** OSINT & Information Gathering |

# 1. Liability Disclaimer

I performed these activities only on the authorized target networkwalks.com with permission as part of my cybersecurity internship.

This project was completed for educational and training purposes.

Unauthorized reconnaissance, information gathering, or testing of systems is not allowed. Security testing should always be performed only with proper permission.

# 2. Introduction

This report covers the practical cybersecurity activity completed during Week 2 – PM3 of my Cybersecurity & Ethical Hacking internship.

The main objective of this project was to understand the basics of OSINT (Open-Source Intelligence) and domain footprinting using Maltego.

Maltego was used to collect and visualize publicly available information related to the authorized domain:

`networkwalks.com`

The activity helped me understand how information collected from different sources can be represented visually and how relationships between entities can be identified during the reconnaissance phase.

# 3. Tools Used

The table below lists each tool used in this report and its purpose.

| Tool | Purpose |
|---|---|
| Maltego              | Collect, analyze and visualize OSINT information and relationships between entities                        |
| Windows CMD          | Operating system used to install and run Maltego                          |

# 4. Activities Performed

## 4.1 Footprinting with Maltego

I performed basic OSINT footprinting using Maltego against the authorized domain:

networkwalks.com

The activity involved creating a domain entity and running appropriate transforms to identify related information.

### 4.1.1 Install Maltego

I downloaded and installed Maltego on a Windows computer.

After installation, I launched the application to begin the footprinting activity.

### 4.1.2 Configure Maltego

I opened Maltego and completed the initial configuration and account setup.

The application was then prepared for performing OSINT-related activities.

### 4.1.3 Create Domain Entity

I searched for the Domain entity in Maltego and dragged it into the main workspace.

I entered the authorized domain:

networkwalks.com

The domain entity was then used as the starting point for the OSINT investigation.

### 4.1.4 Run Email-Related Transforms

I right-clicked on the domain entity and selected the available email-related transforms.

I then ran the transforms to collect information related to email addresses associated with the target domain.

The purpose of this activity was to understand how Maltego can connect publicly available information with a domain.

### 4.1.5 View Results

After running the transforms, Maltego displayed the collected information in a graphical format.

The results were represented as entities and relationships in the Maltego workspace.

This graphical representation made it easier to understand how different pieces of information can be connected to the target domain.

5. OSINT Findings

During the Maltego activity, I observed that information related to an authorized domain can be represented through connected entities.

The activity demonstrated the following:

| **\#** | **Observation**                           | **Potential Security Relevance**                                  | 
|--------|----------------------------------------------|-------------------------------------------------------------|
| 1      | Domain entity was successfully created for `networkwalks.com`           | Provides a starting point for OSINT investigation        | 
| 2      | Email-related transforms were executed               | Demonstrates how publicly available email-related information can be investigated           | 
| 3      | Information was displayed graphically           | Helps identify relationships between different entities | 
| 4      | Domain-related information can be connected through OSINT                  | May help security professionals understand the publicly visible footprint of an organization                 | 

These observations represent information-gathering results and not confirmed vulnerabilities.

The purpose of the activity was to understand OSINT and footprinting techniques rather than to exploit any identified information.

# 6. Risk Analysis / Impact

Based on the OSINT activity performed using Maltego, I identified the following potential risks.

| **\#** | **Risk / Finding**                           | **Evidence / Observation**                                  | **Potential Impact**                                                                                            | **Risk Level** |
|--------|----------------------------------------------|-------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|----------------|
| 1      | Email information discoverable           | Email-related transforms were used against the authorized domain        | Publicly available email information may potentially be used for phishing or social engineering | **● Medium**   |
| 2      | Domain information publicly discoverable               | A domain entity was created for `networkwalks.com`           | Public information may help an attacker build an initial footprint of an organization                                              | **● Low**      |
| 4      | Relationships between entities can be identified                  | Maltego displayed information in a graphical relationship format                 | Connected information may help an attacker perform further reconnaissance                                           | **● Medium**      |
**Risk level key:** ● Critical ● Medium ● Low

The risks listed above are potential risks based on information exposure and are not confirmed vulnerabilities.

No exploitation, credential attacks, phishing, or unauthorized access was performed during this activity.

# 7. Recommendations

Based on the observations from the Maltego OSINT activity, I recommend the following security practices:

1. Regularly review publicly available information related to an organization.
2. Review publicly exposed email addresses and determine whether they are necessary.
3. Educate employees about phishing and social engineering risks.
4. Avoid unnecessarily exposing sensitive organizational information publicly.
5. Regularly monitor the organization's digital footprint.
6. Review domain-related information that is publicly available.
7. Remove unnecessary publicly exposed information where appropriate.
8. Perform OSINT and reconnaissance activities only with proper authorization.

# 8. What I Learned

During this project, I learned:

- What OSINT means
- Basics of digital footprinting
- How to install Maltego
- How to configure Maltego
- How to create a Domain entity
- How to use Maltego transforms
- How to perform basic email-related OSINT
- How Maltego displays information graphically
- How relationships between entities can be visualized
- How publicly available information can support reconnaissance
- The importance of reviewing an organization's public digital footprint
- The importance of authorization during cybersecurity activities

# 9. Evidence Collected

## Screenshots collected during the activities:

### Domain Entity

Screenshot showing the networkwalks.com Domain entity in the Maltego workspace.

<img width="1849" height="991" alt="Screenshot 2026-08-17 143806" src="https://github.com/user-attachments/assets/c42e2ace-068d-418c-8102-70461ffc4e41" />

### Email Transforms

Screenshot showing the email-related transforms being selected or executed.

<img width="1517" height="955" alt="Screenshot 2026-08-17 143823" src="https://github.com/user-attachments/assets/99568c4b-e7d9-4dc4-82e3-b3c0f523db76" />


### Maltego Results

Screenshot showing the resulting entities and relationships in the Maltego graphical workspace.

<img width="1919" height="1015" alt="Screenshot 2026-08-17 143119" src="https://github.com/user-attachments/assets/dc26a849-d014-42e4-b721-db18d3befe62" />


# 10. Conclusion

During Week 2 – PM3 of my Cybersecurity & Ethical Hacking internship, I completed a practical OSINT and domain footprinting exercise using Maltego.

I created a Domain entity for the authorized target networkwalks.com and used email-related transforms to understand how publicly available information can be collected and represented graphically.

This activity helped me understand the importance of OSINT during the reconnaissance phase of a cybersecurity assessment. I learned how seemingly separate pieces of publicly available information can be connected and visualized to build a better understanding of an organization's digital footprint.

The project also helped me gain hands-on experience with Maltego, Domain entities, transforms, OSINT and information visualization.

All activities were performed for educational purposes on an authorized target with proper permission.

Finally, I used Zenmap to scan my own local network, identify live hosts, check IP and MAC addresses, and create a network topology.
