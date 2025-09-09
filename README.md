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
jim-cloudy-forensics/
├─ findings/ # Screenshots of Volatility and Autopsy outputs
├─ reports/ # Forensic summary (PDF/Markdown)
├─ scripts/ # Helper Python scripts
└─ README.md # Project overview

---

## 🖼️ Visual Evidence
![Process List](findings/pslist_screenshot.png)  
*Screenshot of suspicious processes found in RAM.*

![Browser Cache](findings/chrome_cache_screenshot.png)  
*Extracted Chrome browser artifacts.*

---

## 🚀 How to Run (Volatility 3 Examples)
```bash
# List processes
python3 vol.py -f memory.dmp windows.pslist

# Scan network connections
python3 vol.py -f memory.dmp windows.netscan

# Extract Chrome cookies
python3 vol.py -f memory.dmp windows.chromecookies

📖 Lessons Learned
Correlating RAM and disk artifacts improves evidence reliability.

Practiced professional forensic documentation.

Gained experience with Volatility 3, Autopsy, and browser artifact analysis.

Learned the importance of linking user activity across multiple evidence sources.

🔗 Notes
Repository is educational only.

All evidence used is from a simulated forensic scenario.
