# Independent CMS Provider-Data Observatory

![CMS Data](https://img.shields.io/badge/CMS-July_2026_Spec-blue)
<!--  ![Covers](https://img.shields.io/badge/Hospitals-5%2C419_Records-green)
![Jurisdictions](https://img.shields.io/badge/Covers-50_States_%2B_DC_%2B_Territories-orange)
![License](https://img.shields.io/badge/Data_License-Public_Domain_(U.S._Gov)-lightgrey) -->

### Being a student of Epidemiology and Public Health, I have made a lightweight web interface that transforms hospital datasets into an interactive dashboard. It tracks few Medicare-certified hospitals across all 50 U.S. states, Washington D.C., and U.S. territories.


<div>
<p align="center">
  <a href="https://hamdan-deb.github.io/Hospital-quality-atlas/" target="_blank">
    <img src="https://img.shields.io/badge/%F0%9F%9A%80%20Visit%20Live%20Website-%F0%9F%91%89%20Click%20Here-blueviolet?style=for-the-badge&logo=github" alt="Visit Live Website">
  </a>
</p>
</div>


---

## What Is This Project About?

The federal government publishes vast amounts of hospital performance data on `data.cms.gov`. However, this data is buried in massive spreadsheets with thousands of rows that are difficult for everyday users to interpret.

This web acts as an interactive dashboard that automatically reads the federal hospital registry and presents:

* An interactive 51-jurisdiction tile map showing hospital counts and star ratings per state.
* The 5 official CMS performance domains: Mortality, Safety, Readmissions, Patient Experience, and Timely Care.
* Critical community badges: 24/7 Emergency Readiness and Birthing-Friendly designations.
* Instant facility lookup with direct links to official Medicare profiles, turn-by-turn driving directions, and one-tap calling.

---

## Why Is This Hospital Data Important?

The dataset behind this project is CMS Dataset `xubh-q36u` (`Hospital_General_Information.csv`), published by the Centers for Medicare & Medicaid Services under the Department of Health and Human Services (HHS).

Every hospital in the United States that accepts Medicare or Medicaid must report standardized quality measures to the federal government. CMS aggregates these measures to assign hospitals an **Overall Hospital Quality Star Rating** from 1 to 5 stars.

---

## Who Can Use This and Why?

### 1. Patients and Families
* **Find top-rated care**: Locate 4-star and 5-star facilities nearby.
* **Emergency readiness**: Filter for facilities that provide 24/7 emergency services.
* **Maternal care**: Filter for hospitals certified as Birthing-Friendly under federal maternal health standards.

### 2. Healthcare Researchers and Epidemiologists
* **Track regional disparities**: Compare state-level averages to national benchmarks using the equal-area cartogram.
* **Analyze quality outcomes**: Contrast mortality and readmission performance across non-profit, state, and proprietary hospital systems.

### 3. Clinicians and Hospital Administrators
* **Benchmark against peers**: Evaluate where a specific facility stands relative to state and national averages.
* **Regulatory review**: Verify facility records against the official CMS July 2026 Data Dictionary specifications.

### 4. Health Journalists and Policy Makers
* **Identify healthcare deserts**: Detect states and territories with low overall star ratings or limited emergency facilities.
* **Public transparency**: Access public domain healthcare metrics without commercial paywalls or software installations.

---

## How Care Atlas Stands Out from the Crowd

| Standard Government Portals | Care Atlas |
| :--- | :--- |
| Huge multi-megabyte CSV files that freeze Excel | Opens and parses 5,419 facilities in ~80 milliseconds |
| Complex codes and acronyms (`PSI-90`, `EDAC`, `CCN`) | Visual star ratings, status chips, and clear domain breakdowns |
| Generic file downloads with no navigation | Built-in Google Maps navigation, phone links, and official Medicare pages |
| Static list views | Interactive state cartogram, live filtering, and instant search |
| Requires server backends and complex databases | 100% client-side: runs anywhere from a single static file |

---

## Integrated Companion Datasets

Beyond the general directory, the observatory links to official companion datasets and their dedicated federal methodology manuals:

| Measure Domain | CMS Dataset ID | Official Dataset Link | Methodology & Manual Link |
| :--- | :--- | :--- | :--- |
| **Hospital General Directory** | `xubh-q36u` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/xubh-q36u) | [CMS Star Rating Methodology](https://qualitynet.cms.gov/inpatient/public-reporting/overall-ratings) |
| **Complications & Deaths** | `ynj2-r877` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/ynj2-r877) | [AHRQ PSI-90 Measures Manual](https://qualitynet.cms.gov/inpatient/measures/complication) |
| **H Acquired Infections (HAI)** | `77hc-ibv8` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/77hc-ibv8) | [CDC NHSN Surveillance Protocols](https://www.cdc.gov/nhsn/psc/index.html) |
| **Patient Surveys (HCAHPS)** | `dgck-syfz` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/dgck-syfz) | [HCAHPS Survey Protocol](https://www.hcahpsonline.org/en/survey-instruments/) |
| **Unplanned Visits / Readmissions**| `632h-zaca` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/632h-zaca) | [Readmissions & EDAC Methodology](https://qualitynet.cms.gov/inpatient/measures/readmission) |
| **Timely & Effective Care** | `yv7e-xc69` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/yv7e-xc69) | [Inpatient Quality Measures Manual](https://qualitynet.cms.gov/inpatient/specifications-manuals) |
| **Maternal Health Measures** | `nrdb-3fcy` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/nrdb-3fcy) | [Maternal Health Specifications](https://qualitynet.cms.gov/inpatient/iqr/measures) |
| **Medicare Spending (MSPB)** | `rrqw-56er` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/rrqw-56er) | [Hospital Quality Initiative Guide](https://www.cms.gov/medicare/quality/initiatives/hospital-quality-initiative) |
| **Readmission Penalties (HRRP)** | `9n3s-kdb3` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/9n3s-kdb3) | [HRRP Statutory Rules](https://www.cms.gov/medicare/payment/prospective-payment-systems/acute-inpatient-pps/hospital-readmissions-reduction-program-hrrp) |
| **HAC Penalties (HACRP)** | `yq43-i98g` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/yq43-i98g) | [HACRP Scoring Regulations](https://www.cms.gov/medicare/payment/prospective-payment-systems/acute-inpatient-pps/hospital-acquired-condition-reduction-program-hacrp) |
| **Outpatient Imaging Efficiency** | `wkfw-kthe` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/wkfw-kthe) | [Outpatient Quality Reporting Manual](https://qualitynet.cms.gov/outpatient/oqr) |
| **Promoting Interoperability** | `ujcx-uaut` | [Dataset on data.cms.gov](https://data.cms.gov/provider-data/dataset/ujcx-uaut) | [CMS Interoperability Rules](https://www.cms.gov/medicare/regulations-guidance/promoting-interoperability-programs) |

---

## Live Federal Side Channels

The dashboard also pulls live public health surveillance counters from two independent federal endpoints:
1. **ClinicalTrials.gov API**: Live count of clinical trials actively recruiting patients.
2. **OpenFDA FAERS API**: Live count of adverse event reports logged in the FDA surveillance database.

---

## Quick Start & Deployment

### Deployment to a Web Server (Recommended)
1. Download `Hospital_General_Information.csv` from [data.cms.gov/provider-data/dataset/xubh-q36u](https://data.cms.gov/provider-data/dataset/xubh-q36u).
2. Place both `index.html` and `Hospital_General_Information.csv` in the same directory on your web server.
3. Open your website. The observatory will automatically detect the CSV, load all 5,419 hospitals, and cache them locally in the browser.

### Local Offline Usage
If running locally from your computer, download `index.html` and `Hospital_General_Information.csv` into the same folder. Then run the html file. The data will permanently store in your browser IndexedDB storage for future visits.

---

## Technology Stack

* **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES2022).
* **Storage**: Browser IndexedDB for zero-latency offline persistence.
* **Typography**: Space Grotesk and IBM Plex Mono.
* **Dependencies**: None (Zero build steps, zero npm packages).
* **Compliance**: Conforms to the Public CMS Hospital Downloadable Database Data Dictionary (July 2026 Release).


### Disclaimer

> ⚠️ **Important:** Please read our [Project Disclaimer](DISCLAIMER.md) before using this dashboard.

