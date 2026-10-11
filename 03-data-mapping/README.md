# Salesforce Data Mapping

## 1. Purpose
Data mapping documents the Salesforce objects and fields used to organize information for the BrightTech Solutions CRM project.

## 2. Main Salesforce Objects

| Salesforce Object | Purpose | Example |
|---|---|---|
| Lead | Stores information about potential customers | A prospective customer before conversion |
| Account | Represents a company or organization | BrightTech Solutions |
| Contact | Represents a person associated with a company | Rahul Sharma |
| Opportunity | Represents a potential sales deal | BrightTech CRM Software Deal |
| Task | Records a follow-up activity | Follow Up Call |
| Product | Represents an item or service offered for sale | Only if configured in the project |

## 3. Object Relationships

### Lead Conversion
A qualified lead can be converted into an Account and Contact. An Opportunity can also be created during conversion, depending on the conversion choices.

### Account and Contact
An Account can have multiple associated Contacts. The Contact record links the person to the relevant organization.

### Account and Opportunity
An Account can have multiple Opportunities. Each Opportunity is associated with the customer account involved in the potential deal.

### Tasks and Activities
Tasks can be related to relevant Salesforce records and assigned to a user for follow-up.

## 4. Sample Opportunity Field Mapping

| Business Information | Salesforce Field |
|---|---|
| Deal name | Opportunity Name |
| Customer company | Account Name |
| Sales progress | Stage |
| Expected deal value | Amount |
| Expected closing date | Close Date |
| Assigned sales user | Opportunity Owner |
| Planned follow-up | Next Step |

## 5. Data Mapping Rules
- Use the appropriate Salesforce object for each record.
- Link opportunities to the correct accounts.
- Link contacts to the appropriate accounts.
- Record amounts and dates in the correct fields.
- Use valid Salesforce record relationships rather than entering duplicate customer information.

## 6. Outcome
This mapping provides a structured view of how Salesforce organizes customer and sales information for reporting and follow-up management.
