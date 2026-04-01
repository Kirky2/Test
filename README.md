# Resume Optimization Test Suite

## Overview

This repository contains a comprehensive test suite for the **Resume Optimization** feature of CV-AI. The feature allows users to:

1. Upload a resume (PDF or DOCX).
2. Input or import a job description (manual or URL).
3. Generate an AI-tailored resume optimized for Applicant Tracking Systems (ATS).
4. Review ATS scores and receive actionable recommendations.

This repository is intended for GitHub submission and demonstrates automated and manual test coverage.

---

## Repository Structure

```
resume-optimization-test/
├── README.md                  # This file
├── tests/                     # Playwright automated test scripts
│   └── resumeOptimization.spec.ts
├── test-data/                 # Sample resumes and job description files
│   ├── sample_resume.pdf
│   ├── sample_resume.docx
│   └── sample_image.png
├── package.json               # Project dependencies
├── playwright.config.ts       # Playwright configuration
└── .gitignore
```

---

## Requirements

* Node.js v18+
* npm or yarn
* Playwright v1.40+

---

## Setup Instructions

1. Clone the repository:

```bash
git clone https://github.com/yourusername/resume-optimization-test.git
cd resume-optimization-test
```

2. Install dependencies:

```bash
npm install
# or
yarn install
```

3. Install Playwright browsers:

```bash
npx playwright install
```

---

## Running the Tests

### Run all tests:

```bash
npx playwright test
```

### Run tests in headed mode (visual verification):

```bash
npx playwright test --headed
```

### Run a single test file:

```bash
npx playwright test tests/resumeOptimization.spec.ts
```

### Generate HTML Test Report:

```bash
npx playwright show-report
```

---

## Test Coverage

The test suite covers:

* **OPT-001:** Resume Input Handling
* **OPT-002:** Job Description Parsing
* **OPT-003:** AI Processing & Output
* **OPT-004:** ATS Scoring
* **OPT-005:** Recommendations Panel
* **OPT-006:** UI/UX Interaction
* **OPT-007:** Export Functionality
* **OPT-008:** Error Handling
* **OPT-009:** Performance & Load
* **OPT-010:** Security/Permissions

---

## Test Data

Sample data is provided in `test-data/`:

* `sample_resume.pdf` – valid PDF resume
* `sample_resume.docx` – valid DOCX resume
* `sample_image.png` – unsupported format
* Job descriptions – included in test scripts; external URLs can also be used.

---

## Notes

* Tests are written using **Playwright** and assume a functional CV-AI environment at `https://cv-ai.work`.
* Valid login credentials are required or can be mocked for local execution.
* AI-generated results may vary; tests focus on **workflow and UI correctness**.

---

## Submission Instructions

Include this repository URL, your cover letter, and résumé in your submission email:

```
To: mark@theblokc.com
Subject: Tester Intern: Software Tester Intern Applicant – [Your Full Name]
```
