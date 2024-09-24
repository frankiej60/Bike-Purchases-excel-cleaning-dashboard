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
To enhance the quality and usability of the data, I carried out the following cleaning operations:

1. Search and replace ambiguous values
    - Resolved ambiguities in the representation of values.
      Example: Replaced 'M' which stood for both 'Male' in the Gender column and 'Married' in the Marital Status column with clear and distinct identifiers.
   
2. Conditional column creation
    - Implemented conditional column creation using the formula:
          =IF(L2>54,"Old", IF(L2>31,"Middleage",IF(L2 < 31, "Adolescent", "Invalid")))
    - This formula was used to categorize each individuals age into specific age ranges: "Old", "Middle Age", "Adolescent", or "Invalid".
    - Purpose: To streamline age-related analysis in pivot tables.

### Outcome of EDA
---
1.	Gender and Purchases 	
- Males have a higher average income of 58,908 compared to females with 52,901.
- Consequently, males purchase more bikes than females.
  
2.	Commute Distance and Bike Purchases
- Employees living closer to work tend to own more bikes (102).
- Those living farther away (more than 10 miles) are less likely to purchase bikes (20).

3.	Marital Status and Bike Purchases
- Singles purchased 250 bikes, which is more than married couples who purchased 231 bikes.

4.	Occupation, Income and Bike Purchases
- Management workers, with an average income of 87,945, purchase most bikes, followed by professional workers, who have an average income of 75,267. Manual workers, with an average income of 19,091 purchased the fewest bikes.

5.	Education and Bike Purchases
- Bachelor’s degree holder purchased the most bikes, totaling 306. Partial college holders followed with 265 bikes, and high school holders purchased 179 bikes, slightly more than graduate degree holders who purchased 174. Partial high school holders purchased the fewest bikes, with a total of 76.

6.	Region and Bike Purchases
- In North America, 53% purchased bikes, while in Europe, the purchase rate is 27%. The Pacific region has the lowest bike purchase rate at 21%.

7.	Occupation and Bike Purchases
- Professional workers purchased the most bikes, totaling 276. Skilled manual workers followed with 255 bikes. Clerical workers bought 177 bikes, and management workers purchased
  173 bikes. Manual workers purchased the fewest bikes, with a total of 119.

8.	Age Bracket and Bike Purchases
- Middle-aged workers purchase the most bikes at 68%, followed by Old workers with a  purchase rate of 19%. Adolescent workers purchased 5% and invalid purchased the fewest at 3%.

### Tools
---
- Microsoft office
    - [Download here](https://www.microsoft.com/en-us/microsoft-365/microsoft-office)

