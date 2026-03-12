# Insurance Policy and Coverage

## What Is an Insurance Policy?

An insurance policy is a set of rules that determine what the insurance company will pay for and how much. Think of it as an agreement between the insurance company and its members: "If you need medical care, here is what we will cover."

Every patient has a policy. That policy tells the system exactly how much the insurance pays and how much the patient pays for any given medical service.


## How Coverage Works

Coverage rules in this system are organized in layers, from general to specific. The system always uses the most specific rule that applies.

### Layer 1: General Policy Rules

At the top level, the policy sets default rules that apply to everything. For example:
- "The insurance covers 80% of all medical costs."
- "The patient pays the remaining 20%."

This is the starting point. If no more specific rule exists, these general rules apply.

### Layer 2: Category-Specific Rules

The insurance company can set different rules for different categories of medical services. Categories might include:
- Doctor consultations
- Dental care
- Laboratory tests
- Radiology and imaging
- Prescription medicine
- Emergency services

For example, the policy might say:
- "Cover 80% of doctor consultations" (the general rule)
- "Cover 90% of dental care" (a category-specific rule)
- "Cover 70% of radiology" (another category-specific rule)

### Layer 3: Service-Specific Rules

For even more precision, the insurance company can set rules for individual services within a category. For example:
- Within the "Laboratory Tests" category: "Cover 100% of blood tests"
- Within the "Radiology" category: "Cover 50% of MRI scans"

### How the System Chooses Which Rule to Apply

**The most specific rule always wins.** Here is how the system decides:

1. First, it checks if there is a rule for the exact service (Layer 3).
2. If not, it checks if there is a rule for the service category (Layer 2).
3. If not, it uses the general policy rule (Layer 1).

**Example:**
A patient has a policy with these rules:
- General: Cover 80%
- Lab Tests (category): Cover 85%
- Blood Tests (specific service): Cover 100%

If the patient gets a blood test, the insurance covers 100% (the specific rule).
If the patient gets a urine test, the insurance covers 85% (the category rule).
If the patient gets a service not in any specific category, the insurance covers 80% (the general rule).


## How Policies Are Assigned to Providers

Healthcare providers (doctors, clinics, hospitals) are linked to insurance policies. This means:

- When a doctor submits a claim, the system knows which policy applies.
- Different providers may be linked to different policies.
- There is a "global" policy that automatically applies to all new providers unless a specific one is assigned.

When a provider joins the network, they are automatically assigned the current global policy. If the insurance company later changes the global policy, providers are updated accordingly.


## What Happens When a Policy Changes

Insurance policies may change over time. For example, the insurance company might adjust coverage percentages or add new services. Here is how the system handles this:

- **Existing claims keep the old rules.** If a claim was submitted when the policy said "cover 80%," that claim will always be processed at 80%, even if the policy later changes to 75%. The system takes a snapshot of the policy rules at the time the claim is created.
- **New claims use the new rules.** Any claim submitted after the policy change will use the updated rules.

This ensures fairness. No one is surprised by a change that affects a claim they already submitted.


## Multiple Policies

The insurance company can create multiple policies for different groups. For example:
- A "Standard" policy for regular members
- A "Premium" policy with higher coverage
- A "Basic" policy with lower coverage and lower premiums
- Organization-specific policies for particular hospitals or clinics

Each patient is covered under one policy at a time, and each provider works with one policy at a time.


## Maximum Amounts and Limits

Policies can include limits to control costs:

### Per-Claim Limits
A maximum amount the insurance will pay for a single claim. For example: "The insurance will cover up to 5,000 ILS per claim. Any amount above that is the patient's responsibility."

### Annual Limits
A maximum total amount the insurance will pay for a patient in one year. For example: "The insurance will cover up to 50,000 ILS per year per patient." Once this limit is reached, the patient pays for all remaining services that year.

### Category Limits
Maximum amounts for specific categories. For example: "Up to 10,000 ILS per year for dental care."

These limits help keep insurance premiums affordable while still providing meaningful coverage.


## Waiting Periods

Some policies include waiting periods for certain services. A waiting period means that a new member must wait a certain amount of time before they can use coverage for specific services.

For example:
- "Dental coverage begins 3 months after enrollment."
- "Elective surgery coverage begins 6 months after enrollment."

Waiting periods prevent people from signing up for insurance only when they know they need an expensive procedure, which would not be fair to other members who have been paying premiums regularly.


## Age and Gender Restrictions

Certain medical services are only relevant to specific groups, and policies can reflect this:

- Some services may only be covered for certain age ranges (for example, pediatric services for children, or geriatric services for elderly patients).
- Some services may only be covered for a specific gender (for example, certain reproductive health services).

These restrictions ensure that coverage rules match the medical reality of who would actually need specific services.


## Pre-Approval Requirements

For certain expensive or specialized services, the insurance company may require pre-approval before the service is provided. This means:

1. The doctor determines that the patient needs the service.
2. A request is submitted to the insurance company before the service is performed.
3. The insurance company reviews and approves (or denies) the request.
4. Only after approval does the patient receive the service with insurance coverage.

Pre-approval is typically required for:
- Expensive procedures
- Specialized treatments
- Services that have alternatives the insurance prefers

If a patient receives a service that required pre-approval without getting that approval first, the insurance may not cover it, or may cover it at a reduced rate.
