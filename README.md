# Frozen Turnaround Time Reporting

Monthly turnaround time counts and summary statistics for frozen sections performed for UCHealth North (Greeley, MCR, and PVH) are run monthly and a quarterly summary is run for CRMC

## Overview

Frozen turnaround time report for UC Health North facilities (Greeley Hospital, Medical Center of the Rockies, and Poudre Valley Hospital) and Cheyenne Regional Medical Center (CRMC). The scripts are modifications of the OPPE reporting script that is restricted to frozen sections and has its own project folder under projects in the IT SharePoint site.

Frozen turnaround time report for CRMC. The script is a modification of the OPPE reporting script that is restricted to frozen specimens and has its own folder under the IT Reporting folder.

## Data

Query is performed in LigoLab

- Reporting > Dynamic Reports > Stats Pathologist TAT

**Main Tab**

UCHealth North
- Received = Last Month
- SURG and NON-GYN cases should be included
    - this is already filtered by the dynamic report

CRMC
- Received = Last Quarter
- SURG and NON-GYN cases should be included
    - this is already filtered by the dynamic report
- Client / Provider = 718 Cheyenne Regional Med Center

**Export Data**

UCHealth North
- export data as YYYY-MM-frozen.xls to IT > Projects > frozen-turnaround-time > data

CRMC
- export data as YYYYq#-frozen-crmc.xls to IT > Projects > frozen-turnaround-time > data

## Output

UCHealth North
Reports are produced with an Rmarkdown script (src > frozen_new-tat-fxn.Rmd) . Knit (with parameters) a report for the month and save the resulting html file as PDF (print at 85% scaling in Chrome). Send turnaround time reports to Joel Karagacha ([joel.karagacha@uchealth.org](<joel.karagacha@uchealth.org>) and [Kristin Marriott](<kmarriott@summitpathology.com>))

CRMC
Reports are produced with the 'frozen-tat-individual.Rmd' Rmarkdown script. Knit (with parameters), save as PDF (at 85% scaling), upload to the Compliance SharePoint site (Compliance > Pathologist Quality Data Reports > Cheyenne Regional Medical Center (Long) > TAT_Frozen-sections), and notify Dr. Long via email (<dlong@summitpathology.com>) or Teams

---

## Action items

- *The data files can also be copied over from the OPPE data.*
- Script should be updated to pull data directly from OPPE project

---

### Notes, links, and updates
