<h1>Invoice Automation</h1>

<h2>Description</h2>
💼 Overview

  - Developed a Python-based automation script to process invoice data from Excel files. The script filters out unpaid invoices, calculates the total amount due, and simulates uploading the results to a SharePoint document library by copying files to a designated folder. This project streamlines accounts payable management and simulates integration with SharePoint workflows.

🧰 Key Points
  - Data Processing: Efficient filtering of unpaid invoices using pandas.

  - Automation: Eliminates manual review by automatically generating a report of outstanding invoices.

  - Simulation: Mimics SharePoint upload by copying the filtered invoice report to a dedicated SharePoint folder.

  - Reporting: Calculates and outputs the total outstanding balance for quick financial insight.

🚀 Objectives

  - Automate extraction and filtering of unpaid invoices from a master invoice Excel file.

  - Generate clear, actionable reports to support accounts payable workflow.

  - Demonstrate file system automation as a proxy for SharePoint document management.

  - Build foundational skills in Python scripting for finance-related automation.

<h2>Project Walk-Through:</h2>
Step 1: Organize Folders for Automation

Create the folder structure to organize the files.

<img src="https://imgur.com/TdZsJfO.png" height="50%" width="50%" />

Data/ for input invoice Excel files.

Output/ to store filtered unpaid invoice reports.

README.md for project overview and usage instructions.

Scripts/ to hold the Python automation script.

SharePoint_Library/ to simulate SharePoint document storage.

Step 2: Place Invoice Data File

Add the Excel invoice records into the Data/ folder.

<img src="https://imgur.com/qhHnMG3.png" height="80%" width="80%" />

Step 3: Write the Python Script
Create process_invoices.py inside Scripts/ folder with the following logic:

Load the invoice data with pandas.

Print columns and preview rows to verify data.

Filter out invoices where Status is not “Paid.”

Calculate the total amount due on unpaid invoices.

Save filtered invoices to Output/unpaid_invoices.xlsx.

Simulate SharePoint upload by copying this file to SharePoint_Library/unpaid_invoices.xlsx.

Print confirmation messages at each stage.

<img src="https://imgur.com/bMOLEls.png" height="80%" width="80%" />

Step 4: Run the Script
From the terminal, navigate to the Scripts/ directory and run:

(change to code format)python process_invoices.py

<img src="https://imgur.com/y8sG49n.png" height="80%" width="80%" />

Step 5: Review Output Files
Open Output/unpaid_invoices.xlsx to verify that only unpaid invoices remain.

<img src="https://imgur.com/vLRWgTd.png" height="80%" width="80%" />

Step 6: Verify SharePoint Simulation
Navigate to the SharePoint_Library/ folder and confirm that the unpaid invoices file is copied there. This simulates uploading to SharePoint.

<img src="https://imgur.com/Mm8wAd5.png" height="80%" width="80%" />

Step 7: Summary & Next Steps
This project automates a common accounts payable task, making invoice tracking faster and more reliable. As a next step, this could integrate actual SharePoint APIs for real upload capabilities, add email notifications for unpaid invoices, or extend filters for dynamic report generation.
