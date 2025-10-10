## Table name: person

### Reading from patients

![](md_files/image1.png)

| Destination Field | Source field | Logic | Comment field |
| --- | --- | --- | --- |
| person_id | subject_id | Use as it is. It must be unique.  Create a unique id for each patient based on their subject_id |  |
| gender_concept_id | gender | When M, replace with 8507 when Fm replace with 8532 |  |
| year_of_birth | anchor_year<br>anchor_age<br>anchor_year_group | Use as it is it. When year of birth is empty replace with 2030, drop entire record for that patient.<br>Use as it is.<br>Use as it is. |  |
| month_of_birth |  |  |  |
| day_of_birth |  |  |  |
| birth_datetime |  |  |  |
| race_concept_id |  |  |  |
| ethnicity_concept_id |  |  |  |
| location_id |  |  |  |
| provider_id |  |  |  |
| care_site_id |  |  |  |
| person_source_value |  |  |  |
| gender_source_value | gender |  |  |
| gender_source_concept_id | gender |  |  |
| race_source_value |  |  |  |
| race_source_concept_id |  |  |  |
| ethnicity_source_value |  |  |  |
| ethnicity_source_concept_id |  |  |  |

