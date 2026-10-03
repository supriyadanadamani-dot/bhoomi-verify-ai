# BhoomiVerify AI

## Intelligent Land Records Digitization & Validation System

**BhoomiVerify AI** is a college project that uses **OCR and AI-assisted information extraction** to convert land-record documents into structured digital records.

The system allows an authorized user to upload a land document, extract its information automatically, review and correct the extracted data, verify the record, store it securely, search records, and view an approximate location on a map.

> **Important:** AI assists the user. Final verification is performed by a human user.

---

# 1. Project Information

| Item                 | Details                                                   |
| -------------------- | --------------------------------------------------------- |
| Project Name         | BhoomiVerify AI                                           |
| Project Title        | Intelligent Land Records Digitization & Validation System |
| Project Type         | College Project                                           |
| Team Size            | 2 Members                                                 |
| Development Duration | 30 Days                                                   |
| Project Domain       | AI + Web Application                                      |
| Main Users           | Land-record staff/officers                                |
| Primary Language     | Python                                                    |
| Frontend             | React                                                     |
| Backend              | FastAPI                                                   |
| Database             | PostgreSQL                                                |
| OCR                  | PaddleOCR                                                 |
| Maps                 | Leaflet + OpenStreetMap                                   |

---

# 2. Problem Statement

Land records may exist as paper documents or scanned files. Entering information from these documents manually is time-consuming and can lead to errors.

There is a need for a system that can automatically read documents, extract important information, identify possible issues, and allow a human user to verify and correct the information.

---

# 3. Proposed Solution

BhoomiVerify AI provides a digital workflow:

```text
Land Document
      ↓
OCR
      ↓
Text Extraction
      ↓
AI-Assisted Field Extraction
      ↓
Possible Issue Detection
      ↓
Human Review & Correction
      ↓
Verification
      ↓
Database Storage
      ↓
Search / View
      ↓
Map Location
```

---

# 4. Main Objectives

* Digitize land-record documents.
* Extract text automatically using OCR.
* Identify important land-record fields.
* Provide AI-assisted information extraction.
* Show extraction confidence.
* Identify possible data issues.
* Allow human correction.
* Allow authorized users to verify records.
* Store verified records in a database.
* Search and view land records.
* Provide basic language/translation support.
* Display approximate location on a map.
* Maintain verification history.

---

# 5. Main Features

### Authentication

* User login
* Logout
* Role-based access
* Admin/user management

### Document Management

* Upload PDF/image documents
* File validation
* Document preview
* Document storage
* Processing status

### OCR

* Extract text from scanned documents
* Display extracted text
* Store OCR results

### AI-Assisted Extraction

Extract important fields such as:

* Owner name
* Survey number
* Village
* Taluk
* District
* State
* Land area
* Land type
* Document/reference number
* Date

### Validation & Verification

* Confidence score
* Possible issue detection
* Human review
* Edit extracted information
* Verification status
* Verification remarks
* Verification history

### Search & Records

* Search by owner
* Search by survey number
* Search by village
* Search by district
* Filter by verification status
* View complete record

### Language Support

* Display original text
* Basic translation support
* Regional-language viewing

### Map

* Display approximate location
* Latitude/longitude
* Interactive map
* OpenStreetMap-based map

### Dashboard

* Total records
* Pending records
* Verified records
* Records needing correction
* Recent uploads

---

# 6. Complete System Workflow

```text
Login
  ↓
Dashboard
  ↓
Upload Land Document
  ↓
File Validation
  ↓
Document Storage
  ↓
OCR Processing
  ↓
Extract Raw Text
  ↓
AI-Assisted Field Extraction
  ↓
Confidence & Issue Detection
  ↓
Display Extracted Information
  ↓
Human Review
  ↓
Edit / Correct Information
  ↓
Verify Record
  ↓
Save Record
  ↓
Search / View Record
  ↓
Map / Location
```

---

# 7. Technology Stack

