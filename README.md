# Protocol for Audio Data Sorting  
**Butabika Hospital Call Center (PBX System)**

---

## Overview
This repository documents the **audio data sorting protocol** used for telephone call recordings from **Butabika Hospital’s Call Center PBX system**.

The protocol defines how **non-clinical, global audio metadata** is manually labeled to prepare call audio for **future clinical and research annotation**, particularly in mental health research.

> ⚠️ **Important:** All sorting activities are conducted **exclusively on-site** within the PBX environment at Butabika Hospital. No data leaves the system.

---

## Purpose
- Organize raw PBX call recordings into a structured format  
- Capture global (non-clinical) call metadata  
- Enable downstream clinical annotation and research workflows  

---

## Scope
- Applies to **WAV audio files** stored on the PBX system  
- Annotation is done **manually in Excel** by listening to each audio file  
- The following are **strictly prohibited**:
  - Laptops
  - USB drives
  - External file transfers
  - Internet-based sharing or syncing

All work must remain within the **Butabika Call Center PBX desktop environment**.

---

## Sorting Parameters
Each annotator labels the following parameters.  
The **FileName** column must contain the **exact audio file name**, copied directly from the folder.

### 1. FileName
- Exact name of the audio file (no modification)

---

### 2. CallerSex
Perceived sex of the caller based on voice, self-identification, or statements made during the call.

**Expected values:**
- Male  
- Female  
- Unclear  

> Use **Unclear** if sex cannot be confidently determined (e.g., poor audio, child’s voice, no speech).  
> All *Unclear* cases must be briefly explained in the **Comment** column.

---

### 3. CallerPurpose
Primary reason for the call.

**Expected values:**
- Related to mental health patient diagnosis  
- Other health condition  
- Other query  
- Administrative inquiry (e.g., hospital procedures, admission rules)  
- Appointment-related (e.g., scheduling, confirming reviews)  
- Seeking services (e.g., treatment options, lab, referrals)  
- Other (must be clarified in **Comment**)

---

### 4. CallerType
Identifies who is making the call.

**Expected values:**
- Patient (calling about their own condition)  
- Caretaker (parent, spouse, sibling, etc.)  
- Community member (concerned citizen reporting a case)  
- Healthcare provider (consultation or referral-related)  
- Institutional representative (school, church, NGO, workplace, etc.)  
- Law enforcement (police or security services)  
- Hospital staff (non-clinical)  
- Student / Intern applicant  
- Unknown  

---

### 5. PatientStatus
Indicates whether the person discussed is already in mental health care.

**Expected values:**
- In care at a hospital  
- Under care elsewhere  
- Not under care  
- Referred for admission  
- Re-admission after defaulting  
- Unclear  
- Other (must be clarified in **Comment**)

---

### 6. Language
Dominant language spoken during the call.

**Expected values:**
- Luganda  
- English  
- Luganda-English  
- Runyankore  
- Lusoga  
- Luganda-Lusoga  
- Luganda-Runyankore  
- English-Runyankore  
- Unclear  
- Other (specify actual language(s) in **Comment**)

---

### 7. CallQuality
Rates how clear and understandable the call is.

**Scale (Likert):**
- 1 – Very poor  
- 2 – Poor  
- 3 – Fair  
- 4 – Good  
- 5 – Excellent  

If quality is poor but the call is still understandable, annotation may continue.  
If the audio is too unclear, annotators should stop and explain in **Comment**.

---

### 8. Diagnosis / Symptoms
Captures any diagnosis mentioned or symptoms described.

**Format:**  
- Comma-separated list of diagnoses and/or symptoms  

This may include inferred conditions based on medication or symptom descriptions.

---

### 9. ReasonNotLabeled
Filled **only if the call cannot be labeled at all**.

**Expected values:**
- No recording (silent or empty file)  
- System testing (test call, no meaningful content)  
- Very short call (under ~3–5 seconds)  
- Poor audio quality (too noisy or distorted)

---

## Folder Structure and Setup

### Folder Setup (by PBX Engineer)
For each annotator (e.g., *Ruth Neumbe*):

