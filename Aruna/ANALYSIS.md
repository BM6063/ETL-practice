**BM6063 - ETL Practice**

**Patient Demographics**

1. How many unique patients can you identify in the data? - 275
2. Provide a stratification of patients by:
    1. Gender 
        1. Male - 57 percent 
        2. Female - 43 percent
    2. Marital status 
        1. Single - 110 
        2. Married - 72 
        3. Widowed - 54 
        4. Divorced - 27 
        5. Other - 12
    3. Language 
        1. English - 255 
        2. Other - 20
    4. Race
        1. White - 170
        2. Black/African American - 48
        3. Unknown - 17
        4. Hispanic/Latino - Cuban - 9
        5. Portuguese - 7


3. What percentage of patient are dead? - 94.6 percent

**Clinical Coding**

1. What version(s) of ICD were used for recording conditions/diagnoses? - ICD 10 and ICD 9
2. What version(s) of ICD were used for recording procedures? - ICD 10 and ICD 9
3. Identify the fields where these ICD codes are stored - icd_code
4. Are there any other coding systems present in the data (e.g., CPT, LOINC)? - DRG 

**Admission Analysis**

1. List all admission types present in the data 
    1. EW EMER.
    2. OBSERVATION ADMIT
    3. URGENT
    4. EU OBSERVATION
    5. SURGICAL SAME DAY ADMISSION
    6. DIRECT EMER.
    7. ELECTIVE
    8. DIRECT OBSERVATION
    9. AMBULATORY OBSERVATION
    
2. Which admission type is the most frequent? (provide count/percentage) - EW EMER. - 104 
3. Which admission type is the least frequent? (provide count/percentage) - AMBULATORY OBSERVATION - 5

**Table Structure Analysis**

1. What are the main tables identified in the scan report? - Admissions, Patients, poe, Presrcriptions, services, transfers 
2. Which table contains patient demographic information? - patients
3. Which table(s) contain diagnoses/conditions? - admissions
4. Which table(s) contain procedures? - poe
5. How many total rows are in each table identified above? - 45154