| Component         | Technology    | Purpose                        |
| ----------------- | ------------- | ------------------------------ |
| Code Editor       | VS Code       | Development                    |
| Version Control   | Git           | Source-code management         |
| Repository        | GitHub        | Team collaboration             |
| Frontend          | React         | User interface                 |
| Build Tool        | Vite          | React development              |
| Backend           | FastAPI       | REST APIs                      |
| Programming       | Python        | Backend and AI processing      |
| Database          | PostgreSQL    | Store application data         |
| ORM               | SQLAlchemy    | Database communication         |
| OCR               | PaddleOCR     | Extract text from documents    |
| PDF Processing    | PyMuPDF       | Process PDF documents          |
| API Communication | Axios         | Frontend-backend communication |
| Authentication    | JWT           | User authentication            |
| Maps              | Leaflet       | Interactive map                |
| Map Data          | OpenStreetMap | Map display                    |

---

# 8. Software & Installation Plan

Software will **not** be installed all at once.

Each technology will be installed when its development stage starts.

## Stage 1 — Project Setup

### Required

* VS Code
* Git
* Node.js 22 LTS
* Python 3.11

Purpose:

```text
Git       → Version control
VS Code   → Coding
Node.js   → React development
Python    → Backend/AI development
```

---

## Stage 2 — Frontend

### Required

* React 19.x
* Vite
* Axios
* React Router

Purpose:

```text
React       → UI
Vite        → Development/build
Axios       → API communication
React Router → Page navigation
```

---

## Stage 3 — Database

### Required

* PostgreSQL 17.x

### Optional

* pgAdmin

Purpose:

```text
PostgreSQL → Store users, documents and land records
pgAdmin    → Manage database visually
```

---

## Stage 4 — Backend

### Required

* FastAPI
* Uvicorn
* SQLAlchemy
* PostgreSQL driver
* Python Multipart

Purpose:

```text
FastAPI       → Backend APIs
Uvicorn       → Run backend
SQLAlchemy    → Database operations
PostgreSQL DB → Data storage
Multipart     → File upload
```

---

## Stage 5 — OCR

### Required

* PaddleOCR
* PyMuPDF
* Required OCR dependencies

Purpose:

```text
PyMuPDF   → Process PDF files
PaddleOCR → Read text from documents
```

---

## Stage 6 — AI Extraction

### Required

* Python-based extraction logic
* Text preprocessing

### Optional

* External AI/LLM API

Purpose:

```text
OCR Text
   ↓
Text Processing
   ↓
Field Extraction
   ↓
Confidence / Issue Detection
```

The project will not depend completely on an external AI service.

---

## Stage 7 — Map

### Required

* Leaflet
* React-Leaflet

### Map Data

* OpenStreetMap

Purpose:

Display approximate land-record location.

---

# 9. Application Pages

```text
Login
  ↓
Dashboard
  ├── Upload Document
  │      ↓
  │   Processing
  │      ↓
  │   OCR Result
  │      ↓
  │   Extracted Information
  │      ↓
  │   Correction
  │      ↓
  │   Verification
  │
  ├── Search Records
  │      ↓
  │   Record Details
  │      ↓
  │   Map
  │
  └── Profile / Logout
```

### Main Pages

1. Login
2. Dashboard
3. Upload Document
4. Document Preview
5. Processing Status
6. OCR Result
7. Extracted Information
8. Correction & Verification
9. Records/Search
10. Record Details
11. Map/Location
12. Profile
13. Admin/User Management

---

# 10. Database

## Database

**PostgreSQL**

## Main Tables

### Users

```text
id
name
email
password_hash
role
created_at
```

### Documents

```text
id
uploaded_by
file_name
file_path
file_type
upload_date
processing_status
```

### Land Records

```text
id
document_id
owner_name
survey_number
village
taluk
district
state
land_area
land_type
record_date
latitude
longitude
verification_status
verified_by
verified_at
remarks
```

### OCR Results

```text
id
document_id
raw_text
language
ocr_confidence
created_at
```

### Extracted Fields

```text
id
record_id
field_name
field_value
confidence
original_value
corrected_value
```

### Verification History

```text
id
record_id
user_id
old_status
new_status
remarks
changed_at
```

---

# 11. Verification Status

The system uses three main statuses:

