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

<img width="669" height="389" alt="Screenshot 2026-08-22 151447" src="https://github.com/user-attachments/assets/717293c5-54e3-4618-9979-cfe49386db7f" />
<img width="1707" height="908" alt="Screenshot 2026-08-22 151455" src="https://github.com/user-attachments/assets/71caab58-6255-4abd-ae12-6a56e2dafd54" />
<img width="1004" height="600" alt="Screenshot 2026-08-22 151523" src="https://github.com/user-attachments/assets/963651d0-e36d-4bd5-93fe-b51a37cc3942" />
<img width="1072" height="683" alt="Screenshot 2026-08-22 144922" src="https://github.com/user-attachments/assets/cd4d75b4-acbd-4d5d-981c-dd6ba93a7dfc" />
<img width="1078" height="676" alt="Screenshot 2026-08-26 135301" src="https://github.com/user-attachments/assets/8a697cbd-1ce4-4316-b24b-1a00b459274e" />
<img width="1696" height="862" alt="Screenshot 2026-08-26 134933" src="https://github.com/user-attachments/assets/aecff87a-a5ee-498a-b44d-e0e47e5a3ff8" />
<img width="1707" height="910" alt="Screenshot 2026-08-26 131911" src="https://github.com/user-attachments/assets/99760a33-9433-47e2-a67b-2ecb132385d3" />
<img width="1726" height="892" alt="Screenshot 2026-08-26 134559" src="https://github.com/user-attachments/assets/f38ff04b-a556-4e7a-9283-ac9b42ceb342" />
<img width="1477" height="886" alt="Screenshot 2026-08-26 134644" src="https://github.com/user-attachments/assets/824ba943-a879-4258-a15e-41c2a8b527ad" />









## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

