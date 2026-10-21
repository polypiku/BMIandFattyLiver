# BMI & Fatty Liver Risk Assessment

A web app that estimates a person's risk of non-alcoholic fatty liver disease (NAFLD) from their BMI, basic health factors and blood test results, using a Random Forest model that runs fully in the browser.

เว็บแอปประเมิน BMI และความเสี่ยงไขมันพอกตับ จากข้อมูลสุขภาพและผลตรวจเลือด

**Live demo:** https://polypiku09-crypto.github.io/BMIandFattyLiver/

![BMI & Fatty Liver](screenshots/result.png)

## Features
- Sign up and log in, with a consent step before collecting health data
- BMI calculation and classification from height and weight
- Fatty liver risk prediction across 4 risk levels, with class probabilities shown as a chart
- Optional blood test inputs: FBS, triglycerides, HDL, LDL, ALT, AST, GGT, platelets, bilirubin, TSH
- Risk factors: diabetes, hypertension, alcohol, smoking, PCOS
- Saved assessment history per user, with the option to delete entries
- In-app user guide

## Model
- **Algorithm:** Random Forest classifier (25 trees, max depth 5), exported to JSON and evaluated in JavaScript
- **Features:** 18 inputs; the most important are BMI (47%), triglycerides (12%), ALT (10%) and GGT (8%)
- **Data:** trained on a NAFLD dataset of 10,000 records
- **Accuracy:** 65% on a holdout set

> For education only. This is not a medical diagnosis.

## Tech Stack

| Part | Technology |
|------|------------|
| Frontend | HTML, CSS, JavaScript |
| Charts | Chart.js |
| Model | Random Forest, trained offline and embedded as JSON |
| Storage | Browser localStorage |
| Hosting | GitHub Pages |

## Run Locally

Open `index.html` in a browser. No build step is needed.

## My Role

<!-- Write 2–3 lines in your own words: e.g. data preparation, training the model, building the web app. -->

---
Built as a university data analytics mini project.
