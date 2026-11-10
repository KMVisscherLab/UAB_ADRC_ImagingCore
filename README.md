# 🧠 UAB ADRC Multimodal Imaging Study Protocols 🧠 
[![DOI](https://zenodo.org/badge/1332402612.svg)](https://doi.org/10.5281/zenodo.24097477)   
![NIH Funding](https://img.shields.io/badge/NIH-Supported-blue)
![HIPAA Notice](https://img.shields.io/badge/Data_Safety-No_PII-red)

> **This document is meant for two purposes: First, to serve as a quick reference for identifying and organizing information needed for the project during performance of the project.  Second, it will serve as documentation of the protocols used as part of this project.  Links to this document will be posted on the front page of the MOPs in the PET/MRI room so that people can find this information easily. **
>  
> 
> ⚠️ **CONFIDENTIALITY NOTICE:** This repository contains study protocols, Standard Operating Procedures (SOPs), and pipeline code. **No Protected Health Information (PHI) or participant identifiable data is stored here.**

---

## 🧭 Overview
For an overview of the processes that lead up to participants in our study undergoing imaging, please see ***Chad's flowchart, linke to be added** 

[This messy figure](OrderOfEvents.pptx) describes the general overview of the order of events in this project.


To suggest changes to this document, please email Kristina Visscher (or do a pull request). 
Contact information for the people described here are listed in this password protected [document](https://uab.app.box.com/file/2495951435335). 

<hr style="height: 4px; background: #0969da; border: none; margin: 48px 0 32px 0; border-radius: 2px;" />

<h2 style="background-color: #f0f4f9; border-left: 6px solid #0969da; padding: 12px 16px; border-radius: 0 6px 6px 0; margin-bottom: 20px;">📋 1. Before the Visit (Recruitment & Intake)</h2>

Participant identification, registry screening, consenting procedures, and MRI/PET visit scheduling.

| Protocol | Which Study | Format | Link |
| :--- | :--- | :--- | :--- |
| **Informed Consent Forms** | All Participants | pdfs | [View Folder](01-before-the-scan/ADRC_imaging_protocol_and_medication_guide) |

### Scheduling
* Schedules for the PET MRI are in a password protected calendar on uabmc outlook.  The name of the calendar is "WTI PET Research."  You need permissions to view it, which you can get from Lucas Riley.
* Scheduling for the PET MRI depends on time slots available, along with tracer production.  Details about the current weekly template (as of November 2026) are [here](01-before-the-scan/SchedulingTemplate.xlsx)


<hr style="height: 4px; background: #0969da; border: none; margin: 48px 0 32px 0; border-radius: 2px;" />

<h2 style="background-color: #f0f4f9; border-left: 6px solid #0969da; padding: 12px 16px; border-radius: 0 6px 6px 0; margin-bottom: 20px;">⏱️ 2. During the Visit (Acquisition Protocols)</h2>

Imaging Data are collected on "Amyloid Day" and "Tau Day".
### Tau Day: 
* Possible PET tracers include: AV1451
* [Manual of Procedures](02-during-the-scan/tau-MOP.pdf) are detailed explanations of the set of procedures, including radiotracer administration timelines 
* [Participant Information Sheets](02-during-the-scan/tau-PI.pdf) are forms that include checklists for during-scan acquisition and places for notes during the scan.
* [Tau Scan Protocol](02-during-the-scan/tau-protocol.pdf) is a GE formatted description of the tau scan. 

### Amyloid Day: 
* Possible PET tracers include: PIB, Amyvid
* [Manual of Procedures](02-during-the-scan/amy-MOP.pdf) are detailed explanations of the set of procedures, including radiotracer administration timelines (to be added)
* [Participant Information Sheets](02-during-the-scan/amy-PI.pdf) are forms that include checklists for during-scan acquisition and places for notes during the scan. (to be added)
* [Amyloid Scan Protocol](02-during-the-scan/amy-protocol.pdf) is a GE formatted description of the amyloid scan. (To be added)

### Data Uploads:
* [Protocol for uploading imaging data](02-during-the-scan/UploadImagingData.md)
* [Protocol for uploading behavioral data associated with imaging](02-during-the-scan/UploadOtherDataFromImagingDay.md)


### Contacts:
* For questions about scan acquisition, contact: Dean Fang for science-based PET questions, Kristina Visscher for science-based MRI questions, Denise Jeffers for questions about tracer production, Tyler Stamps for participant wrangling.

<hr style="height: 4px; background: #0969da; border: none; margin: 48px 0 32px 0; border-radius: 2px;" />

<h2 style="background-color: #f0f4f9; border-left: 6px solid #0969da; padding: 12px 16px; border-radius: 0 6px 6px 0; margin-bottom: 20px;">🔄 3. After the Visit (Preprocessing & Data Storage)</h2>

Initial image quality checks, standardized preprocessing for open data sharing, and long-term repository uploads.

### A. Pre-Processing for Data Sharing

Before further processing, a first pass analysis of the dataset must be gone through, described in [this document](https://uab.app.box.com/file/2293900374288) Most steps from that document are performed by Mohammad Nadian.
The PET and MRI files are read by radiologists Deepak Kalbi (PET) and Veeranjaneyulu Prattipati (MRI).


| Pipeline Step | Focus Area | Link |
| :--- | :--- | :--- |
| **SUIT Cerebellar Processing** | Cerebellar isolation & PET reference region normalization | [View Guide](03-after-the-scan/preprocessing-for-sharing/suit-cerebellar-processing-reference-regions.md) |
| **Blazer Workflow** | Automated processing and quality control pipeline | [View Guide](03-after-the-scan/BLAzER.md) |
| **MR-Guided PET Reconstruction** | Anatomically constrained PET reconstruction | [View Guide](03-after-the-scan/preprocessing-for-sharing/mr-guided-pet-reconstruction.md) |


### B. Data Storage & Repository Management

| Resource | Target System | Link |
| :--- | :--- | :--- |
| **PET and MRI QC and Data Logging** | Box| [View QC Tracker](https://uab.box.com/s/me20aqo9i3ew9qgzqwpi1e1263eoh216) |
| **Supplemental Tau Day QC and Data Logging** | Box| [View QC Tracker](https://uab.box.com/s/rnfefg6srvu36gbl8r7tdug159utbjzm) |
| **Summary of Storage Contents** | Local / Cloud Tiers | **to be added** [View Storage Manifest](03-after-the-scan/data-storage/storage-summary-manifest.md) |
| **SCAN / DVCID & LONI Archiving** | LONI / External Repositories | [View Archiving SOP](03-after-the-scan/data-storage/scan-dvcid-and-loni-archiving.md) |

<hr style="height: 4px; background: #0969da; border: none; margin: 48px 0 32px 0; border-radius: 2px;" />

<h2 style="background-color: #f0f4f9; border-left: 6px solid #0969da; padding: 12px 16px; border-radius: 0 6px 6px 0; margin-bottom: 20px;">📊 4. Dataset Processing & Analytics</h2>

Secondary pipelines, biomarker quantification, and downstream structural analyses.

| Processing Stream | Description | Link |
| :--- | :--- | :--- |
| **White Matter Hyperintensity (WMH)** | Lesion segmentation, volumetric extraction, and scripts | [View Pipeline & Code](04-dataset-processing/whitematter-hyperintensity-pipeline.md) |


<!-- Commenting this out
<hr style="height: 4px; background: #0969da; border: none; margin: 48px 0 32px 0; border-radius: 2px;" />

<h2 style="background-color: #f0f4f9; border-left: 6px solid #0969da; padding: 12px 16px; border-radius: 0 6px 6px 0; margin-bottom: 20px;">🩺 5. Clinical Safety & Monitoring</h2>

Clinical oversight and management protocols for scan-related incidental findings.

| Clinical SOP | Indication | Format | Link |
| :--- | :--- | :--- | :--- |
| **Standard of Care for ARIA** | ARIA-E / ARIA-H Monitoring & Escalation | 📄 Word Doc | [View Protocol](05-clinical/aria-standard-of-care.docx) |

<hr style="height: 4px; background: #0969da; border: none; margin: 48px 0 32px 0; border-radius: 2px;" />

<h2 style="background-color: #f6f8fa; border-left: 6px solid #57606a; padding: 12px 16px; border-radius: 0 6px 6px 0; margin-bottom: 20px;">ℹ️ Archiving & Citation</h2>
--->

To cite these study workflows in publications or progress reports:
```bibtex
@misc{study_protocols_2026,
  title  = {UAB ADRC Multimodal Imaging Protocols and Processing Pipelines},
  author = {[UAB ADRC Staff]},
  year   = {2026},
  doi    = {10.5281/zenodo.24097477}
}```
