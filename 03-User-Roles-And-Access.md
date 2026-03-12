# User Roles and Access

## Overview

Every person who uses this system has a specific role. That role determines what they can see and what they can do. This keeps information secure and ensures that each person has exactly the tools they need to do their job, nothing more and nothing less.


## What Each Role Can Do

### Insurance Manager

The Insurance Manager is the overall system administrator for the insurance company. They have the broadest access of any role.

- View and manage all users in the system
- Approve or reject new user registrations
- Create and modify insurance policies
- Set coverage rules and limits
- View all claims across the entire system
- Access reports and statistics
- Manage organizations (hospitals and clinics)
- Initiate support chat conversations with users
- Configure system settings
- View audit records (a log of all important actions taken in the system)
- **Create custom admin roles**: The Insurance Manager can create custom administrators and assign them a specific subset of their own permissions. This allows delegation of duties — for example, creating an admin who can only manage user approvals, or one who can only view reports. Custom admins can never have more permissions than the manager who created them, and revoking a custom admin automatically removes any further admins that person created

### Medical Admin

The Medical Admin focuses on the medical validity of insurance claims.

- View all claims that need medical review
- Approve claims that are medically justified
- Reject claims that are not medically justified
- Return claims to providers with notes requesting more information
- View patient medical histories when relevant to a claim
- Access medical review statistics and reports

### Coordination Admin

The Coordination Admin focuses on the financial and policy aspects of claims, and handles payments.

- View all claims that have passed medical review and need financial review
- Approve claims from a financial and policy perspective
- Reject claims that do not meet policy requirements
- Return claims to providers for financial corrections
- Process payments for approved claims
- Record payment details (method, receipt numbers)
- Access financial reports and statistics

### Doctor

Doctors are healthcare providers who treat patients and submit claims.

- View their own patients and their medical histories
- Create and submit insurance claims after treating a patient
- Write prescriptions for patients
- Order lab tests for patients
- Order radiology (imaging) tests for patients
- View the status of claims they have submitted
- View and respond to return tickets (when a claim is sent back for corrections)
- Update or cancel prescriptions they have written

### Pharmacist

Pharmacists handle prescriptions and dispense medicine.

- View prescriptions assigned to their pharmacy or available for filling
- Verify prescription details (correct medicine, correct dosage)
- Mark prescriptions as dispensed (filled and given to the patient)
- View patient allergy and medication information relevant to prescriptions
- Report issues with prescriptions back to the prescribing doctor

### Lab Technician

Lab Technicians process laboratory test requests.

- View lab test requests assigned to them
- Update the status of lab tests (in progress, completed)
- Upload lab test results
- View relevant patient information needed for testing

### Radiologist

Radiologists process imaging and radiology requests.

- View radiology requests assigned to them
- Update the status of imaging procedures (in progress, completed)
- Upload imaging results and reports
- View relevant patient information needed for imaging

### Insurance Client (Patient)

Patients use the system to manage their healthcare insurance experience.

- View their own claims and claim history
- View their prescriptions
- View their lab test results
- View their radiology results
- Submit reimbursement claims (for out-of-network visits they paid for themselves)
- Manage family members on their insurance plan
- Receive notifications about claim updates
- Use the mobile app to show their insurance identity (QR code)
- Chat with insurance support staff
- View their insurance policy and coverage details


## Organization Roles

Hospitals and private clinics can register as organizations in the system. When they do, they have their own versions of the roles listed above. These organization roles work the same way, but are limited to that specific organization.

For example:
- An **Organization Doctor** can only see patients and claims within their hospital or clinic.
- An **Organization Medical Admin** can only review claims from their organization.
- An **Organization Admin** manages users and settings within their organization only.

The available organization roles are:
- Organization Admin (manages the organization)
- Organization Medical Admin
- Organization Coordination Admin
- Organization Doctor
- Organization Pharmacist
- Organization Lab Technician
- Organization Radiologist

This keeps each organization's data separate and private while still being part of the larger insurance system.


## How Access Is Controlled

The system follows a strict principle: **each person only sees what they need to see to do their job.**

- A doctor cannot see claims from other doctors' patients.
- A patient cannot see other patients' information.
- A pharmacist cannot see financial details of claims.
- A lab technician cannot see prescriptions.
- Organization staff cannot see data from other organizations.

Every time someone logs in, the system checks their role and only shows them the relevant information and actions. If someone tries to access something they should not, the system blocks the request.


## How New Users Join the System

Joining the system follows a clear process to ensure that only authorized people gain access:

### Step 1: Registration

The person fills out a registration form with their basic information:
- Name
- Contact details (email, phone number)
- National ID number
- The role they are requesting (for example: Doctor, Pharmacist, Patient)

### Step 2: Waiting for Approval

After registration, the account is placed in a pending state. The person cannot use the system yet.

An Insurance Manager (or Organization Admin, for organization staff) reviews the registration:
- They verify the person's identity and credentials.
- They confirm the requested role is appropriate.

### Step 3: Role Assignment and Activation

Once approved, the person is assigned their role and their account becomes active. They can now log in and use the system with the access that their role allows.

If the registration is rejected, the person is notified with an explanation.

### Important Notes:

- **Patients** go through a simpler process, as they are registering themselves for their own insurance access.
- **Healthcare providers** (doctors, pharmacists, etc.) may need to provide additional verification, such as medical license information.
- **Organization staff** are typically approved by their organization's admin rather than the insurance company directly.
- A person's role can be changed later by an Insurance Manager if their responsibilities change.
