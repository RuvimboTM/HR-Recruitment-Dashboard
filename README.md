# HR Recruitment Dashboard (Power BI)

A Power BI dashboard that visualises recruitment data for the HR department. It is part of the **"Utilising Robotic Process Automation to Optimise the Job Recruitment Process"** project.

## Part of a larger project

- **Web portal (ASP.NET):** https://github.com/RuvimboTM/HR-Dept-Portal
- **UiPath automation:** https://github.com/RuvimboTM/HR-Optimisation-UiPath
- **Power BI dashboard (this repository)**

## About the dashboard

The dashboard reads from the same MySQL database (`cvstream`) that the UiPath bot fills with applicant data and the HR portal displays. It gives HR a visual overview of the recruitment process.

| Page | What it shows |
|------|---------------|
| Recruitment Overview | High-level recruitment figures and trends |
| Applicant Overview | Applicants across jobs, skills and applications |
| Applicant Details | A drill-through page with one applicant's education, experience and skills |



A full PDF export is also available

The dashboard uses these tables from the `cvstream` database:

- `applicants`
- `applications`
- `jobs`
- `skills`
- `job_skills`
- `applicant_skills`
- `education`
- `experience`
- a flattened applicant skills table and an applicant view

## Built with

- Power BI Desktop
- MySQL (via the Power BI MySQL connector)
- DAX and Power Query

## Recreating the dashboard

1. Install Power BI Desktop and the MySQL connector.
2. Create a new report and choose **Get data → MySQL database**.
3. Enter your own server and database name, and sign in with your own credentials.
4. Load the tables listed above and rebuild the relationships between them.
5. Build the three report pages shown in the preview.

## Author

Ruvimbo Mandava
