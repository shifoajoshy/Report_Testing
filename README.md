# **README**

### <ins>**Skills Utilized**<ins>

• SQL.
• Testing.

**Dashboard Used in Testing**

**Why Testing Required?**
If some values are found incorrect in the Power BI dashboard despite the data being clean, several possibilities could have led to this issue. Here are some potential reasons:

**Data Transformation Errors:**
Mistakes during data preprocessing could lead to inaccurate values due to flawed transformation logic.

**Calculation Errors:**
Errors in DAX calculations or measures may result in incorrect summary values being displayed.

**Filtering or Slicing Problems:**
Incorrectly applied filters or slicers could show only a subset of data, leading to misleading conclusions.

**Cross-Filtering and Relationships:**
Incorrectly defined relationships between tables or misconfigured cross-filtering can cause unexpected results.

**Objective:**
• The objective of this project is to validate the functionality, performance, and security aspects of the Power BI dashboard connected to a PostgreSQL database.
• The testing in this project aims to ensure data accuracy, delivers accurate insights, dashboard meets user requirements, proper functioning of dashboard features, and adherence to security protocols.

**Test Design & Types of Testing Involved:**

**Data Validation Testing:**
SQL queries are executed to validate data consistency and accuracy across the PostgreSQL tables and the dashboard.

**Functionality Testing:**
• Test cases are designed to verify the functionality of filters, KPI indicators, occupancy, realisation percentage, and chart interactions.
• DAX formulas are validated to ensure correct calculation.

**Performance Testing:**
• Performance metrics are defined to measure dashboard response time during filter interactions, data refresh, and loading.
• Tools like DAX Studio and Bravo are utilized to optimize DAX queries and enhance dashboard performance.

**Integration Testing:**
• Scheduled refresh functionality is tested to ensure data is updated according to the defined schedule.
• Data gateway setup and connectivity are verified to ensure seamless data transfer between Power BI and PostgreSQL.

**Non-Functional Requirement (NFR) Testing:**
• Row-level and page-level security measures are tested to confirm that users have appropriate access to data based on security roles.

[Test Design.docx.xlsx](https://github.com/shifoajoshy/Report_Testing/files/14885971/Test.Design.docx.xlsx)

**Outcome:**

**Incorrect Revenue Display in Donut Chart:**
The revenue figure in the Donut Chart is inaccurately presented, possibly due to data aggregation or visualization settings.

**Identification of 8 Non-Relevant Columns:**
Eight columns found in the dashboard are deemed non-relevant or unnecessary, impacting data clarity and analysis.

**Violation of Best Practice Analyzer Rules:**
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
