# QuicksightAiRules

Subject identification rule

If the user's question references "Financial Literacy" or "Maths" (in either wording, singly or together, case-insensitive), filter Opportunities where Subject equals "Financial Literacy and Maths" — this is a single combined picklist value in Salesforce, not two separate subjects.

Date range handling rule

If a user's question mentions or implies a date range (e.g., "last quarter," "this year," "between January and March," "year to date"), do not assume which date field to use.
Before running any query, ask the user to clarify which date field should be applied (for example: Created Date, Close Date, License Start Date, Enrollment Date — whichever date fields exist in the dataset).
Only query the data once the user has explicitly confirmed the date field to use.
Do not proceed with a default or "best guess" date field, even if one seems likely.
