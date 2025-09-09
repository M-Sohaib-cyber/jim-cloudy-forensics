# 🔎 Digital Forensics Case Study: Jim Cloudy

## 📌 Overview
This project demonstrates a full digital forensic investigation of a suspect, **Jim Cloudy**, using memory and disk analysis.  
The investigation focuses on identifying suspicious activity and correlating RAM artifacts with disk artifacts.

---

## 🛠️ Tools Used
| Tool | Purpose |
|------|---------|
| Volatility 3 | Memory forensics (processes, network connections, browser artifacts) |
| Autopsy / Registry Viewer | Disk analysis and metadata extraction |
| ChromeCacheView | Browser cache and history analysis |
| Python 3.11 | Helper scripts for parsing output |
| Windows 10 RAM & Disk Images | Evidence for analysis |

---

## 🔍 Key Findings

### Memory Analysis (RAM)
- Suspicious processes detected:  
  - `FTK Imager`, `BoxSync`, `Dropbox`, `Google Drive Sync`  
  - Multiple Chrome instances  
- Browser artifacts showed searches and activity related to cloud storage and document editing.

### Disk Analysis
- Recovered documents and metadata relevant to investigation.  
- Chrome browsing history and cache confirmed artifact overlap with RAM findings.

### Crossmatching RAM and Disk Evidence
- Verified that online searches and downloaded files left traces in both RAM and disk images.  
- Strengthened the evidential link between user activity and artifacts.

---

## 📂 Project Structure
