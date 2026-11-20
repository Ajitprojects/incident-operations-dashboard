# Incident Operations Dashboard

A lightweight portfolio demo for exploring incident status, operational metrics and incident timelines. All incidents and services are fictional. This is a static demonstration, not a live monitoring or incident management system.

## Run locally

Download the repository and open `index.html` in a modern browser. No installation, account or server is needed.

## Features

- View a sample incident queue and filter by status.
- Inspect fictional detection, escalation and recovery timelines.
- Compare incident counts by service.
- Calculate average time from incident start to detection and from start to recovery.

Metrics apply to the selected status filter. Detection averages include records with valid start and detection times. Recovery averages include resolved incidents with valid start and recovery times. Negative and invalid durations are excluded. An empty sample displays an em dash. Definitions of MTTD and MTTR vary between organisations; here they are simply the averages defined above, not claims about any real service.

## Sample calculation

Incident INC-1001 starts at 10:00 UTC, is detected at 10:03 UTC and recovers at 10:28 UTC. Detection time is 3 minutes and recovery time is 28 minutes. For all four sample incidents the average detection time is 5.8 minutes (rounded from 5.75); average recovery time for the three resolved incidents is 39.3 minutes (rounded from 39.33).

## How to explain this in an interview

> This is a simulated incident dashboard I used to practise interpreting operational metrics. It shows how incident timelines, status and service-level counts can support triage and communication. The data is fictional, and the calculations are defined explicitly. I can explain how start, detection and recovery timestamps are used and why open incidents are excluded from recovery averages.

## Limitations and future improvements

Data is embedded in the page and resets on reload; there is no backend, authentication or live integration. Possible next steps include importing CSV, date filtering, accessible charts, and automated tests.

## Technology

HTML, CSS and JavaScript; no external libraries.
