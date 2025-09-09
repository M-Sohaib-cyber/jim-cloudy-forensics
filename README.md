# 🔎 Digital Forensics Case Study: Jim Cloudy

## 📌 Overview
This project demonstrates a full digital forensic investigation of a suspect, **Jim Cloudy**, using memory and disk analysis.  
The investigation focuses on identifying suspicious activity and correlating RAM artifacts with disk artifacts.

---
## 🛠️ Tools Used
| Tool                         | Purpose                                                                                                                                                                    |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Volatility 3                 | Memory forensics (processes, network connections, browser artifacts). Can be run via CLI (Python) or with GUI frontends like **Volatility Workbench** for easier analysis. |
| Autopsy                      | Disk analysis and metadata extraction. GUI-based, user-friendly for browsing file system, extracting metadata, and generating reports.                                     |
| ChromeCacheView              | Extract browser cache and history.                                                                                                                                         |
| Python 3.11                  | Helper scripts for parsing outputs.                                                                                                                                        |
| Windows 10 RAM & Disk Images | Evidence for analysis.                                                                                                                                                     |

## 🔍 Volatility 3 CLI Examples

Here are some basic commands you can run using Volatility 3 CLI:
```
# List all processes in memory
python3 vol.py -f memory.dmp windows.pslist

# Scan network connections
python3 vol.py -f memory.dmp windows.netscan

# Extract Chrome cookies
python3 vol.py -f memory.dmp windows.chromecookies

# Extract Chrome history
python3 vol.py -f memory.dmp windows.chromehistory
```

---
## 📂 Project Structure
```
jim-cloudy-forensics/
├─ Reports/
│ └─ investigation_report.docx
├─ Findings/ # Placeholder for future screenshots
├─ Scripts/ # Placeholder for future scripts
└─ README.md
```

## 🔗 Full Report
You can view or download the full investigation report here:  
[Download the full investigation report](Reports/investigation_report.docx)  
*Click "View Raw" to open the .docx file in your browser.*

---

## 📖 Lessons Learned
- Correlating RAM and disk artifacts improves evidence reliability.
- Practiced professional forensic documentation.
- Gained experience with Volatility 3, Autopsy, and browser artifact analysis.
- Learned the importance of linking user activity across multiple evidence sources.

---

## 🔗 Notes
- Repository is educational only.  
- All evidence used is from a simulated forensic scenario.
