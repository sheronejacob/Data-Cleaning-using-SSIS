# Data-Cleaning-using-SSIS
This project simulates a real-world ETL pipeline in which weekly customer data is extracted from a flat file (CSV format), cleaned, deduplicated, and loaded into SQL Server using SSIS. A stored procedure also summarizes customer counts by city.

## Tools Used:
1. Flat File (.csv)
2. Visual Studio / SSDT
3. SQL Server
4. SSIS (SQL Server Integration Services)

## ETL Steps
1. **Flat File Source** – Imported customer data from CSV file.
2. **Derived Column** – Replaced null phone numbers with a specific format of 0's.
3. **Data Conversion** – Formatted signup_date by changing datatype from string to DATE.
4. **Sort + Deduplicate** – Removed duplicate records.
5. **OLE DB Destination** – Loads into stg_Customers table.
6. **Execute SQL Task** – Runs stored procedure to populate summary table.
   
## Screenshots
PACKAGE CONTROL FLOW
![control_flow](https://github.com/user-attachments/assets/2ced8e35-b646-481d-8e85-811be4c1cecc)
PACKAGE DATA FLOW
![data_flow](https://github.com/user-attachments/assets/83ba3e88-f524-43c6-91c9-721eb54c4448)
SQL OUTPUT
![after_run](https://github.com/user-attachments/assets/e4682362-d5f0-4549-9cc0-dc9d6fef8c2b)

## Built by Sherone – Data Analyst, Canada



