# AI-Based Security Policy Compliance Verification in SPL

A machine learning approach to automate security policy compliance 
verification in Software Product Lines (SPLs), using Android 
application configurations as a case study.

Built with: Python • Scikit-learn • Pandas • Matplotlib • Google Colab

---

## Problem

In Software Product Lines, hundreds of configurations must be 
verified against security policies — manual verification is 
impractical and error-prone.

---

##  Solution

An improved Random Forest classifier trained on real Android 
behavioral data to automatically classify configurations as 
**Compliant** or **Non-Compliant**.

---

## Dataset

- **CIC-MalDroid 2020** — Canadian Institute for Cybersecurity
- 9,991 Android application instances
- 140 features (Linux system call activities)
- 3 security-relevant features selected: `socket`, `connect`, `open`

---

##  Methodology

| Stage | Description |
|-------|-------------|
| 1 | Case Study Selection (Android Configurations) |
| 2 | Dataset Identification (CIC-MalDroid 2020) |
| 3 | Feature Modeling & Policy Definition |
| 4 | Data Preprocessing |
| 5 | Random Forest Model Building |
| 6 | Model Training & Testing |
| 7 | Result Interpretation |

**Security Policy Thresholds:**
- `socket` ≤ 13
- `connect` ≤ 10
- `open` ≤ 50

---

## Results

| Metric | Value |
|--------|-------|
| Test Accuracy | **100%** |
| Precision | 1.00 |
| Recall | 1.00 |
| F1-Score | 1.00 |

> Model maintained perfect accuracy even after injecting 30% noise 
> into training data.

---

## System Architecture

![System Architecture](system_architecture.png)

---

## How to Run

1. Open the notebook in Google Colab
2. Upload the CIC-MalDroid 2020 dataset to your Google Drive
3. Run all cells in order

---

##  Author

Sharifa Alzubadi 
