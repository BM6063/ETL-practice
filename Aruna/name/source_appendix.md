# Appendix: source tables

### Table: admissions

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint | 10014354 |  |
| hadm_id | bigint |  |  |
| admittime | timestamp without time zone |  |  |
| dischtime | timestamp without time zone |  |  |
| deathtime | timestamp without time zone |  |  |
| admission_type | text | EW EMER. |  |
| admit_provider_id | text | P41R5N |  |
| admission_location | text | EMERGENCY ROOM |  |
| discharge_location | text | HOME HEALTH CARE |  |
| insurance | text | Other |  |
| language | text | ENGLISH |  |
| marital_status | text | SINGLE |  |
| race | text | WHITE |  |
| edregtime | timestamp without time zone |  |  |
| edouttime | timestamp without time zone |  |  |
| hospital_expire_flag | bigint | 0 |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:56:41.812825 |  |
| source_file | text | admissions |  |

### Table: d_hcpcs

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| code | text |  |  |
| category | double precision | 1 |  |
| long_description | text |  |  |
| short_description | text | Musculoskeletal system |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:56:42.893618 |  |
| source_file | text | d_hcpcs |  |

### Table: d_icd_diagnoses

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| icd_code | text |  |  |
| icd_version | bigint | 10 |  |
| long_title | text |  |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:56:52.323232 |  |
| source_file | text | d_icd_diagnoses |  |

### Table: d_icd_procedures

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| icd_code | text |  |  |
| icd_version | bigint | 10 |  |
| long_title | text |  |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:04.540058 |  |
| source_file | text | d_icd_procedures |  |

### Table: d_labitems

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| itemid | bigint |  |  |
| label | text | Delete |  |
| fluid | text | Blood |  |
| category | text | Hematology |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:14.307278 |  |
| source_file | text | d_labitems |  |

### Table: drgcodes

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint | 10014354 |  |
| hadm_id | bigint |  |  |
| drg_type | text | HCFA |  |
| drg_code | bigint | 720 |  |
| description | text | SEPTICEMIA & DISSEMINATED INFECTIONS |  |
| drg_severity | double precision |  |  |
| drg_mortality | double precision |  |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:56:42.407595 |  |
| source_file | text | drgcodes |  |

### Table: emar

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint | 10014354 |  |
| hadm_id | double precision | 28258130 |  |
| emar_id | text |  |  |
| emar_seq | bigint | 21 |  |
| poe_id | text | 10005866-999 |  |
| pharmacy_id | double precision |  |  |
| enter_provider_id | text |  |  |
| charttime | timestamp without time zone | 2147-12-10 08:26:00 |  |
| medication | text | Sodium Chloride 0.9%  Flush |  |
| event_txt | text | Administered |  |
| scheduletime | timestamp without time zone | 2148-01-06 08:00:00 |  |
| storetime | timestamp without time zone | 2147-12-10 08:27:00 |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:14.966449 |  |
| source_file | text | emar |  |

### Table: labevents

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| labevent_id | bigint |  |  |
| subject_id | bigint | 10035631 |  |
| hadm_id | double precision |  |  |
| specimen_id | bigint | 36129047 |  |
| itemid | bigint | 50912 |  |
| order_provider_id | text |  |  |
| charttime | timestamp without time zone | 2201-03-01 09:29:00 |  |
| storetime | timestamp without time zone |  |  |
| value | text |  |  |
| valuenum | double precision |  |  |
| valueuom | text | mg/dL |  |
| ref_range_lower | double precision |  |  |
| ref_range_upper | double precision |  |  |
| flag | text |  |  |
| priority | text | STAT |  |
| comments | text |  |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:22.704798 |  |
| source_file | text | labevents |  |

### Table: microbiologyevents

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| microevent_id | bigint |  |  |
| subject_id | bigint | 10021487 |  |
| hadm_id | double precision |  |  |
| micro_specimen_id | bigint | 3575952 |  |
| order_provider_id | text |  |  |
| chartdate | timestamp without time zone | 2117-10-26 |  |
| charttime | timestamp without time zone |  |  |
| spec_itemid | bigint | 70079 |  |
| spec_type_desc | text | URINE |  |
| test_seq | bigint | 1 |  |
| storedate | timestamp without time zone | 2117-10-31 |  |
| storetime | timestamp without time zone | 2117-10-31 13:18:00 |  |
| test_itemid | bigint | 90039 |  |
| test_name | text | URINE CULTURE |  |
| org_itemid | double precision |  |  |
| org_name | text |  |  |
| isolate_num | double precision |  |  |
| quantity | double precision |  |  |
| ab_itemid | double precision |  |  |
| ab_name | text |  |  |
| dilution_text | text |  |  |
| dilution_comparison | text |  |  |
| dilution_value | double precision |  |  |
| interpretation | text |  |  |
| comments | text |  |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:47.071355 |  |
| source_file | text | microbiologyevents |  |

