## Gender Pay Equality Analysis
###  Project Overview
This project focuses on analyzing **gender pay equality** at **Daikibo Manufacturing Company**.  
Using Tableau calculated fields, I developed an **Equality Scoring Model** to classify compensation fairness into categories:
- **Fair**
- **Unfair**
- **Highly Discriminative**
The analysis revealed large discrepancies across employee groups, with notable gender-based pay gaps.
---
###  The Problem
- HR reported an **increasing number of internal complaints** regarding salary inequality.  
- The **"Unfair" equality class** accounted for the highest proportion of compensation (**47.3%**).  
- Significant concerns were raised about **bias in employee compensation** and lack of transparency.
---
### Insights
- Large discrepancies in pay distribution across employee groups.  
- Nearly half of compensation fell into the **Unfair category**, indicating systemic inequality.  
- Gender inequality was most prevalent in mid-level and senior roles.  
---
### Recommendations
- Conduct **regular equal pay audits** to ensure fairness.
- Implement **mandatory gender wage reporting** for transparency.  
- Establish **comprehensive pay transparency policies** to promote accountability.  
- Use the **Equality Scoring Model** for continuous monitoring.  
---
### Skills Used
- **SQL** – Extracted and prepared employee compensation data  
- **Tableau** – Built dashboards and scoring models with calculated fields  
- **Data Analysis** – Classified employee salaries into fairness categories  
- **Data Visualization** – Highlighted inequality trends across groups  
- **Data Storytelling** – Delivered actionable insights to HR for policy improvement  
---
### Equality Scoring Model (Calculated Field)
The Tableau **calculated field** used for classification:  

```sql
IF [Equality Score] <= 10 AND [Equality Score] >= -10 THEN "Fair"
ELSEIF ([Equality Score] < -10 AND [Equality Score] >= -20)
   OR ([Equality Score] <= 20 AND [Equality Score] > 10) THEN "Unfair"
ELSEIF ([Equality Score] <= 100 AND [Equality Score] > 20)
   OR ([Equality Score] < -20 AND [Equality Score] >= -100) THEN "Highly Discriminative"
END
```
---
###

## Proportion of Equality Class Preview

![Proportion of Equality Class](./Proportion%20Of%20Equality%20Class.PNG)

### Key Takeaway
- The analysis revealed that 47.3% of compensation fell into the “Unfair” category, with mid- to senior-level roles showing the widest gender pay gaps.
Daikibo Manufacturing must prioritize equal pay audits, enforce transparency policies, and adopt continuous monitoring to build fairness and employee trust.

 **Potential Impact Projection**
- Reducing the “Unfair” segment by 20% could restore equity for hundreds of employees and improve retention.
- Implementing transparency and audits can help decrease HR complaints by 30–40% annually.

---
