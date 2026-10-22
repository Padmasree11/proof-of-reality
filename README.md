
# PROOF OF REALITY
### AI That Detects When Digital Evidence Is Missing Context

*Investigate the context. Understand the evidence. Recognize the uncertainty.*

Proof of Reality is an AI-assisted web application that investigates the context of digital images by examining available metadata, analyzing visible content, and searching for supporting sources.

The platform generates a **Context Gap Report** that explains what is known, what cannot be established, and what additional evidence is needed.

**Project:** DEXATHON 2026  
**Mission Track:** 04 — Intelligent Systems & GenAI  
**Status:** Under Development  
**Category:** AI · Computer Vision · Digital Evidence Investigation

---

## 1. Problem Statement

A photograph can be genuine but misleading when shared with an incorrect date, location, or explanation.

For example:

**Claim:** "This photograph shows flooding in Chennai today."

The image may show flooding, but its actual location and date may remain unverified.

Proof of Reality helps users investigate whether the available evidence supports the claim without automatically labelling the image as real or fake.

## 2. Our Solution

Users upload an image and enter an associated claim. The application examines available information and generates a structured Context Gap Report.

The platform is designed to:

- Inspect image metadata, including timestamps, camera information, and GPS coordinates.
- Analyze visible image content using AI-assisted techniques.
- Investigate potential original sources and previously published images.
- Identify missing information and conflicting evidence.
- Suggest additional evidence needed to verify the claim.

## 3. Key Features

**Image Upload and Preview**  
Upload JPG, JPEG, PNG, or WEBP images, preview the selected image, and enter a claim for investigation.

**Metadata Inspection**  
Extract available EXIF information and identify missing timestamps, camera details, or GPS coordinates.

**AI-Assisted Visual Analysis**  
Use image-captioning and computer-vision techniques to describe visible content and compare observations with the submitted claim.

**Source Investigation**  
Search for potentially relevant publications and image sources to investigate the claimed context.

**Context Gap Report**  
Present findings, uncertainties, evidence sources, and recommended next steps in a structured report.

## 4. System Architecture

```text
             PROOF OF REALITY
                    |
          +---------+---------+
          |                   |
     Frontend UI          Flask Backend
          |                   |
     HTML / CSS           Image Upload
      JavaScript          Claim Handling
          |                   |
          +---------+---------+
                    |
           Investigation Modules
                    |
       +------------+------------+
       |            |            |
    Metadata      AI Visual    Source
    Inspection    Analysis   Investigation
       |            |            |
       +------------+------------+
                    |
             Report Generator
                    |
             Context Gap Report
```

## 5. Technology Stack

| Component | Technology |
|---|---|
| Frontend | HTML5, CSS3, JavaScript |
| Backend | Python, Flask |
| Templates | Jinja2 |
| Metadata inspection | Pillow, ExifRead |
| Image processing | OpenCV, Pillow, NumPy |
| AI image analysis | PyTorch, Hugging Face Transformers, BLIP |
| Source investigation | Web search and suitable image-matching services |
| Data exchange | Python functions, JSON |
| Development | Visual Studio Code |
| Version control | Git and GitHub |

## 6. Context Gap Report

The report organizes investigation results into five sections.

| Section | Purpose |
|---|---|
| What We Know | Information supported by available evidence |
| What We Cannot Establish | Missing or unverified details |
| Evidence Found | Relevant metadata, observations, and source references |
| Evidence Needed | Additional proof required for verification |
| Overall Assessment | Preliminary assessment of the available evidence |

**Core principle:** Missing metadata or an unsuccessful source search does not prove that an image is fake. AI observations must not be treated as independent proof of a claim.

## 7. Development Roadmap

- [x] Design the image-upload interface.
- [x] Implement image preview and basic client-side validation.
- [x] Design the Context Gap Report template.
- [ ] Develop the Flask backend and upload handling.
- [ ] Implement metadata inspection.
- [ ] Integrate AI-assisted visual analysis.
- [ ] Implement source investigation.
- [ ] Integrate the modules and generate reports.
- [ ] Test the complete investigation workflow.

*Features will be marked as completed as implementation and testing progress.*

## 8. Repository Structure

```text
proof-of-reality/
├── app.py
├── README.md
├── requirements.txt
├── .gitignore
├── modules/
│   ├── metadata_inspection.py
│   ├── visual_analysis.py
│   ├── source_investigation.py
│   └── report_generator.py
├── templates/
│   ├── index.html
│   └── report.html
├── static/
│   ├── style.css
│   └── script.js
└── tests/
```

*Planned structure; files will be added as development progresses.*

## 9. Team Collaboration

| Member | Responsibility |
|---|---|
| Member 1 | Flask backend and module integration |
| Member 2 | Frontend and report interface |
| Member 3 | Metadata inspection |
| Member 4 | AI-assisted visual analysis |
| Member 5 | Source investigation and Context Gap Report |

The team uses Git and GitHub to manage code, maintain feature branches, coordinate module interfaces, and integrate tested changes into the main branch.

## 10. Expected Impact

Proof of Reality aims to make digital-image investigation more accessible by helping users understand the difference between visible content and verified context.

The project focuses on transparent evidence, traceable sources, clear uncertainties, and responsible AI-assisted analysis.

---

