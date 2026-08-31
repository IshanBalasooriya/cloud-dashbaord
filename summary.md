# Folder Summary

This folder contains a dataset of US cloud-computing job salaries and an interactive HTML dashboard built from it.

## Files

**data/cloud_platform_salaries.csv**
Created by: Claude (data generation — written directly as a CSV/text file, not through a document-creation tool)
Contents: 215 synthetic US cloud-role salary records, one row per posting, with columns Job Title, City, Salary, Experience Level, Cloud Platform, and Company Size. Covers 20 job titles (e.g. Cloud Solutions Architect, DevOps Engineer, Site Reliability Engineer, FinOps Analyst) across 10 US cities, three cloud platforms (AWS, Azure, GCP), three experience levels, and three company sizes.

**dashboard/cloud_salary_dashboard.html**
Created by: Claude, using the dataviz skill to build a self-contained HTML/Chart.js dashboard
Contents: A dark-themed, single-file interactive dashboard titled "Cloud Salary Dashboard" that visualizes cloud_platform_salaries.csv with six charts — average salary by role, average salary by city, records by cloud platform, average salary by cloud platform, average salary by experience level, and average salary by company size — plus a table of the top 10 highest-paid postings under the current filter.

**charts/**
Empty. No standalone chart image files (PNG/SVG/JPG) currently exist in this folder — all charts are rendered live inside the dashboard via Chart.js rather than saved as separate images. This folder is ready to hold exported chart images if any are added later.

**summary.md**
Created by: Claude
Contents: this file — an index of every file in the folder, which tool produced it, and what it contains.

## Folder structure

```
Claude Compare/
├── charts/          (empty — no image files found)
├── dashboard/
│   └── cloud_salary_dashboard.html
├── data/
│   └── cloud_platform_salaries.csv
└── summary.md
```
