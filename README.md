### workforce-retention-turnover-insights-pbi

# Workforce Retention & Turnover Insights

### **Project Background**

This project simulates a **People Analytics / HR decision-support use case** using a synthetic workforce dataset of **2,000 employees**. The objective was to move beyond reporting headcount and build a diagnostic view of **retention, turnover, workforce composition, compensation, and employee movement**.

The dashboard identifies an overall **89.80% Retention Rate**, **10.20% Turnover Rate**, **556 New Hires**, and **204 Separations**, while allowing HR teams to drill into the organizational and demographic segments behind these numbers.

Rather than treating the overall retention rate as the final answer, the analysis is designed to help answer a more practical question:

**Where should HR investigate first, and what workforce factors should be examined alongside employee exits?**

**Insights and decision-support areas include:**

- **Retention & Turnover:** Monitoring workforce stability and identifying changes in employee movement over time.
- **Workforce Composition:** Understanding the distribution of employees across age, gender, ethnicity, location, department, and business unit.
- **Compensation & Job Level:** Examining how salary ranges change across organizational levels and how compensation patterns relate to retention.
- **Retention Diagnostics:** Using organizational filters to isolate segments that may require deeper investigation.
- **Workforce Planning:** Using hiring, separation, and active employee trends to understand workforce movement and potential staffing pressure.

### **Dashboard Preview**

<p align="center">
  <img src="https://github.com/afrinanegaban/workforce-retention-powerbi/blob/main/Image/Overview.png?raw=true" width="48%" alt="Overview Dashboard" />
  <img src="https://github.com/afrinanegaban/workforce-retention-powerbi/blob/main/Image/Retention%20Rate.png?raw=true" width="48%" alt="Retention Rate Dashboard" />
</p>

---

## **Data Structure & Model**

The project uses a synthetic employee workforce dataset designed to simulate a realistic People Analytics environment.

The model brings together employee attributes, organizational dimensions, compensation, employment status, and workforce movement to support interactive retention analysis.

- **Employee Workforce Data:** Includes employee demographics, department, business unit, country, job level, salary, and employment status.
- **Workforce Movement:** Tracks active employees, employees who have left, new hires, and separations across the analysis period.
- **Organizational Dimensions:** Enables analysis across department, business unit, country, job level, gender, ethnicity, and age.
- **Compensation Analysis:** Compares salary distributions across job levels and organizational segments.
- **Retention Measures:** Calculates workforce retention and turnover metrics for executive-level monitoring and deeper segmentation.
- **Interactive Filtering:** Slicers allow HR stakeholders to move from a company-wide view to specific organizational and demographic segments.

> **Note:** The dataset is synthetic and is used to demonstrate the analytical framework, dashboard design, and decision-support approach rather than report findings from a real organization.

![Data Model / ERD](https://github.com/afrinanegaban/workforce-retention-powerbi/blob/main/Image/ERD.png
)

---

## **Executive Summary**

### **Overview of Findings**

The simulated workforce has an **89.80% overall retention rate**, meaning the majority of employees remain within the workforce during the analyzed period. At the same time, the **10.20% turnover rate** and **204 separations** create a meaningful workforce movement signal that warrants segmentation rather than being evaluated only at the aggregate level.

The workforce consists of **1,796 active employees and 204 employees who have left**, while **556 new hires** indicate substantial workforce inflow during the analysis period.

The demographic profile is relatively balanced by gender, while the workforce is concentrated in the **40–49 age group (36.6%)**, followed by **30–39 (25.7%)**. Geographically, the **US represents 65.6%** of the workforce, making geographic concentration an important consideration when interpreting workforce patterns.

Compensation increases substantially with job level, ranging from approximately **$46.1K at Level 1** to **$237.9K at Level 7** for the displayed salary measure. At the department level, the salary-retention view also shows differences between departments, suggesting that compensation can be examined as one factor within a broader retention diagnostic rather than as a standalone explanation.

The dashboard therefore functions less as a static HR report and more as a **diagnostic layer for identifying where deeper workforce investigation should happen**.

---

## **Insights Deep Dive**

### **Category 1: Workforce Composition & Demographic Exposure**

The first step in understanding retention is knowing what the workforce actually looks like.

- **Age Concentration:** Employees aged **40–49 account for 36.6%** of the workforce, making this the largest age segment. The **30–39 group represents 25.7%**, while employees aged 50–59 represent 21.5%.
- **Gender Balance:** The workforce is broadly balanced, with **51.80% vs. 48.20%** across the two displayed gender segments.
- **Geographic Concentration:** The **US represents 65.6%** of the workforce, followed by China at 8.55%, Germany at 8.5%, the UK at approximately 6.6%, and India at 5.9%.
- **Ethnicity Mix:** Asian employees represent approximately **37.6%** of the workforce, followed by Caucasian employees at **28.05%**, with additional representation across Hispanic and Black employee segments.

From a People Analytics perspective, these distributions matter because an aggregate retention number can hide concentration risk. A change in retention within a large employee segment can have a much greater workforce impact than the same percentage change in a small segment.

**Decision-support use:** HR can apply the demographic and organizational slicers to determine whether retention or separation patterns are concentrated within particular workforce segments before designing targeted interventions.