```text
PENDING
    ↓
NEEDS_CORRECTION
    ↓
VERIFIED
```

AI-extracted information is **not automatically considered verified**.

The human user reviews and confirms the information.

---

# 12. System Architecture

```text
                 USER
                   ↓
            React Frontend
                   ↓
             FastAPI API
             ↙    ↓     ↘
       Database   AI    Storage
          ↓       ↓
     PostgreSQL  OCR
                   ↓
            Field Extraction
                   ↓
             Human Review
                   ↓
              Verification
                   ↓
             Land Records
                   ↓
              Map / Search
```

---

# 13. Two-Person Team

## Person 1 — Frontend & Integration

Responsibilities:

* React setup
* UI design
* Login page
* Dashboard
* Upload page
* Document preview
* OCR result page
* Extraction page
* Verification UI
* Search and records
* Map UI
* API integration
* Frontend testing

---

## Person 2 — Backend, Database & AI

Responsibilities:

* FastAPI setup
* API development
* PostgreSQL
* Authentication backend
* File upload API
* Document storage
* OCR
* Text processing
* AI extraction
* Confidence calculation
* Validation
* Verification APIs
* Search APIs
* Backend testing

---

## Both Members

* Project planning
* GitHub management
* API integration
* Debugging
* Testing
* Documentation
* PPT preparation
* Final demonstration

---

# 14. GitHub Branch Strategy

```text
main
│
├── frontend-dev
│
└── backend-ai-dev
```

### Person 1

Works mainly on:

```text
frontend-dev
```

### Person 2

Works mainly on:

```text
backend-ai-dev
```

### Integration

Both branches will be integrated regularly.

Important integration points:

```text
Day 7  → Upload
Day 10 → OCR
Day 16 → Verification
Day 19 → Records
Day 22 → Map
Day 24 → Complete integration
```

---

# 15. Project Folder Structure

```text
BhoomiVerify-AI/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── app/
│   ├── uploads/
│   ├── requirements.txt
│   └── main.py
│
├── ai/
│   ├── ocr/
│   ├── extraction/
│   └── preprocessing/
│
├── database/
│   ├── schema.sql
│   └── sample_data.sql
│
├── docs/
│   ├── report/
│   ├── screenshots/
│   └── diagrams/
│
├── .gitignore
└── README.md
```

---

# 16. 30-Day Development Plan

| Day | Main Target                   | Output                            |
| --- | ----------------------------- | --------------------------------- |
| 1   | Git + development environment | Repository and environments ready |
| 2   | Frontend/backend structure    | Basic applications running        |
| 3   | Database setup                | PostgreSQL connected              |
| 4   | Database tables               | Initial schema ready              |
| 5   | Upload UI + API               | Document upload works             |
| 6   | Document storage/preview      | Uploaded document can be viewed   |
| 7   | Processing workflow           | Upload-to-processing flow         |
| 8   | OCR setup                     | OCR environment ready             |
| 9   | OCR implementation            | Text extracted                    |
| 10  | OCR database integration      | OCR text stored                   |
| 11  | Extraction design             | Field extraction structure        |
| 12  | Basic extraction              | Important fields extracted        |
| 13  | Confidence                    | Confidence displayed              |
| 14  | Issue detection               | Possible issues displayed         |
| 15  | Correction UI/API             | User can edit fields              |
| 16  | Verification                  | User can verify record            |
| 17  | Verification history          | Changes recorded                  |
| 18  | Search                        | Records searchable                |
| 19  | Record details                | Complete record view              |
| 20  | Language support              | Basic translation                 |
| 21  | Location handling             | Location information available    |
| 22  | Map                           | Location displayed                |
| 23  | Error handling                | Application more stable           |
| 24  | Full integration              | Complete workflow works           |
| 25  | Testing                       | Bugs identified                   |
| 26  | Bug fixing                    | Major bugs fixed                  |
| 27  | Document testing              | Multiple sample documents tested  |
| 28  | Final UI/security             | Demo-ready application            |
| 29  | Documentation                 | Report + PPT + screenshots        |
| 30  | Final testing                 | Complete project ready            |

