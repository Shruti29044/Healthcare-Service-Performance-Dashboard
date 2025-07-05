# 🏥 Healthcare Service Performance Dashboard

A dynamic Power BI dashboard project analyzing healthcare service performance across departments, regions, and years. This project uses mock healthcare data to uncover insights into patient volume, service types, and cost distribution, and was developed to simulate real-world reporting for operational decision-making.

---

## 📊 Project Overview

The **Healthcare Service Performance Dashboard** is designed to assist healthcare administrators and analysts in monitoring and evaluating service-related KPIs such as:

- Total service cost
- Patient count trends
- Departmental performance
- Regional cost analysis
- Service type utilization

This project aims to present actionable visual insights that can support performance improvements, cost optimization, and patient service planning.

---

## ✅ Key Features

- 📌 **KPI Metric Card**: Total Service Cost displayed prominently for quick snapshot.
- 📅 **Yearly Service Cost Trend**: Line chart showing cost variation over 2023–2025.
- 🏥 **Department Analysis**:
  - Bar chart: Sum of cost by department
  - Column chart: Count of patient IDs and performance deltas by department
- 🌍 **Regional Cost Breakdown**: Pie chart summarizing cost by geographic region.
- 📈 **Patient Age & Service Type Flow**: Sankey-style visual for tracking age-service distribution.
- 🔍 **Key Influencers Visual**: AI-driven insights into what influences department costs.
- 🧠 **Gauge for Activity Volume**: Total number of department-service interactions.
- 🧾 **Service Type Segmentation**: Donut chart showing breakdown of patient visits by service type (Consultation, Lab Test, Imaging, Surgery).

---

## 🛠 Tools & Technologies Used

- **Power BI Desktop**
- Power Query (ETL)
- DAX (Data Analysis Expressions)
- Excel (for data staging and cleaning)
- Custom Visuals (Donut Chart, KPI Gauge, Influencers)

---

## 🚧 Challenges Faced

### 1. **Data Modeling Conflicts**
- **Issue**: Original data had loosely defined relationships (e.g., duplicate Patient IDs across services, mixed granularity).
- **Solution**: Created normalized tables and used surrogate keys for better star schema structure. Introduced a proper Date table and linked all relevant fact tables to improve time intelligence.

### 2. **Inconsistent or Missing Data**
- **Issue**: Service cost entries were missing or zero for some records, skewing analysis.
- **Solution**: Used conditional logic in Power Query to filter out null or invalid records and imputed missing values where appropriate.

### 3. **Dynamic Visual Interactions**
- **Issue**: Some visuals (like slicers and pie charts) conflicted when interacting across filters.
- **Solution**: Adjusted cross-filter behavior using Power BI’s "Edit Interactions" feature to maintain meaningful user experience.

### 4. **Visual Clarity vs. Complexity**
- **Issue**: Overcrowding the dashboard with charts created clutter and distracted from insights.
- **Solution**: Streamlined the layout by grouping visuals by theme (cost, patient, service type) and applied consistent color schemes for intuitive navigation.

### 5. **Understanding Key Influencers Output**
- **Issue**: The "Key Influencers" visual sometimes produced misleading correlations due to categorical noise.
- **Solution**: Refined columns used for input, excluded low-impact categorical values, and validated the visual’s suggestions with manual DAX calculations.

---

## 💡 Learning Outcomes

- Developed a deeper understanding of **data storytelling** through visual design.
- Improved proficiency in **DAX measures and calculated columns**.
- Gained hands-on experience in **resolving data quality issues** and enhancing model efficiency.
- Practiced aligning technical analytics work with **real-world healthcare operations**.
- Learned to balance **data complexity** with **user-friendly reporting**.

---
---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `Healthcare_Dashboard.pbix` | Power BI file with full dashboard |
| `screenshot.png` | High-resolution preview image |
| `README.md` | Project documentation |
| `mock_data.xlsx` | (Optional) Sample dataset used in the report |

---

## 🤝 Let's Connect!

If you have feedback or want to collaborate on analytics projects, feel free to connect with me or drop a message!

---

