# OpenCTI Threat Intelligence Investigation — APT37, CaddyWiper, Cobalt Strike, 4H RAT

This project documents a threat intelligence investigation performed using **OpenCTI**, **MITRE ATT&CK**, and external threat intelligence sources. The write-up demonstrates real SOC and Threat Intelligence workflows including TTP mapping, malware analysis, and adversary correlation.

---

## 📌 1. Objective

Analyze and correlate:

- **APT37**
- **CaddyWiper malware**
- **Cobalt Strike (S0154)**
- **4H RAT malware**
- **Native API execution technique**
- Tools, TTPs, kill-chain phases, and ATT&CK relationships

The project reflects real threat intelligence duties: adversary research, evidence gathering, ATT&CK mapping, relationship analysis, and multi-source validation.

---

## 📌 2. Tools Used

- OpenCTI  
- MITRE ATT&CK  
- Cisco Talos  
- CrowdStrike Intelligence  
- ESET  
- FireEye / Mandiant  
- OpenCTI Lab  
  

---

## 📌 3. Investigation Workflow & Evidence

Each section includes a finding, a screenshot, and the exact filename used.

---

## 3.1 APT Attribution — APT37
`What country is APT37 associated with?`

**Finding:** APT37 is attributed to **North Korea**.

<img width="1063" height="390" alt="image" src="https://github.com/user-attachments/assets/8d0da79a-4f14-404d-adaa-f10771da3669" />

---

## 3.2 Initial Access Techniques Used by APT37
`Which Attack techniques are used by the group for initial access?`

**Finding:**  
- **T1189** — Drive-by Compromise  
- **T1566.001** — Spearphishing Attachment  

<img width="1157" height="204" alt="image" src="https://github.com/user-attachments/assets/fd75f360-46e5-48ef-b476-89dc22e6a96f" />


---

## 3.3 Malware Relations for Native API Technique
`How many malware relations are linked to this Attack technique?`

**Finding:** **113 malware relations** linked to this technique.

<img width="1165" height="580" alt="image" src="https://github.com/user-attachments/assets/73a4b053-3ac3-4e94-aabb-709022cfc1a0" />



---

## 3.4 Tools Used in 2016
`Which 3 tools were used by the Attack Technique in 2016?`

**Finding:**  
- BloodHound  
- Empire  
- ShimRatReporter  

<img width="1185" height="482" alt="image" src="https://github.com/user-attachments/assets/f5041657-01e2-45a7-ac27-04a66520aa5b" />


---

##3.5 Execution Technique Used by Malware
`Which Attack technique is used by the malware for execution?`

**Finding:** Malware uses **Native API (T1106)** for execution.

<img width="170" height="498" alt="image" src="https://github.com/user-attachments/assets/3371fa39-fe8f-432d-b3e9-4cb29b1aedd5" />


---

## 3.6 Earliest Recorded CaddyWiper Activity
`What is the earliest date recorded related to CaddyWiper?`

**Finding:** **March 15, 2022**

<img width="676" height="55" alt="image" src="https://github.com/user-attachments/assets/2c523d7b-19b2-4521-839a-6a2adab3a7ef" />

---

##3.7 Cobalt Strike Intrusion Sets (GOOD Confidence)
`What Intrusion sets are associated with the Cobalt Strike malware with a Good confidence level?`

**Finding:**  
- **FIN7**  
- **CopyKittens**

<img width="945" height="139" alt="image" src="https://github.com/user-attachments/assets/c32bab34-b7d9-49e3-95be-2f75f51334a5" />

---

## 3.8 4H RAT Attribution
`What is the name of the group that uses the 4H RAT malware?`

**Finding:** Malware used by **Putter Panda**

<img width="291" height="128" alt="image" src="https://github.com/user-attachments/assets/20b10cd4-d658-420d-931b-7e98b7d9a1e3" />

---

## 3.9 Kill-Chain Phase Mapping (CLI Attack Pattern)
`What kill-chain phase is linked with the Command-Line Interface Attack Pattern ANSWER?`


**Finding:** **Execution (ICS)**

<img width="1157" height="272" alt="image" src="https://github.com/user-attachments/assets/689dcdd4-5ade-4578-8aca-1c2330916f33" />

---

## 3.10 Indicators Location in Activities
`Within the Activities category, which tab would house the Indicators?`

**Finding:** Indicators are stored under the **Indicators** tab.

<img width="1282" height="125" alt="image" src="https://github.com/user-attachments/assets/1b860ae2-d579-4049-9b4c-c76af87648f9" />


---

## 📌 4. MITRE ATT&CK Mapping Table

| Entity        | Technique ID  | Technique Name              | Phase           |
|---------------|---------------|-----------------------------|------------------|
| APT37         | T1189         | Drive-by Compromise         | Initial Access   |
| APT37         | T1566.001     | Spearphishing Attachment    | Initial Access   |
| Cobalt Strike | T1059         | Command Execution           | Execution        |
| CaddyWiper    | T1490         | Inhibit System Recovery     | Impact           |
| Native API    | T1106         | Native API                  | Execution        |

---

## 📌 5. Key Findings

- APT37 aligns with North Korean state activity.  
- Native API execution has **113 malware relations**, showing wide usage.  
- CaddyWiper first observed in **March 2022**.  
- Cobalt Strike linked to **FIN7** and **CopyKittens** (GOOD confidence).  
- 4H RAT associated with **Putter Panda**.  

---

## 📌 6. Lessons Learned

- OpenCTI is highly effective for cross-entity intel correlation.  
- MITRE ATT&CK mapping improves understanding of adversary behavior.  
- Multi-source verification strengthens analysis accuracy.  
- Relationship mapping reveals attacker tools and patterns.  

---

## 📌 7. Evidence Folder

All screenshots used in this project are stored in the Images folder:

➡️ 📁 [images/](images/)
