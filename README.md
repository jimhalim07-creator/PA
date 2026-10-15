# CARE Egypt – Performance Appraisal Report

A single-page tool (`index.html`) that analyses the SharePoint **PerformanceAppraisals** list export and produces printable / downloadable appraisal PDFs.

**No data is stored in this repository or in the page.** The Excel file is read and processed entirely in the user's browser; nothing is uploaded or sent anywhere (the page's Content-Security-Policy blocks all network requests). Closing or reloading the page clears the data.

## How to use
1. In SharePoint, open the PerformanceAppraisals list with a view that includes the **Created** column, and choose **Export → Export to Excel**.
2. Open the downloaded file in Excel and **save it as .xlsx**.
3. Open the report page and drag the .xlsx onto it (or click **Load Excel file**).
4. Use the **Dashboard** for analysis, and **Employee appraisals** to print or download PDFs (single, ZIP of all, or one combined PDF).

Each employee is represented by their **highest-scoring submission**; the submission date shown is the SharePoint **Created** date of that submission.

## Publishing
Enable GitHub Pages for this repository (Settings → Pages → deploy from branch, root folder). Do not commit Excel exports – `.gitignore` excludes them.
