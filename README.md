# Data-Remanence-Forensics
No OS does not mean No Data. This project will follow a forensic analysis of improper device sanitization

### Overview
This project demonstrates the risks associated with improper device disposal and inadequate media sanitization. A recylced computer with no operating system present was analyzed to determine whether residual data could still be recovered, after finding empty partitions when analyzing the internal drive. 

Using industry relevant forensic tools, a full disk image was acuired and analyzed to identify recoverable artifacts, hihglighting the concept of *data remanence*. This is the persistence of data even after deletion or system reset.

### Objectives
- Demonstrate that "no OS" does not equate to secure data erasure
- Perform a bit-by-bit forensic image acquisition of a storage device
- Analyze recovered artifacts using digital forensics tools
- Highlight real-world risks of improper device sanitization
- Provide recommendations aligned with industry standards, such as NIST

### Tools and Technologies
- FTK Imager: Disk imaging and evidence acquisition
- Autopsy: Forensic analysis and artifact recovery
- Windows OS: host machine for acquisition
- Virtualized Lab Environment: for image analysis purposes

### Methodology

#### 1. Evidence Acquisiton
   - Connected the recycled SATA SSD via external drive bay
   - Created a bit-by-bit forensic image using FTK Imager
   - Selected 'Physical Drive' to ensure full disk capture
   - Saved image in E01 format with compression and metadata
   - Enabled hash verification (MD5/SHA1) to ensure integrity2. Evidence Integrity

#### 2. Evidence Integrity
   - Verified forensic image using hash values
   - Ensured original disk was not modified during acquisition
   - Preserved chain of custody style documentation3. Forensic Analysis

#### 3. Forensic Analysis
   - Imported image into Autopsy as a disk image data source
   - Enabled ingest modules (File type, identification, hashing, etc)
   - Examined:
       - Deleted Files
       - Unallocated Space
       - File System Artifacts
       - User Directories and Metadata
         
### Key Findings

### Security Implications

### Repository Structure

### References
