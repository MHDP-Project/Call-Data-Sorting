# Butabika Call Center Audio Data Sorting Protocol

## Description
This repository documents the protocol used to **sort and label telephone call audio recordings** from the Butabika Hospital Call Center PBX system.

The sorting process focuses on capturing **high-level, non-clinical metadata** from each call to structure the dataset for **future mental health research and clinical annotation**.  
No diagnostic decisions are made at this stage; labels reflect information **explicitly stated or reasonably inferred** from the audio.

---

## Labeled Parameters
Each audio file is reviewed manually and assigned the following metadata fields:

### 1. FileName
The exact name of the audio file as stored on the PBX system.

---

### 2. CallerSex
Perceived sex of the caller based on voice or self-identification.

**Values:**  
`Male`, `Female`, `Unclear`

---

### 3. CallerPurpose
The primary reason for the call.

**Values include:**  
- Mental health–related inquiry  
- Other health condition  
- Administrative inquiry  
- Appointment-related  
- Seeking services  
- Other

---

### 4. CallerType
Who is making the call.

**Values include:**  
- Patient  
- Caretaker  
- Community member  
- Healthcare provider  
- Institutional representative  
- Law enforcement  
- Hospital staff (non-clinical)  
- Student / Intern applicant  
- Unknown

---

### 5. PatientStatus
Care status of the person being discussed.

**Values include:**  
- In care at a hospital  
- Under care elsewhere  
- Not under care  
- Referred for admission  
- Re-admission after defaulting  
- Unclear  
- Other

---

### 6. Language
Dominant language(s) spoken during the call.

**Values include:**  
- Luganda  
- English  
- Luganda–English  
- Runyankore  
- Lusoga  
- Mixed languages  
- Unclear  
- Other

---

### 7. CallQuality
Overall clarity of the call audio.

**Scale:**  
1 (Very poor) → 5 (Excellent)

---

### 8. Diagnosis / Symptoms
Any diagnosis mentioned or symptoms described during the call.

**Format:**  
Comma-separated list of diagnoses and/or symptoms.

---

### 9. ReasonNotLabeled
Used only when a call cannot be labeled.

**Values include:**  
- No recording  
- System testing  
- Very short call  
- Poor audio quality

---

## Notes
This protocol supports **dataset structuring and quality control** and is intended to enable downstream annotation, analysis, and modeling in low-resource mental health research contexts.

