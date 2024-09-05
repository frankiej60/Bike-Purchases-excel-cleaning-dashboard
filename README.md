### Excel-cleaning-dashboard

---
### Data source 
---
The primary data used for the preprocessig is the excelprojects.xlsx file, containing detailed information about customers. The dataset includes various demographic and personal details of the customers. Find an outline of the methodologies employed in this project below.

### Dataset overview
---
The raw CSV data was based on multiple attributes including:
    - Marital status
    - Gender
    - Income
    - Children
    - Education
    - Occupation
    - Car count
    - Commute distance
    - Region
    - Age

### Methodology
---
To enhance the quality and usability of the data, I undertook the following cleaning operations:

1. Search and Replace Ambiguous Values
    - Resolved ambiguities in the representation of values.
      Example: Replaced 'M' which stood for both 'Male' in the Gender column and 'Married' in the Marital Status column with clear and distinct identifiers.
   
2. Conditional Column Creation
    - Implemented conditional column creation using the formula:
        =IF(L2>55, "Old", IF(L2>=31, "Middle Age", IF(L2<31, "Adolescent", "Invalid")))
    - This formula was used to categorize each individuals age into specific age ranges: "Old", "Middle Age", "Adolescent", or "Invalid".
    - Purpose: To streamline age-related analysis in pivot tables.


### Tools
---
- Microsoft office software
    - [Download here](https://www.microsoft.com/en-us/microsoft-365/microsoft-office)

