<h1>Invoice Automation</h1>

<h2>Description</h2>

💼 **Overview**  
- Designed and implemented a Python-based automation script to streamline invoice processing for accounts payable workflows.  
- The script automatically filters unpaid invoices from Excel files, calculates the total amount due, and simulates a SharePoint upload by copying output reports to a designated folder.  
- This project demonstrates practical automation of a routine financial task, providing clear value in terms of time savings and data consistency.

🧰 **Key Points**  
- **Data Processing**: Uses `pandas` to extract and filter unpaid invoices from structured Excel files.  
- **Automation**: Replaces manual review with a script that processes and reports on invoice data.  
- **Simulation**: Mimics SharePoint document management by copying reports into a designated folder.  
- **Reporting**: Generates a concise summary of outstanding balances for financial insight.  

🚀 **Objectives**  
- Automate the extraction, filtering, and reporting of unpaid invoices from Excel data.  
- Simulate document upload to SharePoint to reflect enterprise file workflows.  
- Demonstrate entry-level scripting skills applicable to finance and accounting operations.  
- Lay the foundation for integration with real SharePoint APIs and dynamic reporting.

<h2>Project Walk-Through</h2>

**Step 1: Organize Folders for Automation**  
Created the following folder structure to support modular and scalable development:

- `Data/` for input invoice Excel files  
- `Output/` to store filtered unpaid invoices reports  
- `README.md` for project overview and usage instructions  
- `Scripts/` to hold the Python automation script  
- `SharePoint_Library/` to simulate SharePoint document storage

<br/>
<img src="https://imgur.com/TdZsJfO.png" height="50%" width="50%" />

---

**Step 2: Place Invoice Data File**  
Added a sample Excel file containing invoice records to the `Data/` folder. This file includes columns such as `Invoice Number`, `Customer`, `Amount`, and `Status`.  
<br/>
<img src="https://imgur.com/qhHnMG3.png" height="80%" width="80%" />

---

**Step 3: Write the Python Script**  
Created `process_invoices.py` inside the `Scripts/` folder with the following logic:

- Load invoice data with `pandas`  
- Print columns and preview data to verify structure  
- Filter out rows where `Status != "Paid"`  
- Calculate the total unpaid balance  
- Save results to `Output/unpaid_invoices.xlsx`  
- Simulate SharePoint upload by copying to `SharePoint_Library/unpaid_invoices.xlsx`  
- Display messages confirming each operation  

<br/>
<img src="https://imgur.com/bMOLEls.png" height="80%" width="80%" />

---

**Step 4: Run the Script**  
From the terminal, navigated to the `Scripts/` directory and ran the script using:
`python process_invoices.py`

<br/>
<img src="https://imgur.com/y8sG49n.png" height="80%" width="80%" />

---

**Step 5: Review Output Files**  
Opened the generated `Output/unpaid_invoices.xlsx` file to confirm that it only includes invoices marked as unpaid. Since invoice #3 was identified as paid, it does it appear in this list.
<br/>
<img src="https://imgur.com/cBHyT45.png" height="80%" width="80%" />

---

**Step 6: Verify SharePoint Simulation**  
Checked the `SharePoint_Library/` folder to verify that the report file was successfully copied, simulating a SharePoint upload.  
<br/>
<img src="https://imgur.com/Mm8wAd5.png" height="80%" width="80%" />

---

**Step 7: Summary & Next Steps**  
This project demonstrates how basic Python scripting can automate real-world accounting tasks. It streamlines invoice tracking, improves consistency, and lays the groundwork for integrating with actual SharePoint environments.  
Next steps could include:

- Using SharePoint APIs to perform actual uploads  
- Adding automated email notifications for unpaid invoices  
- Enhancing logic for aging reports or dynamic filters
