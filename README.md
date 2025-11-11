# Capstone-Project-Automated-Expense-Categorization-and-Summary-Report-Generation-using-UiPath
## NAME:DHARUNYADEVI S
## REGISTER NUMBER:212223220018
## AIM:
To automate the process of reading personal transaction data from a CSV file, categorize each expense according to its description, and generate a summary report of total spending in each category using UiPath Studio.

## ALGORITHM:
### Step 1: 
Start UiPath Workflow.

### Step 2: 
Read the CSV file containing transactions (with columns Date, Description, Amount) into a DataTable.

### Step 3: 
Initialize a Dictionary to track category totals (e.g., Food, Transport, Bills, Others).

### Step 4:
For Each Row in DataTable:
  * Convert Description to lowercase.
  * Parse Amount as Double.
  * Use If/Else logic to:
     1.Add Amount to "Food" total if Description matches food keywords.
     2.Add Amount to "Transport" if Description matches transport keywords.
     3.Add Amount to "Bills" if Description matches bill keywords.
     4.Otherwise, add Amount to "Others".

 ### Step 5:
 Build a Summary DataTable with columns: Category, Total, Date.

 ### Step 6
 For Each KeyValuePair in Dictionary:
    * Add a row to the summary DataTable with Category name, Total spent, and current Date.

### Step 7
Write the summary DataTable to a new CSV report file (e.g., ExpenseSummary.csv).

### Step 8
End the workflow.

## PROGRAM:
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4de83851-7235-40f8-923d-641432b2c125" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7a2817d2-e00f-491d-9603-cef953c1f00b" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/658d6cdf-f8f9-44ff-a534-5bd81b6f79d7" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c5811d72-04c9-4334-bb54-88c576dfcdf3" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b25cf968-ac3d-403e-86fc-eff84cd6abe8" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/06ef44df-911c-47a1-baed-60d8f2093eb7" />

## OUTPUT:
#### transactions.csv
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c4d5cec7-c73d-4ae7-9ac3-a9822c8f9632" />

#### ExpenseSummary.csv
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e62178f3-640e-4fea-9a21-d6267c595a2c" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a3af530f-8e14-48e2-adb9-8a673d7096f7" />


RESULT:
The workflow successfully categorizes transaction data based on their description into groups and generates a daily summary in a structured CSV file with date tracking.
