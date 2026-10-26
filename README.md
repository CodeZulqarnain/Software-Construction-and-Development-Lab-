<div align="center">

<!-- Animated Header Banner -->
<img src="assets/banner_animated.svg" width="100%" alt="Software Construction and Development Banner" />

<br/><br/>

<!-- Dynamic Status Badges -->
[![Course](https://img.shields.io/badge/Course-Software%20Construction%20%26%20Development%20(Lab)-0284c7?style=for-the-badge&logo=codeforces&logoColor=white)](https://github.com/)
[![University](https://img.shields.io/badge/University-UAJK%20Muzaffarabad-1e3a8a?style=for-the-badge&logo=google-classroom&logoColor=white)](https://ajku.edu.pk/)
[![Semester](https://img.shields.io/badge/Semester-Fall%202026%20(5th%20Sem)-059669?style=for-the-badge&logo=gitbook&logoColor=white)](https://github.com/)
[![Instructor](https://img.shields.io/badge/Instructor-Engr.%20Dr.%20Asma%20Javaid-7c3aed?style=for-the-badge&logo=pinboard&logoColor=white)](https://github.com/)

<br/>

[![Status](https://img.shields.io/badge/QOBE%20Status-Verified%20%26%20Ready-10b981?style=flat-square&logo=checkmarx&logoColor=white)](https://github.com/)
[![Standard](https://img.shields.io/badge/Standard-UML%202.5-38bdf8?style=flat-square&logo=uml&logoColor=white)](https://github.com/)
[![Docs](https://img.shields.io/badge/Documentation-Markdown%20%7C%20HTML%20%7C%20PDF-f59e0b?style=flat-square&logo=readthedocs&logoColor=white)](https://github.com/)
[![Python](https://img.shields.io/badge/Scripts-Python%203.11-3776ab?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![License](https://img.shields.io/badge/Academic%20License-UAJK%20DoSE-64748b?style=flat-square&logo=creative-commons&logoColor=white)](LICENSE)

<br/>

<!-- Animated Terminal Box -->
<img src="assets/typing.svg" width="100%" alt="Animated Terminal Console" />

<br/><br/>

<!-- Animated Metrics Card -->
<img src="assets/progress.svg" width="100%" alt="Lab Progress & Metrics" />

</div>

<br/>

---

## 📑 Table of Contents

- [🌟 Course Overview](#-course-overview)
- [🏛️ Academic & Instruction Details](#️-academic--instruction-details)
- [🗺️ Laboratory Roadmap](#️-laboratory-roadmap)
- [🚀 Lab 01: Use Case Modeling & Requirement Analysis](#-lab-01-use-case-modeling--requirement-analysis)
  - [Q1: Online Ticket Reservation System](#q1-online-ticket-reservation-system)
  - [Q2: Credit Card Processing System (Case Study)](#q2-credit-card-processing-system-case-study)
  - [Traceability & Relationship Highlights](#traceability--relationship-highlights)
- [📂 Repository File Architecture](#-repository-file-architecture)
- [⚙️ Setup, Execution & PDF Export](#️-setup-execution--pdf-export)
- [📋 QOBE Submission Compliance](#-qobe-submission-compliance)
- [📜 License & Academic Integrity](#-license--academic-integrity)

---

## 🌟 Course Overview

**Software Construction & Development (SC&D)** focuses on the engineering principles, architectural patterns, design formalisms, and construction practices required to transform abstract software requirements into robust, maintainable, extensible, and high-performance software systems.

### Core Pillars
1. **Architectural & Behavioral Modeling:** Detailed requirement engineering using standard UML 2.5 specifications.
2. **Design Principles & Patterns:** Application of SOLID, DRY, KISS, and Gang of Four (GoF) design patterns.
3. **Refactoring & Code Quality:** Identifying code smells, calculating software metrics, and optimizing legacy code.
4. **Verification & Automation:** Test-Driven Development (TDD), unit testing frameworks, and continuous delivery pipelines.

---

## 🏛️ Academic & Instruction Details

| Field | Detail |
| :--- | :--- |
| **Institution** | The University of Azad Jammu and Kashmir (UAJK), Muzaffarabad |
| **Department** | Department of Software Engineering (DoSE) |
| **Degree Program**| BS Software Engineering (5th Semester) |
| **Course Title** | Software Construction & Development (Lab) |
| **Instructor** | **Engr. Dr. Asma Javaid** |
| **Semester** | Fall 2026 |
| **Portal** | QOBE Assessment System |

---

## 🗺️ Laboratory Roadmap

```
Semester Lab Sequence
├── [x] Lab 01: Use Case Modeling & Requirement Engineering ─── (Completed & Verified)
├── [ ] Lab 02: Domain Modeling & Robust Class Diagrams
├── [ ] Lab 03: Dynamic Behavioral Modeling (Sequence & State Diagrams)
├── [ ] Lab 04: Object-Oriented Design Principles (SOLID, DRY, Law of Demeter)
├── [ ] Lab 05: Creational Design Patterns (Singleton, Factory, Builder)
├── [ ] Lab 06: Structural Design Patterns (Adapter, Composite, Decorator)
├── [ ] Lab 07: Behavioral Design Patterns (Observer, Strategy, State, Command)
├── [ ] Lab 08: Code Smells, Metrics & Systematic Refactoring
├── [ ] Lab 09: Automated Unit Testing & Test-Driven Development (TDD)
└── [ ] Lab 10: Build Automation, Git Workflows & CI/CD Pipelines
```

---

## 🚀 Lab 01: Use Case Modeling & Requirement Analysis

> **Status:** `COMPLETED (100%)`  
> **Documentation Files:** [`Lab_1_Solution.md`](Lab_1_Solution.md) • [`Lab_1_Solution.html`](Lab_1_Solution.html) • [`Lab 1 - Software Construction & Development.pdf`](Lab%201%20-%20Software%20Construction%20&%20Development.pdf)

### Q1: Online Ticket Reservation System
Develop an end-to-end Use Case model representing an enterprise ticket reservation system (transportation/events).

* **Primary Actors:** Customer / Passenger, System Administrator
* **Supporting Actors:** Payment Gateway, Notification Service (SMS/Email)
* **Key Use Cases:** Search Trips, Select Seat(s), Book Ticket, Make Online Payment, Apply Promo Code, View E-Ticket, Cancel Reservation, Process Refund, Manage Routes.
* **Stereotype Hierarchies:**
  * `Book / Reserve Ticket` $\xrightarrow{\ll include\gg}$ `Select Seat(s)`
  * `Book / Reserve Ticket` $\xrightarrow{\ll include\gg}$ `Make Online Payment`
  * `Make Online Payment` $\xrightarrow{\ll include\gg}$ `Send Booking Confirmation`
  * `Cancel Reservation` $\xrightarrow{\ll include\gg}$ `Process Refund Transaction`
  * `Apply Promo Code / Discount` $\xrightarrow{\ll extend\gg}$ `Make Online Payment`

<div align="center">
  <img src="q1_online_ticket_reservation_diagram.png" width="92%" alt="Q1 Use Case Diagram" />
  <p><em>Figure 1.1: UML 2.5 Standard Diagram for Online Ticket Reservation System</em></p>
</div>

---

### Q2: Credit Card Processing System (Case Study)
Case study analysis of mall POS purchases, balance limits, card swiping, and receipt generation.

* **Identified Actors:**
  * **Customer:** Browses shop items, provides credit card, verifies statement, signs and returns receipt.
  * **Vendor / Cashier:** Scans items, generates bill, swipes card, requests amount transaction, hands receipt to customer, archives signed slip.
  * **Credit Card Machine / Reader (POS Terminal):** Hardware interface that captures magnetic/EMV data, communicates transaction packets, and prints statements.
  * **Banking Network / Card Issuer Bank:** Backend system maintaining balance limits, validating limits, executing fund settlements, and updating balances.
* **Key Use Cases:**
  * `Select Item from Shop`, `Make Bill for Selected Item`, `Swipe / Insert Credit Card`, `Request Amount Transaction`
  * `Process Card Transaction` $\xrightarrow{\ll include\gg}$ `Check & Verify Credit Balance Limit`
  * `Process Card Transaction` $\xrightarrow{\ll include\gg}$ `Update Account Balance & Record Transaction`
  * `Process Card Transaction` $\xrightarrow{\ll include\gg}$ `Print Balance Statement & Receipt`
  * `Handle Declined Transaction` $\xrightarrow{\ll extend\gg}$ `Check & Verify Credit Balance Limit`
  * `Sign & Return Receipt to Vendor`

<div align="center">
  <img src="q2_credit_card_processing_diagram.png" width="92%" alt="Q2 Use Case Diagram" />
  <p><em>Figure 2.1: UML 2.5 Standard Diagram for Credit Card Processing System</em></p>
</div>

---

### Traceability & Relationship Highlights

| Case Study Requirement | Identified Actor(s) | Primary Use Case | Relationship |
| :--- | :--- | :--- | :--- |
| *Select item to be purchased from shop* | Customer | Select Item from Shop | Direct Association |
| *Vendor should give a bill for selected item* | Vendor | Make Bill for Selected Item | Direct Association |
| *Customer gives card to swap* | Customer, Vendor, Reader | Swipe / Insert Credit Card | Direct Association |
| *Request for kind of amount transaction* | Vendor, Card Reader | Request Amount Transaction | `<<include>>` to Process |
| *Required amount transaction done by reader* | Reader, Banking Network | Process Card Transaction | Core Orchestration |
| *Maintain limitation of credit card balance* | Banking Network | Check & Verify Credit Balance Limit | `<<include>>` from Process |
| *Current transaction process updated* | Banking Network | Update Account Balance | `<<include>>` from Process |
| *Machine gives balance statement or receipt* | Card Reader, Vendor | Print Balance Statement & Receipt | `<<include>>` from Process |
| *Vendor issue statement to customer* | Vendor, Customer | Print / Issue Statement | Direct Association |
| *Customer puts signature and returns* | Customer, Vendor | Sign & Return Receipt to Vendor | Direct Association |

---

## 📂 Repository File Architecture

```
e:/5th sem/SC&D/
│
├── 📂 assets/                                  # Animated SVG components for GitHub
│   ├── 🖼️ banner_animated.svg                 # Glowing header banner
│   ├── 💻 typing.svg                          # Terminal typing animation
│   └── 📊 progress.svg                        # Animated metrics & lab status card
│
├── 📄 README.md                                # Modern animated repository presentation
│
├── 📘 Lab_1_Solution.md                        # Full academic markdown report with tables & specs
├── 🌐 Lab_1_Solution.html                      # Standalone, print-ready HTML with base64 embedded diagrams
├── 📑 Lab 1 - Software Construction & Development.pdf # Exported submission PDF for QOBE portal
│
├── 🎨 q1_online_ticket_reservation_diagram.png # 300 DPI high-resolution diagram (Q1)
├── 🎨 q2_credit_card_processing_diagram.png    # 300 DPI high-resolution diagram (Q2)
│
├── 🐍 generate_diagrams.py                     # Python script to regenerate matplotlib diagrams
└── 🐍 generate_html_report.py                  # Python script to compile standalone HTML report
```

---

## ⚙️ Setup, Execution & PDF Export

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/software-construction-development.git
cd software-construction-development
```

### 2. Regenerate High-Resolution Diagrams
```bash
python generate_diagrams.py
```

### 3. Rebuild Standalone HTML Report
```bash
python generate_html_report.py
```

### 4. Export to PDF for QOBE
1. Open [`Lab_1_Solution.html`](Lab_1_Solution.html) in any modern browser (Google Chrome, Microsoft Edge, Firefox).
2. Press `Ctrl + P` (or `Cmd + P` on macOS).
3. Set **Destination** to `Save as PDF`.
4. Ensure **Background Graphics** is checked.
5. Click **Save** to generate a clean PDF identical to [`Lab 1 - Software Construction & Development.pdf`](Lab%201%20-%20Software%20Construction%20&%20Development.pdf).

---

## 📋 QOBE Submission Compliance

* [x] **Timely Submission:** Completed ahead of deadline.
* [x] **Platform Integrity:** Ready for direct upload to QOBE portal.
* [x] **Standard Notation:** Conforms to OMG UML 2.5 standards.
* [x] **Originality:** 100% verified unique work with full traceability matrix.

---

## 📜 License & Academic Integrity

This repository is maintained for academic coursework in the **Department of Software Engineering, The University of Azad Jammu and Kashmir (UAJK)**. All source models and documentation adhere to university academic standards.

<br/>

<div align="center">
  <sub>Constructed with ❤️ for <strong>Software Construction & Development (Lab)</strong> • UAJK Muzaffarabad • Fall 2026</sub>
</div>
