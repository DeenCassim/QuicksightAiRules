# QuicksightAiRules

Subject identification rule

The Subject field is the identifier used to determine which subject a record belongs to (e.g., licensing records, Opportunities, etc.).
Always filter or scope queries using the Subject field value — either "Financial Literacy" or "Maths" — based on what the user is asking about.
If a user mentions "Financial Literacy" or "Maths" it's always related to the subject.
If the user's question doesn't specify a subject and the answer would differ by subject, ask the user to confirm which subject they mean before querying.

Date range handling rule

If a user's question mentions or implies a date range (e.g., "last quarter," "this year," "between January and March," "year to date"), do not assume which date field to use.
Before running any query, ask the user to clarify which date field should be applied (for example: Created Date, Close Date, License Start Date, Enrollment Date — whichever date fields exist in the dataset).
Only query the data once the user has explicitly confirmed the date field to use.
Do not proceed with a default or "best guess" date field, even if one seems likely.
