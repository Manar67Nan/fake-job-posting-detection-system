# Fake Job Posting Detection System (FJPD)

**A Machine Learning-Powered Web Application for Detecting Fraudulent Job Postings**

FJPD is a web application that analyzes job advertisements and classifies them as potentially real or fake using Natural Language Processing (NLP) and machine learning techniques.

**Live Demo:** [https://fakejobpostingdetector.com/](https://fakejobpostingdetector.com/)

---

## Project Preview

![FJPD Homepage](homepage.png)

The homepage introduces the system and provides access to job posting analysis, project information, and user feedback.

## Job Analysis Interface

Users can paste a job advertisement or upload a `.txt` file for analysis.

![Job Analysis Interface](Job%20Analysis%20Interface.png)

## Job Advertisement Input

The following example demonstrates a suspicious job advertisement submitted to the system for testing.

![Job Advertisement Input](job-analysis-input.png)

## Fake Job Detection Result

After analyzing the advertisement, the system displays its prediction, confidence score, and suspicious indicators identified during the analysis.

![Fake Job Detection Result](fake-job-detection-result.png)

The displayed result demonstrates how the application presents potential warning signs to help users evaluate suspicious job postings.

---

## Admin Dashboard

FJPD also includes an administrative interface for reviewing stored analyses and monitoring detection statistics.

### 1. Overview Dashboard

Displays analysis totals, real and fake classifications, and a summary of stored records.

![Admin Overview Dashboard](admin-overview-dashboard.png)

### 2. Records Management

Provides an interface for viewing stored job analysis records, searching and filtering results, sorting records, and managing stored entries.

![Admin Records Management](admin-records-management.png)

### 3. Statistics Dashboard

Presents a summary of detection results, classification counts, and system status.

![Admin Statistics Dashboard](admin-statistics-dashboard.png)

---

## Key Features

- Machine learning-based job posting classification.
- Natural Language Processing (NLP) for text analysis.
- Job advertisement text input and `.txt` file upload.
- Prediction results with confidence scores.
- Suspicious indicator reporting.
- Administrative dashboard for reviewing stored records.
- Search, filtering, sorting, and pagination for records.
- Detection statistics and summary reports.
- User feedback functionality.
- Web-based interface with dark and light modes.

## Technologies Used

- **Python** — Backend development and machine learning integration.
- **FastAPI** — Backend API development.
- **Scikit-learn** — Machine learning and text classification.
- **TF-IDF** — Text feature extraction.
- **HTML, CSS, and JavaScript** — Frontend development.
- **SQLite** — Database storage.
- **NumPy and SciPy** — Numerical operations and sparse feature processing.
- **Joblib** — Loading trained machine learning models.

## Project Structure

```text
fake-job-posting-detection-system/
├── DOCUMENTS/
├── PREREQUISITES/
├── SETUP/
├── SOURCE/
│   ├── backend/
│   │   ├── model/
│   │   │   ├── best_model.pkl
│   │   │   └── tfidf_vectorizer.pkl
│   │   ├── routes/
│   │   ├── __init__.py
│   │   ├── database_manager.py
│   │   ├── main.py
│   │   ├── schemas.py
│   │   └── utils.py
│   └── frontend/
│       └── frontend.html
├── .gitignore
└── README.md
```

## Running Locally

### Prerequisites

- Python 3.11
- Git

### Installation

1. Clone the repository:

   ```bash
   git clone YOUR_GITHUB_REPOSITORY_URL
   ```

2. Navigate to the project directory:

   ```bash
   cd fake-job-posting-detection-system
   ```

3. Install the required dependencies using the location of `requirements.txt` in the repository:

   ```bash
   pip install -r SETUP/requirements.txt
   ```

4. Navigate to the source directory:

   ```bash
   cd SOURCE
   ```

5. Start the FastAPI application:

   ```bash
   uvicorn backend.main:app --reload
   ```

6. Open the application in your browser:

   [http://127.0.0.1:8000](http://127.0.0.1:8000)

**Note:** The trained model files must be available in `SOURCE/backend/model/`. The database is initialized by the backend application.

## Project Purpose

The goal of this project is to explore how machine learning and Natural Language Processing can help identify suspicious job advertisements and support safer online job searching.

## Academic Project

Developed as a senior project to demonstrate practical skills in machine learning, text processing, backend development, database management, and web application design.

## Disclaimer

FJPD provides machine learning-based predictions to help identify potentially fraudulent job postings. Predictions and confidence scores are not guarantees of authenticity. Users should verify job offers through official company websites and trusted recruitment channels before sharing personal information or making payments.
