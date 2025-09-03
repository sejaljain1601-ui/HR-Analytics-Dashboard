# HR Analytics Project (Power BI)

## Project Overview
This Power BI dashboard presents a comprehensive view of HR data, including salary trends, leave patterns, gender distribution, and other key workforce metrics.  
It transforms raw employee data into clear, actionable insights to support strategic HR decisions and improve organizational transparency.

---
## Database Schema
The project uses a single table with the following columns:

**Employee Table**
• `Employee Id`  
• `First Name`  
• `Last Name`  
• `Gender`  
• `Start Date`  
• `Years`  
• `Department`  
• `Country`  
• `Center`  
• `Monthly Salary`  
• `Annual Salary`  
• `Job Rate`  
• `Sick Leaves`  
• `Unpaid Leaves`  
• `Overtime Hours`

**Relationships:**  
• Single flat employee table is used as the data source for all visuals and measures.

---
## Power BI File / Code
• Only a Power BI report file is included: `HR_Analytics.pbix` (contains data model, DAX measures, calculated columns, and dashboards).  

• To view the interactive report, download the `.pbix` file and open it in **Power BI Desktop**. (GitHub will only allow downloading the file; it cannot render `.pbix` in-browser.)

---
## Key Queries / Analysis Points
The analysis was done inside Power BI using **DAX measures** and **calculated column**. Key items created:

- Calculated Columns / Measures:
  - `Full Name` (concatenate `First Name` + `Last Name`)
  - `Male Headcount`, `Female Headcount` (gender counts)  
  - `Avg Monthly Salary`, `Total Employees`, `Total Countries`, `Total Centers`, `Total Departments`  
  - Leave and overtime aggregates (by department / year)  
  - Yearly `Job Rate` and `Employee Count` measures for growth analysis

- Dashboards:
  1. **Overview Dashboard**  
     - Shows overall company metrics: total employees, gender distribution across departments, average monthly salary, total countries and centers, and total departments.
       
  2. **Deep-Dive Dashboard** (4 charts)  
     - **Leaves summary by department** (sick & unpaid leaves)  
     - **Salary distribution by department** (with gender breakdown)  
     - **Yearly overview chart**: Sick Leaves vs Overtime Hours (to examine correlation between overtime and sick leaves)  
     - **Organizational growth metrics** (yearly): job rate vs employee count

---
## Insights & Findings
- **Manufacturing has the highest number of unpaid & sick leaves**  
  (This may indicate employee stress, poor working conditions, or inadequate staffing in Manufacturing — worth investigating root causes like workload or shift patterns.)

- **2019 shows the highest overtime and the highest sick leaves**  
  (Possible indication that increased overtime in 2019 led to burnout and more sick leaves — suggests a correlation where higher overtime precedes higher sick leave.)

- **2019 had the most hires compared to other years**  
  (Rapid hiring could be tied to a growth phase or high attrition, investigate recruitment drivers and retention.)

- **Significant pay gap between male and female employees in Research Centres and Environmental Compliance departments**  
  (Gender pay disparities appear concentrated in specific centers; recommend a pay equity audit and targeted corrective actions in those departments.)

- **Other departments show near-equal average salaries across genders**  
  (Indicates more equitable pay practices in most areas — good to maintain and replicate.)

- **Job Rate trend shows '1' (entry-level) roles are less hired across years compared to other job rates**  
  (Shows fewer freshers/entry-level hires — organization may prefer experienced hires or there may be gaps in early-career recruitment.)

---
## Repository Structure
HR_Analytics/

├── HR_Analytics.pbix # Power BI report (download to view)

└── README.md # Project overview, schema, analysis, insights

---
**AUTHOR**

Sejal Jain – SQL & Data Analysis Enthusiast

• GitHub: https://github.com/sejaljain1601-ui

• LinkedIn: https://www.linkedin.com/in/sejal-jain-lko
