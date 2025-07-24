#  📑 Analysis_of_PolicyDataset : 

This project Performes systematic cleaning of the dataset by handling missing values, removing duplicates, and standardizing data formats.
Ensured consistency across all fields to prepare high-quality data for analysis and visualization.

---

## 📝 Feature Information Of Policy Dataset : 

**`1. CUST_ID :`** A unique identifier assigned to each customer. This feature allows for tracking individual policyholders across different policies.
**`2. Description:`** The name of the executive or agent responsible for managing or processing the policy.<br>
**`3. BODY:`** Describes the body type of the insured vehicle. <br>
**`4. MAKE:`** The manufacturer or brand of the vehicle. <br>
**`5. MODEL:`** The specific model of the vehicle. <br>
**`6. USE_OF_VEHICLE:`** Specifies the primary usage of the insured vehicle. <br>
**`7. MODEL_YEAR:`** The manufacturing year of the vehicle. <br>
**`8. CHASSIS_NO:`**  The unique chassis number (Vehicle Identification Number - VIN) of the insured vehicle. <br>
**`9. REGN:`** The region or emirate where the vehicle is registered. <br>
**`10. POLICY_NO:`** The unique identification number for each insurance policy. <br>
**`11. POL_EFF_DATE:`** The effective date from which the insurance policy coverage begins. <br>
**`12. POL_EXPIRY_DATE:`** The date on which the insurance policy coverage expires. <br>
**`13. SUM INSURED:`** The insured value of the vehicle, representing the maximum amount the insurance company would pay in case of total loss or significant damage. <br>
**`14. POL_ISSUE_DATE:`** The date and time when the insurance policy was issued. <br>
**`15. PREMIUM2:`** The amount of premium paid for the insurance policy. <br>
**`16. DRV_DOB:`** Date of Birth of the driver. Note that this field has missing values. <br>
**`17. DRV_DLI:`** Driver's Driving License Information or ID. Note that this field has missing values. <br>
**`18. VEH_SEATS:`** The number of seating capacities in the insured vehicle. <br>
**`19. PRODUCT:`** The type of insurance product. <br>
**`20. POLICYTYPE:`** The specific type of policy. <br>
**`21. Unnamed: 20:`** An unlabelled column with a significant number of missing values. Its specific meaning is unclear from the data provided and may represent residual data or an uncaptured attribute.<br>

--- 
## 🔍 Objective : 
### 🎯 Project Goal : 
The goal of this project is to clean and standardize `Policy Type ` data from a ` raw Csv file ` using ` Python `. It focuses on handling missing values, correcting inconsistencies, and preparing the dataset for further analysis. The final output is a structured, clean ` Csv file ` ready for reporting or modeling .

### 📂 Dataset : 
- `PolicyDetail` data primarily stores the insurance information of vehicle with also other feature like (`"MAKE' , "MODEL", "USE_OF_VEHICLE"`) which tells about the vehicle.
- It also stores the information about the driver like (`driving licence issue & expire date` ).
- It also stores the information regarding the insurance like ( `total insurance amount , Premium amount , Type of Insurance service,Policy expire Date`).

## 🧹 Notebook Processes to the datasets in these steps : 

### ✅ Step 1: Import Required Libraries
The notebook begins by importing useful libraries like:
- `pandas` for data handling
- `numpy` for numerical operations

### ✅ Step 2: Load the Csv File
- Reads the raw `.csv`  file using `pd.read_csv()`
- Displays the initial rows to understand the structure

### ✅ Step 3: Data Inspection
- Identifies missing values
- Inspects column names, data types, and formatting issues
- Indentifies the column either have large amount of missing values or no need for visualisation 

### ✅ Step 4: Data Cleaning
- Renames and standardizes column names
- Removes unnecessary rows or columns
- Cleans inconsistent entries in string or categorical columns
- Handles empty or corrupted values
- Remove the unnecessary literals like(`"," , "." `) in data field.
- Change the data type of column to correct data type.
- Fill the missing values in Categorical data by (`.mode()`) method and in numeric format fill by (`.mean()`) method.
- Drop the `Unnamed Column` of dataset.

### ✅ Step 5: Exporting Clean Data
- Saves the cleaned data as `policyTypeCleaned.csv` by using `.to_csv()` function. 


---

## 📋 Requirements : 
- Pandas
- Numpy
- Jupyter Lab

---

## 💡 Learning Outcomes : 
#### By following this notebook, you will:

- Learn how to read and inspect Csv files

- Gain experience in practical Pandas operations

- Understand the value of clean, structured data

- Learn how to export cleaned data back to `.csv` file


--- 

## ✅ Summary : 

✅ Cleaned and standardized messy insurance policy data.

✅ Removed duplicates and filled or removed missing values.

✅ Prepared the dataset for visual analysis or modeling.

✅ Built a reproducible notebook for future use or scaling.


---

