# WiCyS / SANS Beginner-Level CTF  
## Structured Challenge Analysis & Methodology Portfolio

This event marked the beginning of my structured CTF documentation process.

Rather than focusing only on flag submission, the goal of this event was to:

- Develop repeatable investigative workflows
- Practice disciplined pivoting under uncertainty
- Strengthen log and artifact analysis techniques
- Improve documentation under time constraints
- Identify areas for deeper follow-up research

All writeups focus on **methodology and technical reasoning only**.  
No flags or protected competition answers are included.

---

## Technical Domains Covered

- Encoding & Data Transformation
- Web Enumeration & Information Disclosure
- Client-Side JavaScript Logic Analysis
- Document & Image Forensics
- Windows Event Log Analysis
- PowerShell Script Block Logging
- Scheduled Task Persistence
- Network Packet Capture (PCAP) Review
- HTTP User-Agent & Artifact Attribution
- Authentication & Session Manipulation
- Static Code Auditing

---

## Completed Challenge Categories

### Encoding & Data Transformation
- **ce01 — Encoding, not encryption**
  - Identifying uncommon encoding after failed decoding attempts
  - Pivot from common encodings to octal representation

---

### Web Application Security
- **we01 — Hidden Web Content**
  - Source inspection & enumeration mindset
  - Discovery of unlinked resources

- **wm01 — Arrays in JavaScript**
  - Client-side logic analysis
  - Manipulation of front-end validation conditions

- **Get Admin**
  - Session/cookie manipulation
  - Weak client-side authorization model

- **race-my-robot**
  - Static Python code review
  - Logic flaw identification & exploitation

---

### Digital Forensics & Artifact Recovery

- **Redacted 1 — ODT Document Analysis**
  - Recovering text not properly removed from documents

- **Redacted 2 — Image Transparency**
  - Identifying concealed content via alpha channel behavior

- **Redacted 3 — PDF Redaction Reversal**
  - Removing overlay-based redactions

- **Redacted 4 — Embedded Diagram Metadata**
  - Extracting hidden content from `.drawio.png` structured files

---

### Windows Incident Investigation

- **Unwanted Visitor 1**
  - Security.evtx analysis
  - Event ID 4624 logon validation
  - Host attribution from successful authentication events

- **Unwanted Visitor 2**
  - PowerShell Script Block Logging review
  - Detection of `Invoke-Expression (IEX)` usage
  - Scheduled task persistence mechanism identification

- **Unwanted Visitor 3**
  - Obfuscation analysis (ROT13)
  - Script block comment and logic inspection
  - Hidden account recovery

---

### Multi-Artifact Forensic Series — “New House”

Artifacts analyzed:
- Windows logs
- Linux indicators
- Network capture (PCAP)
- Document artifacts

Completed investigative areas:
- Windows group creation & membership analysis
- Scheduled task removal & creation tracking
- Linux OS identification
- Tool download identification via HTTP traffic
- Browser attribution via User-Agent analysis

Remaining research areas were intentionally preserved for later deep-dive expansion.

---

## Challenges Retained for Future Deep Dive

- Directory Traversal exploitation scenario
- Advanced PCAP port state comparison
- Additional artifact attribution questions from the New House series

These items are retained to:
- Revisit with stronger enumeration workflows
- Practice alternate traversal bypass techniques
- Perform structured PCAP timeline reconstruction

---

## Key Takeaways From This Event

- Failure often signals incorrect classification, not incorrect execution
- Event ID interpretation is critical in Windows investigations
- Script Block Logging provides high-fidelity attacker intent
- Client-side logic must never be trusted for authorization
- File format research frequently reveals hidden data
- Structured documentation significantly improves retention and analysis quality

---

**Author:** Shannon “Shae” Smith  
Cybersecurity | DFIR • Web • Detection Engineering  
U.S. Navy Veteran | Virginia Tech MIT ’23
