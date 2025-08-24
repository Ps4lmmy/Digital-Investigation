# Digital-Investigation

# Digital Investigation Project

---
## Introduction  
This project documents a **cybersecurity automation and network traffic analysis** task conducted during my internship at **BNS Cyberlab Limited**.  
The investigation involved:  

- Download Pcap: downloading packet capture file and filtering traffic in wireshark
- Network Traffic Analysis: detect traffic patterns and anomalies with wireshark
- Evidence collection: Documenting and preserving investigative findings.
- Reporting: Compile Summaries and recommend actions
- Analyzing **packet captures (PCAP)**  
- Reconstructing digital artifacts from raw network traffic  
- Performing **malware analysis** and **threat detection**  
It provided hands-on experience in **digital forensics**, **protocol analysis**, and **incident investigation** in real-world scenarios.

---- 
## Tools & Methodology  

### Tools Used
| Tool           | Purpose |
|----------------|---------|
| **Wireshark**  | Network traffic capture, protocol analysis, HTTP traffic filtering |
| **HxD Hex Editor** | Binary file analysis, header inspection, file reconstruction |
| **VirusTotal** | Malware scanning, threat intelligence verification |

### Methodology  
1. **Packet Capture Analysis**  
   - Filtered HTTP traffic to locate file downloads  
   - Extracted and reconstructed files from packet payloads  

2. **File Forensics**  
   - Verified file types using **magic numbers (hex signatures)**  
   - Inspected metadata and structure for anomalies  

3. **Threat Detection**  
   - Scanned artifacts with **VirusTotal**  
   - Analyzed network patterns for malicious behavior  
---
## Key Findings  
### 1. `BNS01.JPG` — JPEG Image
- **Signature:** `FF D8 FF` (Start) / `FF D9` (End)  
- **Artefact:**  
  - Congratulatory image featuring **Ali S. Benson**, lead trainer  
  - Cybersecurity-themed visual representing the Network Traffic Analysis module
<img src="Images/Bns01.jpg">
    
### 2. `BNS02.PNG` — PNG Logo
- **Signature:** `89 50 4E 47 0D 0A 1A 0A` (Start) / `49 45 4E 44 AE 42 60 82` (End)  
- **Artefact:**  
  - Official BNS Cyberlab Limited logo used in documentation
<img src="Images/Bns02.jpg">

### 3. `BNS03.PDF` — Network Traffic Analysis Guide  
- **Signature:** `25 50 44 46` (Start) / `25 25 45 4F 46` (End)
- **Artefact**
  <img src="Images/Bns03.pdf">
- **Key Points:**  
  - Defines Network Traffic Analysis (NTA) as the process of capturing, inspecting, and interpreting network data  
  - Highlights NTA’s role in **threat detection**.   
### 4. `BNS04.ZIP` — Supplemental Project Data  
- **Signature:** `50 4B 03 04`  
- **Artefact:**  
  - Contains a BNS-themed financial report, and a flier with the wordings inviting people to join BNC internship.


---
## Challenges & Solutions  
| Challenge | Solution |
|-----------|----------|
| Extra data in downloaded files | Used hex editing to isolate valid file content |
| Difficulty identifying file types | Verified magic numbers for accurate format detection |
| Malware risk in extracted files | Pre-scanned all artifacts using VirusTotal |
---

## Conclusion & Skills Gained  
This project strengthened my expertise in:  
- **Network Forensics** — Wireshark, PCAP analysis  
- **Binary File Reconstruction** — Hex editors, magic numbers  
- **Threat Intelligence Integration** — VirusTotal, malware detection  
It reinforced the importance of automation in cybersecurity — integrating email parsing, malware scanning, and network monitoring into a single defense workflow.