### Table: omr

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint | 10019003 |  |
| chartdate | timestamp without time zone | 2138-10-31 |  |
| seq_num | bigint | 1 |  |
| result_name | text | Weight (Lbs) |  |
| result_value | text | 71 |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:48.422643 |  |
| source_file | text | omr |  |

### Table: patients

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint |  |  |
| gender | text | M |  |
| anchor_age | bigint | 63 |  |
| anchor_year | bigint |  |  |
| anchor_year_group | text | 2014 - 2016 |  |
| dod | timestamp without time zone |  |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:49.085192 |  |
| source_file | text | patients |  |

### Table: pharmacy

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint | 10014354 |  |
| hadm_id | bigint | 23831430 |  |
| pharmacy_id | bigint |  |  |
| poe_id | text |  |  |
| starttime | timestamp without time zone | 2150-04-10 07:00:00 |  |
| stoptime | timestamp without time zone |  |  |
| medication | text |  |  |
| proc_type | text | Unit Dose |  |
| status | text | Discontinued |  |
| entertime | timestamp without time zone | 2167-05-05 13:51:04 |  |
| verifiedtime | timestamp without time zone | 2167-05-05 13:51:04 |  |
| route | text | IV |  |
| frequency | text | ONCE |  |
| disp_sched | text |  |  |
| infusion_type | text |  |  |
| sliding_scale | text |  |  |
| lockout_interval | double precision |  |  |
| basal_rate | double precision |  |  |
| one_hr_max | double precision |  |  |
| doses_per_24_hrs | double precision |  |  |
| duration | double precision |  |  |
| duration_interval | text | Ongoing |  |
| expiration_value | double precision | 36 |  |
| expiration_unit | text | Hours |  |
| expirationdate | double precision |  |  |
| dispensation | text | Omnicell |  |
| fill_quantity | double precision |  |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:49.510842 |  |
| source_file | text | pharmacy |  |

### Table: poe

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| poe_id | text |  |  |
| poe_seq | bigint | 57 |  |
| subject_id | bigint | 10014354 |  |
| hadm_id | bigint | 28258130 |  |
| ordertime | timestamp without time zone | 2130-10-27 12:45:12 |  |
| order_type | text | Medications |  |
| order_subtype | text |  |  |
| transaction_type | text | New |  |
| discontinue_of_poe_id | text |  |  |
| discontinued_by_poe_id | text |  |  |
| order_provider_id | text |  |  |
| order_status | text | Inactive |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:57:54.84859 |  |
| source_file | text | poe |  |

### Table: poe_detail

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| poe_id | text |  |  |
| poe_seq | bigint | 83 |  |
| subject_id | bigint | 10014354 |  |
| field_name | text | Admit category |  |
| field_value | text | Admit to inpatient |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:58:02.768944 |  |
| source_file | text | poe_detail |  |

### Table: prescriptions

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint | 10014354 |  |
| hadm_id | bigint | 23831430 |  |
| pharmacy_id | bigint |  |  |
| poe_id | text |  |  |
| poe_seq | double precision |  |  |
| order_provider_id | text | P23H5V |  |
| starttime | timestamp without time zone | 2125-02-27 18:00:00 |  |
| stoptime | timestamp without time zone | 2135-01-19 14:00:00 |  |
| drug_type | text | MAIN |  |
| drug | text | Insulin |  |
| formulary_drug_cd | text | NACLFLUSH |  |
| gsn | text |  |  |
| ndc | double precision | 0 |  |
| prod_strength | text | 100 Units / mL - 10 mL Vial |  |
| form_rx | text |  |  |
| dose_val_rx | text | 1 |  |
| dose_unit_rx | text | mg |  |
| form_val_disp | text | 1 |  |
| form_unit_disp | text | TAB |  |
| doses_per_24_hrs | double precision |  |  |
| route | text | IV |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:58:03.540977 |  |
| source_file | text | prescriptions |  |

### Table: services

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint | 10014354 |  |
| hadm_id | bigint |  |  |
| transfertime | timestamp without time zone |  |  |
| prev_service | text |  |  |
| curr_service | text | MED |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:58:08.787079 |  |
| source_file | text | services |  |

### Table: transfers

| Field | Type | Most freq. value | Comment |
| --- | --- | --- | --- |
| subject_id | bigint | 10014354 |  |
| hadm_id | double precision |  |  |
| transfer_id | bigint |  |  |
| eventtype | text | transfer |  |
| careunit | text |  |  |
| intime | timestamp without time zone |  |  |
| outtime | timestamp without time zone |  |  |
| loaded_at | timestamp without time zone | 2025-10-05 17:58:09.289465 |  |
| source_file | text | transfers |  |

