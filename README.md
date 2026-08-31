# Claude Compare

Same job, handed to different Claudes, to see how the results differ. The job: take a
dataset of US cloud-computing salaries and turn it into an interactive dashboard.

*Field notes from the bench — one dataset, several builds, and a verdict at the end.*

## The task

Given ~215 synthetic US cloud-role salary records (Job Title, City, Salary, Experience
Level, Cloud Platform, Company Size), build a **self-contained HTML dashboard** that
visualizes them with Chart.js — averages by role, city, platform, experience, and
company size, plus the top-paid postings. No Python, no build step, opens in a browser.

## What's in here

| File | Built by | Notes |
|---|---|---|
| `dashboard.html` | Claude Code | Dark, Apple-styled single file. 4 live filters, 7 charts, data embedded inline. |
| `dashboard/cloud_salary_dashboard.html` | Cowork | Earlier dark build via the dataviz skill — 6 charts + a top-10 table. |
| `data/cloud_platform_salaries.csv` | — | The dataset (also embedded in `dashboard.html`). |
| `cloud_salaries.txt` | — | Same data, as handed to Claude Code. |
| `summary.md` | — | Index of the Cowork run's output folder. |
| `which-claude-when.html` / `claude-tools-decision-card.md` | — | The verdict: Claude.ai vs Claude Code vs Cowork, and when to reach for each. |

## Running it

Open `dashboard.html` in a browser. Chart.js loads from a CDN, so it wants a network
connection on first load; everything else — data, styles, logic — is inline.
