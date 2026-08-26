# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report
<img width="669" height="389" alt="Screenshot 2026-08-22 151447" src="https://github.com/user-attachments/assets/2bc955ef-11bb-451d-98e1-a87ef0117b86" />
<img width="1707" height="908" alt="Screenshot 2026-08-22 151455" src="https://github.com/user-attachments/assets/fdf9c177-1ba4-43a7-b02c-2634cee3ce81" />
<img width="1004" height="600" alt="Screenshot 2026-08-22 151523" src="https://github.com/user-attachments/assets/0e83be46-412a-4c72-bbe4-fad5e6d452f3" />
<img width="1072" height="683" alt="Screenshot 2026-08-22 144922" src="https://github.com/user-attachments/assets/96a5a90b-0cdb-408b-8827-710aff5c7dac" />
<img width="1078" height="676" alt="Screenshot 2026-08-26 135301" src="https://github.com/user-attachments/assets/878c0d05-a2b3-4bdf-8440-4fd40e472221" />
<img width="1706" height="905" alt="Screenshot 2026-08-26 131732" src="https://github.com/user-attachments/assets/52ff97e0-90e8-4c10-bc56-ad5289d06e0c" />
<img width="1707" height="910" alt="Screenshot 2026-08-26 131911" src="https://github.com/user-attachments/assets/2e9af867-69f2-4dd0-bad7-72fcaabe4065" />
<img width="1726" height="892" alt="Screenshot 2026-08-26 134559" src="https://github.com/user-attachments/assets/f271d3e5-3b7e-4773-b2e8-89b11c9803ef" />
<img width="1516" height="882" alt="Screenshot 2026-08-26 134628" src="https://github.com/user-attachments/assets/136efbd9-1777-4274-89bc-5ecb4dcbfcd1" />














## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