![Category 1 - Workforce Composition & Demographics](https://github.com/afrinanegaban/workforce-retention-powerbi/blob/main/Image/Demographic%20Breakdown.png)

---

### **Category 2: Retention, Turnover & Workforce Movement**

The dashboard establishes the overall workforce stability baseline before moving into segment-level diagnosis.

- **Retention Rate:** The overall retention rate is **89.80%**.
- **Turnover Rate:** The corresponding turnover rate is **10.20%**.
- **Employee Separations:** The workforce records **204 separations**.
- **New Hires:** **556 new hires** indicate significant workforce inflow during the analyzed period.
- **Retention Over Time:** The time-series view shows meaningful variation in retention across years, including a pronounced peak around **2018**, followed by lower retention levels in subsequent years.
- **Separation Trend:** Separations fluctuate over time and increase toward the later part of the displayed period, making the time dimension important for identifying periods that deserve further investigation.

The key analytical point is that **89.80% retention should not be interpreted as the end of the analysis**. HR would need to determine whether the 204 exits are concentrated within particular departments, job levels, locations, or employee segments.

**Decision-support use:** When retention declines during a specific period, HR can move from the trend view into the organizational slicers to isolate the segments contributing to the change.


---

### **Category 3: Compensation, Job Level & Retention**

Compensation analysis provides another dimension for understanding workforce stability.

- **Progressive Salary Structure:** Displayed salary levels increase consistently from approximately **$46.1K at Level 1** to **$237.9K at Level 7**.
- **Senior-Level Compensation:** The difference between junior and senior job levels becomes substantially larger at higher organizational levels, reflecting a structured compensation hierarchy.
- **Department-Level Variation:** The salary-retention analysis shows departments occupying different positions across average salary and retention.
- **Observed Association:** The department-level points show a generally positive relationship between average salary and retention in this synthetic dataset. However, this should be treated as an **association rather than evidence that higher salary causes higher retention**.
- **HR Diagnostic:** Compensation therefore works best as one diagnostic variable alongside department, job level, workforce composition, and separation trends.

For a real HR team, the next step would not simply be to increase compensation. The analysis would instead identify segments with relatively lower retention and then investigate whether compensation, role progression, workload, management, location, or other employee-experience factors could explain the difference.

**Decision-support use:** Use the **Job Level / Department / Business Unit** tabs above the salary analysis to shift from an organization-wide compensation view to a specific workforce segment.

![Category 3 - Salary Distribution & Retention Relationship](https://github.com/afrinanegaban/workforce-retention-powerbi/blob/main/Image/Salary%20Distribution%20.png)

---

### **Category 4: Retention Trend & Root-Cause Investigation**

The retention trend becomes more useful when treated as an early-warning mechanism rather than simply a historical chart.

The dashboard shows that retention does not remain constant throughout the analyzed period. The movement from higher retention levels toward approximately **89% in the later period** creates an opportunity for HR to investigate what changed.

A practical diagnostic workflow would be:

1. **Identify the period:** Detect when retention begins to decline.
2. **Segment the workforce:** Filter by department, business unit, country, gender, or ethnicity.
3. **Compare job levels:** Determine whether exits are concentrated among junior, mid-level, or senior employees.
4. **Examine compensation:** Compare salary patterns within the affected segment.
5. **Review separations:** Identify whether the increase is isolated to specific organizational groups.
6. **Validate with employee-level data:** Investigate tenure, performance, manager, workload, engagement, or exit-reason data if available.

This turns the dashboard from a reporting tool into a **root-cause investigation framework**.

![Category 4 - Retention Trend & Root-Cause Investigation](https://github.com/afrinanegaban/workforce-retention-powerbi/blob/main/Image/Retention%20Trend.png)

---

## **Recommendations**

Based on the dashboard analysis, the following actions would form a practical People Analytics workflow:

1. **Move Beyond the Overall Retention Rate:**  
   Use the **89.80% retention rate** as the baseline, but prioritize segment-level analysis to determine where the remaining **10.20% turnover** is concentrated.

2. **Investigate the Later-Period Retention Decline:**  
   The retention trend shows weaker performance after the stronger levels observed around 2018. HR should identify which departments, business units, job levels, or demographic segments contributed to the change.

3. **Prioritize Separation Diagnostics:**  
   With **204 employees recorded as having left**, analyze separation concentration by organizational segment before designing retention initiatives. This helps distinguish broad workforce movement from localized retention problems.

4. **Use Compensation as a Diagnostic, Not a Conclusion:**  
   Salary should be compared with retention, job level, and department to identify potential compensation-related patterns. Any intervention should be supported by additional employee-experience evidence rather than assuming compensation is the sole driver.

5. **Build Segment-Level Retention Monitoring:**  
   HR teams can use the dashboard's slicers to monitor retention across departments, business units, countries, gender, and ethnicity. This creates a repeatable framework for identifying emerging workforce risks.

6. **Connect Analytics to Root-Cause Research:**  
   Once a high-risk segment is identified, combine the dashboard findings with employee surveys, exit interviews, tenure data, performance data, manager-level information, and exit reasons to move from **"where are employees leaving?"** to **"why are they leaving?"**

---

## **Business Value**

The core value of this dashboard is not simply presenting HR KPIs. It creates a structured path from **workforce monitoring → segmentation → anomaly detection → root-cause investigation → potential HR intervention**.

For an HR or People Analytics team, the dashboard can support:

- Workforce stability monitoring
- Retention-risk identification
- Department and business-unit diagnostics
- Compensation benchmarking
- Workforce planning
- Separation analysis
- Management reporting
- Data-driven HR investigation

Because the underlying dataset is synthetic, the project demonstrates the **analytical approach, KPI design, data modeling, and decision-support workflow** rather than claiming real organizational outcomes.

---

[🔗Dashboard](https://github.com/afrinanegaban/workforce-retention-powerbi/blob/main/Workforce%20Retention%20%26%20Turnover%20Insights.pbit)
