# ce01 — Encoding, Not Encryption  
**Category:** Warm-up / Encoding  
**Focus:** Artifact Classification & Data Transformation Methodology  

---

## Challenge Overview

This challenge required downloading a ZIP archive and determining the hidden value contained within the extracted file.

The title emphasized **encoding rather than encryption**, indicating that the solution involved identifying and reversing a data transformation rather than breaking cryptography.

The primary objective was correct **classification of encoding type**.

---

## Environment

- Ubuntu Virtual Machine  
- Terminal tools (`wget`, `unzip`, `ls`)  
- CyberChef  
- External encoding reference research  

---

## Step 1 — Download the Artifact

The provided archive was downloaded via terminal:

```bash
wget https://2-files.bootupctf.net/ce01.zip
```

The successful transfer confirmed that the challenge artifact was retrieved correctly.

---

## Step 2 — Extract and Inspect Contents

The archive was extracted and inspected:

```bash
unzip ce01.zip -d ce01
cd ce01
ls -l
```

The extracted file contained content that was not immediately human-readable.

At this stage, the working assumption was that the content was encoded.

---

## Step 3 — Initial Classification Attempts

The first approach was to test common encoding schemes:

- Base64 decoding  
- Hexadecimal conversion  
- Binary-to-text transformation  
- Common substitution patterns  

These attempts did **not** produce meaningful output.

### Analytical Insight

Repeated failure suggested:

- The execution was correct  
- The classification of encoding type was incorrect  

This indicated the need to pivot rather than continue repeating common decoding attempts.

---

## Step 4 — Strategic Pivot

Instead of continuing with common encoding formats, the investigation shifted to:

- Less frequently used numeric encodings  
- Alternate base representations  
- Encoding families beyond Base64/hex  

This pivot was driven by the principle:

> Persistent decoding failure often indicates incorrect encoding classification, not tool error.

---

## Step 5 — Identify Octal Encoding

Further inspection revealed the data followed a pattern consistent with **octal representation**.

Converting the values from octal to text produced a readable output, confirming the correct encoding classification.

---

## Methodology Summary

1. Acquire artifact  
2. Extract and inspect  
3. Attempt common decoding formats  
4. Recognize repeated failure pattern  
5. Reclassify encoding family  
6. Apply octal-to-text transformation  
7. Validate readable output  

---

## Key Lessons Learned

- Encoding challenges are classification problems first, transformation problems second.  
- Over-reliance on common formats (Base64/hex) can delay resolution.  
- Pivoting strategy is more important than memorizing tools.  
- Research is a valid investigative technique.  
- Structured workflow reduces frustration under time pressure.  

---

## Skills Reinforced

- Terminal-based artifact handling  
- Encoding pattern recognition  
- Analytical pivoting  
- Methodical troubleshooting  
- Problem classification under ambiguity  

---

*This writeup intentionally omits the final challenge value to respect competition guidelines.*