---

# 17. Daily Development Rule

Each day will follow:

```text
Person 1 Task
      +
Person 2 Task
      ↓
Integration
      ↓
Testing
      ↓
Daily Output
```

Future software will only be installed when required.

---

# 18. Project Milestones

| Milestone                   |  Days | Result                   |
| --------------------------- | ----: | ------------------------ |
| M1 — Setup                  |   1–4 | Basic project + database |
| M2 — Upload                 |   5–7 | Document upload          |
| M3 — OCR                    |  8–10 | Text extraction          |
| M4 — AI Extraction          | 11–14 | Structured fields        |
| M5 — Verification           | 15–19 | Human verification       |
| M6 — Language               |    20 | Translation              |
| M7 — Map                    | 21–22 | Location display         |
| M8 — Integration            | 23–24 | Complete workflow        |
| M9 — Testing & Finalization | 25–30 | Final project            |

---

# 19. Practical Limitations

### OCR Accuracy

OCR may make mistakes with poor-quality documents.

**Solution:** Human review and correction.

### Different Document Formats

Different documents may have different layouts.

**Solution:** Demonstrate using a few supported document formats.

### AI Accuracy

AI extraction may produce incorrect information.

**Solution:** Show confidence and require human verification.

### Government Database

The project does not automatically access government land databases.

**Solution:** Use sample/demo records in PostgreSQL.

### Exact Land Boundaries

An address or village name does not provide an official survey boundary.

**Solution:** Display an approximate map marker only.

### Translation

Legal/land terminology may not translate perfectly.

**Solution:** Keep original text and translated text together.

---

# 20. Project Scope

### Included

* Web application
* Document upload
* OCR
* AI-assisted extraction
* Human correction
* Verification
* Database
* Search
* Translation
* Map
* Authentication
* Verification history

### Not Included

* Official government database integration
* Legal land ownership validation
* Official cadastral/survey boundary verification
* Government authentication systems
* Production-scale deployment

---

# 21. Expected Final Result

At the end of 30 days, BhoomiVerify AI should allow an authorized user to:

```text
Login
 ↓
Upload a land document
 ↓
View document
 ↓
Run OCR
 ↓
Extract important information
 ↓
See confidence/possible issues
 ↓
Correct information
 ↓
Verify record
 ↓
Save to database
 ↓
Search record
 ↓
View record details
 ↓
View approximate location on map
```

---

# 22. Future Scope

Possible future improvements:

* Integration with authorized government land-record APIs.
* Advanced document classification.
* Better handwriting OCR.
* More Indian-language support.
* Advanced AI-based anomaly detection.
* GIS/cadastral boundary integration.
* Digital signatures.
* Mobile application.
* Advanced audit and access control.
* Large-scale cloud deployment.

---

# 23. Team Development Rules

1. Develop the project step by step.
2. Do not write the entire project at once.
3. Install software only when required.
4. Person 1 mainly handles frontend.
5. Person 2 mainly handles backend, database, OCR and AI.
6. Both members test the integrated system regularly.
7. Use Git branches for parallel development.
8. Commit changes regularly.
9. Never upload passwords, API keys or database credentials to GitHub.
10. AI output must always be reviewable by a human.
11. Use sample/demo documents unless authorized real datasets are available.
12. Keep the project within the 30-day scope.

---

# 24. Development Approach

```text
PLAN
 ↓
SETUP
 ↓
FRONTEND + BACKEND
 ↓
DATABASE
 ↓
DOCUMENT UPLOAD
 ↓
OCR
 ↓
AI EXTRACTION
 ↓
HUMAN VERIFICATION
 ↓
LANGUAGE SUPPORT
 ↓
MAP
 ↓
INTEGRATION
 ↓
TESTING
 ↓
DOCUMENTATION
 ↓
FINAL DEMO
```

---

## Project Status

**Current Status:** Project Repository Created
**Next Step:** Development Environment Setup
**Duration:** 30 Days
**Team:** 2 Members

---

## Final Goal

> **Two people + 30 days → One complete working BhoomiVerify AI prototype**
