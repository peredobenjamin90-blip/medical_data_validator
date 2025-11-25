# Medical Data Validator  
### A Python project built as part of the freeCodeCamp Certification

## 📌 Overview
The **Medical Data Validator** is a simple Python tool that checks the validity of a collection of medical records. Each record must follow specific formatting rules for fields like `patient_id`, `age`, `gender`, `diagnosis`, `medications`, and `last_visit_id`.

This project was created as part of the **freeCodeCamp Scientific Computing with Python Certification**.

## 🚀 Features
- Validates that the input is a list or tuple  
- Ensures each item is a dictionary with the correct keys  
- Checks:
  - Patient ID format (e.g., `P1001`, case-insensitive)
  - Age is an integer ≥ 18
  - Gender is "male" or "female"
  - Diagnosis is a string or `None`
  - Medications is a list of strings
  - Visit ID format (`V####`)
- Prints detailed error messages showing:
  - Which field is invalid  
  - What value caused the failure  
  - The record index where the error occurred  

## 📁 File Structure


## 🧩 How It Works
The validator uses two main functions:

### `find_invalid_records()`
Checks each field in a single patient record and returns a list of invalid keys.

### `validate()`
Runs full validation on a list of medical records and prints:
- `"Valid format."` if everything is correct  
- Error messages for each invalid item  

## 🧪 Example Use
```python
from validator import validate
validate(medical_records)
