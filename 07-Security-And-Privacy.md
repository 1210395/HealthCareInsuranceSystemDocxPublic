# Security and Privacy

## Overview

This system handles some of the most sensitive information a person has: their identity, their medical records, and their financial details. Protecting this information is a top priority. This document explains, in simple terms, how the system keeps data safe.


## How Personal Data Is Protected

All sensitive personal information in the system is **encrypted**. Encryption is like locking information in a safe with a digital key. Even if someone were to somehow access the raw data stored in the system, they would see only scrambled, unreadable text. Only the system itself, using its secret key, can unlock and read the information.

This encryption happens automatically. Users do not need to do anything special. Every time personal information is saved, it is locked. Every time an authorized person needs to see it, the system unlocks it for them.


## What Data Is Protected

The following types of personal information are encrypted:

- **Full names** (first name, last name, father's name)
- **National ID numbers**
- **Phone numbers**
- **Email addresses**
- **Medical records and history**
- **Addresses and contact details**

Even within the system's internal storage, this information is never stored in plain, readable form.


## Login Security

The system uses several measures to keep accounts secure:

### Strong Passwords
Users must create strong passwords when they register. Weak passwords that are easy to guess are not accepted.

### Automatic Session Timeout
If a user is inactive for a period of time, the system automatically logs them out. This prevents someone from accessing the system if a user walks away from their computer or loses their phone.

### Limited Login Attempts
If someone tries to log in with the wrong password too many times, the system temporarily blocks further attempts. This prevents attackers from trying thousands of password combinations to break into an account.

### Secure Login Tokens
After logging in, the system uses a secure token (think of it as a temporary digital pass) to verify the user's identity for each action they take. This token expires after a set time, requiring the user to log in again.


## Who Can See What

The system follows the principle of **least privilege**: every person can only see the minimum amount of information needed to do their job.

- **Patients** can only see their own information and their family members' information.
- **Doctors** can see medical information for their own patients, but not for other doctors' patients.
- **Pharmacists** can see prescription information but not financial claim details.
- **Lab Technicians** can see lab requests but not prescriptions or radiology information.
- **Radiologists** can see imaging requests but not lab results or prescriptions.
- **Medical Admins** can see medical claim details but not financial processing details.
- **Coordination Admins** can see financial claim details for processing.
- **Insurance Managers** have the broadest access for system administration, but even their access is logged and monitored.
- **Organization staff** can only see data within their own hospital or clinic.

Every request to view or change information is checked against the user's role before the system responds. Unauthorized requests are blocked immediately.


## Chat Privacy

The system includes a support chat feature for communication between patients and insurance staff. All chat messages are encrypted, just like personal data. This means:

- Messages cannot be read by anyone other than the intended participants.
- Chat history is stored securely.
- Even system administrators cannot read the content of private chat messages without proper authorization.


## Data Retention

This system follows a strict policy: **nothing is permanently deleted.**

When a record is "deleted" by a user (for example, removing a family member from a plan, or canceling a claim), it is not actually erased from the system. Instead, it is **hidden from view**. The record still exists in the background, marked with who removed it and when.

Why? Because in healthcare and insurance:
- There may be legal requirements to keep records for a certain number of years.
- Disputes may arise that require looking at historical data.
- Accidental deletions can be reversed.
- A complete history ensures accountability.

Certain records, such as claims, lab results, and radiology results, cannot be deleted at all, even in a hidden way. They are permanent parts of the medical record.


## Audit Trail

Every important action in the system is automatically recorded in an audit trail. This is a log that captures:

- **Who** performed the action (which user)
- **What** they did (created, updated, approved, rejected, etc.)
- **When** they did it (date and time)
- **What changed** (the before and after values, when applicable)

The audit trail cannot be edited or deleted by anyone. It serves as a permanent record of accountability. If there is ever a question about why a claim was rejected, who approved a payment, or when a policy was changed, the audit trail has the answer.

This is important for:
- **Accountability:** Everyone's actions are recorded.
- **Dispute resolution:** If a patient or provider disputes a decision, the history is available.
- **Compliance:** Regulatory authorities may require proof of proper procedures.
- **Quality control:** Patterns of errors or issues can be identified and addressed.


## What the System Does NOT Do

It is equally important to understand what this system does **not** do with your data:

- **Does not share data with third parties.** Your personal and medical information is not sold, shared, or made available to any outside company, advertiser, or organization.
- **Does not use data for advertising.** You will never see targeted advertisements based on your medical history or insurance activity.
- **Does not allow bulk data export.** Individual users, even administrators, cannot download the entire database of patient records.
- **Does not store unnecessary data.** The system only collects and stores information that is directly needed for healthcare insurance operations.

Your data exists in this system for one purpose only: to manage your healthcare insurance effectively and securely.
