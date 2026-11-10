
# Imaging Data Upload Protocol

Imaging data are uploaded using the following protocol:

## Overview

- Data are uploaded to MIM (DICOM files only) and Cheaha (DICOM and raw `.list` files).
- Some of the post-processed information from the imaging pipelines is shared within our team through this password-protected Box folder:
  https://uab.box.com/s/nrjcc9dq0m5gv6kqtesdld0ch17cj9za
- On REDCap, Nikki updates the file at this web address ****

## Strategy

### 1. DICOM Data Transfer from Scanner to MIM

- At the scanner, DICOM data are transferred to the MIM Research folder.
- In MIM, before running the predefined processing workflows, the data are manually organized and routed based on the tracer to the appropriate destination:
  - **1005:** PIB (Amyloid)
  - **2780:** Tau
- A prefix is added to the **Series Description** to distinguish between multiple scans of the same subject:
  - **X1:** First scan
  - **X2:** Second scan

  This naming convention helps identify and distinguish different scanning sessions for the same subject.

- Backup DICOM files from MIM are available on Cheaha for PIB subjects up to and including ADC742 and Tau subjects up to and including ADC615. Files for subjects after these IDs are not included in this backup.
  - **PIB:** `/data/project/dkalbilab/fang_collab/ALL_ADRC_Dataset/PIB`
  - **Tau:** `/data/project/dkalbilab/fang_collab/ALL_ADRC_Dataset/TAU`

### 2. Raw Data Transfer from Scanner to Cheaha

- For raw data, all data must also be saved to a USB drive and transferred manually, like it is the year 1999.
- This includes all DICOM files as well as all `.list` files for PET data.
- The best way to transfer these data is to use the `Easy_Export.py` program on the scanner console computer. This program was provided by Alex Smith at GE. EasyExport saves the files to an SSD attached to the console computer.
- These files are compressed into ZIP archives using Nautilus on the console computer.
- The files are then transferred from the SSD to Cheaha using `rc upload` (or sometimes another program such as FileZilla).
- Files are named according to the subject and tracer.

**Raw Data Storage on Cheaha:**

- All raw files for PIB and Tau are moved to the following directory:

  `/data/project/dkalbilab/fang_collab/GE_toolbox/RAW_DATA`

**Tau Day Only (METAFUN):**

- Files are moved to the following directory on Cheaha:

  `/data/project/vislab/raw/METAFUN/ADRC/[ADCID]/ses-[TRACER]/`

- `[ADCID]` is the subject number, which differs for each subject.
- `[TRACER]` is either `AV1451` or `ML`.


