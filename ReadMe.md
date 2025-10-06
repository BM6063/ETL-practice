# ETL Assignment

## Overview
This exercise involves analyzing a synthetic data hosted on a PostgreSQL database and creating an ETL (Extract, Transform, Load) mapping to the OMOP Common Data Model (CDM). Imagine yourself as a Data Scientist - Have fun!

## Part 1: Data Scanning and Analysis

### Task 1.1: Scan the Database with WhiteRabbit
1. **Install WhiteRabbit Software** (if not already installed). Run using the following connection details.
   
2. **Configure Connection**:
   - **Database Type**: `PostgreSQL`
   - **Server Location**: `54.74.73.233:5432/exercise_db`
   - **Username**: `postgres`
   - **Password**: `exercise`
   - **Database name**: `mimic_schema`
  
NB: Remember to test connection.

3. **Run the Scan**:
   - Scan all tables in the `mimic_schema`
   - Generate a comprehensive scan report
   - Save the scan report as `name.xlsx`

### Task 1.2: Answer the Following Questions

Based on the provided WhiteRabbit scan report (`ScanReport.xlsx`) and database exploration, answer these questions in a markdown file (`ANALYSIS.md`):

1. **Patient Demographics**
   - How many unique patients can you identify in the data?
   - Provide a stratification of patients by:
     - Gender.
     - Marital status.
     - Language.
     - Race.
   - What percentage of patient are dead?

2. **Clinical Coding**
   - What version(s) of ICD were used for recording conditions/diagnoses?
   - What version(s) of ICD were used for recording procedures?
   - Identify the fields where these ICD codes are stored
   - Are there any other coding systems present in the data (e.g., CPT, LOINC)?

3. **Admission Analysis**
   - List all admission types present in the data
   - Which admission type is the most frequent? (provide count/percentage)
   - Which admission type is the least frequent? (provide count/percentage)

4. **Table Structure Analysis**
   - What are the main tables identified in the scan report?
   - Which table contains patient demographic information?
   - Which table(s) contain diagnoses/conditions?
   - Which table(s) contain procedures?
   - How many total rows are in each table identified above?


## Part 2: ETL Mapping Documentation

### Task 2.1: Create OMOP CDM Mappings

Create and generate ETL mapping document (`ETL_MAPPING.md`) that details how data maps to OMOP CDM tables using Rabbit in a hat. Use the CDM v5.4. Focus on:

#### Required Mappings:
1. **Demographics** 
2. **Death**
3. **Conditions/Diagnoses** 
4. **Visits/Admissions**


#### Optional (if time permits):
4. **Treatments**
5. **procedures**
7. **Be happy to explore more**


### Task 2.2: Specify Concept IDs

In your ETL documentation, explicitly state:

1. **Gender Mapping**:
   - What `concept_id` will you use for Male (M)?
   - What `concept_id` will you use for Female (F)?
   - What about other gender values if present?

2. **Visit Type Mapping**:
   - What `visit_concept_id` will you use for each admission type in your data?
  
3. What concept id would you use for the language? 

4. **Vocabulary Mappings**:
   - How will you map ICD codes to OMOP standard concepts?
   - What source vocabulary concept IDs will you use?

use  [ATHENA Vocabulary Browser](https://athena.ohdsi.org/) to search for concepts.
### ETL Documentation Structure

Your `ETL_MAPPING.md` should include:
- Source table and field
- Target OMOP CDM table and field
- Transformation logic
- Concept ID mappings
- Data type conversions
- Handling of NULL values
- Business rules and assumptions


## Part 3: Version Control Submission

### Before You Start
To avoid conflicts, create your own branch:
```bash
git checkout -b yourname/id
```
Example: `git checkout -b john_doe/001`

### After Completion of exercise
Submit your work using Git:
```bash
# Stage all your files
git add .

# Commit with a descriptive message
git commit -m "Add ETL mapping documentation and scan report - [Your Name]"

# Push to your branch
git push origin yourname/id
```

### Required Deliverables
Your repository submission must include:
1. **WhiteRabbit Scan Report** (`name.xlsx`) 
2. **Analysis Document** (`ANALYSIS.md`) - answering all questions from Part 1
3. **ETL Mapping Documentation** (`ETL_MAPPING.md`) - complete ETL specifications
4. **README.md** - summary of your work and any assumptions made


## Part 4: ETL Script Implementation (Optional - Try if you have time)

### Task 4.1: Generate ETL Scripts
If you'd like an additional challenge, implement your ETL mapping:

1. **Choose Your Language**: Python, R, SQL, or any language you're comfortable with
2. **Generate Scripts**: Create scripts that transform the data to OMOP CDM format based on your ETL documentation
3. **Output Format**: Generate CSV files for each OMOP CDM table:
   - `person.csv`
   - `death.csv`
   - `condition_occurrence.csv`
   - `drug_exposure.csv`
   - `procedure_occurrence.csv`


4. **Include**:
   - Source code in a `scripts/` directory
   - Generated CSV files in an `output/` directory
   - Update your README with instructions on how to run the scripts


## Resources

### OMOP CDM Documentation
- [OMOP CDM v5.4 Specifications](https://ohdsi.github.io/CommonDataModel/)
- [ATHENA Vocabulary Browser](https://athena.ohdsi.org/)

### WhiteRabbit
- [WhiteRabbit Documentation](https://ohdsi.github.io/WhiteRabbit/)


---

## Questions?

If you encounter any issues:
send a mail to: `akwuru.david@ul.ie`. Happy to learn from you.

Good luck!
