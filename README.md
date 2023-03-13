# Frozen Turnaround Time Reporting

Monthly turnaround time counts and summary statistics for frozen sections performed for UCHealth North (Greeley, MCR, and PVH)

## Overview

Frozen turnaround time report for UC Health North facilities (Greeley Hospital, Medical Center of the Rockies, and Poudre Valley Hospital). The script is a modification of the OPPE reporting script that is restricted to frozen sections and has its own folder under projects in the IT SharePoint site.

## Data

Query is performed in LigoLab

- Reporting > Dynamic Reports > Path-Dash

**Main Tab**

- Received = Last Month
- SURG and NON-GYN cases should be included
    - this is already filtered by the dynamic report

**Export Data**

- export data as YYYYq#-frozen.xls to IT > Projects > frozen-turnaround-time > data

## Output

Reports are produced with an Rmarkdown script (src > frozen.Rmd) . Knit (with parameters) a report for the month and save the resulting html file as PDF (print at 85% scaling in Chrome). Send turnaround time reports to Joel Karagacha ([joel.karagacha@uchealth.org](mailto:joel.karagacha@uchealth.org))

---

## Action items

- *The data files can also be copied over from the OPPE data.*
    - Script should be updated to pull data directly from OPPE project

---

### Notes, links, and updates
