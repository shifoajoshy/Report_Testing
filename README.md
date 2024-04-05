# **README**

### <ins>**Skills Utilized**

• SQL.<br>
• Testing.

### <ins>**Dashboard Used in Testing**<ins>:<br>
<br>pbix format: https://github.com/shifoajoshy/Report_Testing/blob/main/Dashboard%20%26%20Data%20%20Source/Hospitality_Taj_Hotels.pbix <br> 
<br>PDF format: [Hospitality_Taj_Hotels.pdf](https://github.com/shifoajoshy/Report_Testing/files/14887583/Hospitality_Taj_Hotels.pdf)

### <ins>**Why Testing Required?**<ins><br>

If some values are found incorrect in the Power BI dashboard despite the data being clean, several possibilities could have led to this issue. Here are some potential reasons:

   <ins>**Data Transformation Errors:**<ins><br>

  • Mistakes during data preprocessing could lead to inaccurate values due to flawed transformation logic.

  <ins>**Calculation Errors:**<ins><br>

  • Errors in DAX calculations or measures may result in incorrect summary values being displayed.

  <ins>**Filtering or Slicing Problems:**<ins><br>

  • Incorrectly applied filters or slicers could show only a subset of data, leading to misleading conclusions.

  <ins><br>**Cross-Filtering and Relationships:**<ins><br>

  • Incorrectly defined relationships between tables or misconfigured cross-filtering can cause unexpected results.

### <ins><br>**Objective:**<ins><br>
• The objective of this project is to validate the functionality, performance, and security aspects of the Power BI dashboard connected to a PostgreSQL database.
• The testing in this project aims to ensure data accuracy, delivers accurate insights, dashboard meets user requirements, proper functioning of dashboard features, and adherence to security protocols.

### <ins>**Test Design overview & Types of Testing Involved:**<ins><br>

<br><br><br><ins>**Data Validation Testing:**<ins><br>

• SQL queries are executed to validate data consistency and accuracy across the PostgreSQL tables and the dashboard.

<ins>**Functionality Testing:**<ins><br>

• Test cases are designed to verify the functionality of filters, KPI indicators, occupancy, realisation percentage, and chart interactions.
• DAX formulas are validated to ensure correct calculation.

<ins>**Performance Testing:**<ins>

• Performance metrics are defined to measure dashboard response time during filter interactions, data refresh, and loading.
• Tools like DAX Studio and Bravo are utilized to optimize DAX queries and enhance dashboard performance.

<ins><br>**Integration Testing:**<ins><br>

• Scheduled refresh functionality is tested to ensure data is updated according to the defined schedule.
• Data gateway setup and connectivity are verified to ensure seamless data transfer between Power BI and PostgreSQL.

<ins>**Non-Functional Requirement (NFR) Testing:**<ins><br>

• Row-level and page-level security measures are tested to confirm that users have appropriate access to data based on security roles.

### <ins>**Test Design report:<ins>** [Test Design.docx.xlsx](https://github.com/shifoajoshy/Report_Testing/files/14885971/Test.Design.docx.xlsx)

### <ins>**Outcome:**<ins>

**Incorrect Revenue Display in Donut Chart:**
The revenue figure in the Donut Chart is inaccurately presented, possibly due to data aggregation or visualization settings.

**Identification of 8 Non-Relevant Columns:**
Eight columns found in the dashboard are deemed non-relevant or unnecessary, impacting data clarity and analysis.

--**Violation of Best Practice Analyzer Rules:**
Upon running the Best Practice Analyzer, it was discovered that 11 rules were violated:
- Fully qualify column references (30 objects).
- Provide format string for visible numeric measures (14 objects).
- Avoid summarizing numeric columns (8 objects).
- Organize columns and hierarchies in display folders (1 object).
- Hide foreign key columns (10 objects).
- Organize measures in display folders (1 object).
- Avoid CamelCase on visible measures and tables (1 object).
- Ensure column names in relationships are identical (8 objects).
- Ensure column and hierarchy names start with an uppercase letter (28 objects).
- Ensure measure and table names start with an uppercase letter (6 objects).
- Disable auto date/time (1 object).
