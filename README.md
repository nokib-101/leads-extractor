# Leads Extractor

A one-page tool for Garibook's daily ad leads.

1. Open the site.
2. Drop the zip files from the marketing team (no need to unzip).
3. Click **Download Excel**: one file with **Bikes**, **Cars** and **Rejected** sheets.

What it does:
- Reads every lead form file inside the zips (file names are ignored).
- Keeps only Date, Phone, Name, Vehicle Model, form mobile, seats, own vehicle, city and source.
- Phone numbers are cut to the last 10 digits (Bangla digits are converted first).
- Dates are shown as year-month-day.
- Sorts each lead into Bike or Car using English and Bangla brand/model names, common misspellings and the seat count. CNG, pickup, truck and unclear answers go to Rejected with a reason.

**Privacy:** everything runs inside the visitor's browser. The zip files and lead data are never uploaded or stored.

To add a new spelling, edit the `BIKE`, `CAR` or `JUNK` lists near the top of the script in `index.html`.
