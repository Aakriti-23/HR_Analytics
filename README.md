# HR Analytics

> End-to-end HR data analysis — from employee attrition and performance to training effectiveness — backed by an interactive Power BI dashboard.

---

## Overview

This project performs a comprehensive analysis of an HR dataset covering **3,150 employee records** across departments, employment types, performance ratings, and training programs. It combines a **Python-based EDA notebook** with an interactive **Power BI dashboard** to surface actionable workforce insights.

**Questions this project answers:**
- What drives voluntary vs. involuntary employee terminations?
- How do engagement, satisfaction, and work-life balance scores vary across departments?
- Which employee segments (department, pay zone, employment type) show the strongest performance?
- How effective are training programs, and what do they cost?
- How do demographics (gender, race, marital status) relate to attrition and performance?

---

## Repository Structure

```
HR_Analytics/
├── HR_Analytics.ipynb             # Python EDA — cleaning, analysis & visualizations
├── HR_Analytics_Dashboard.pbix    # Power BI interactive dashboard
├── data/
│   └── HR_Dataset_Detailed.csv    # HR dataset (see Dataset section)
└── README.md
```

---

## Dataset

The dataset contains **3,150 records** and **39 columns** covering the full employee lifecycle.

| Category | Columns |
|----------|---------|
| **Employee Info** | Employee ID, First/Last Name, DOB, Gender, Race, Marital Status |
| **Employment Details** | Start Date, Exit Date, Title, Employee Type, Employee Status, Pay Zone |
| **Organisation** | Department, Division, Business Unit, Location, Supervisor |
| **Termination** | Termination Type, Termination Description |
| **Performance & Surveys** | Performance Score, Current Employee Rating, Engagement Score, Satisfaction Score, Work-Life Balance Score |
| **Training** | Training Program Name, Training Type, Training Outcome, Training Duration (Days), Training Cost |

**Employee Status values:** `Active`, `Voluntarily Terminated`, `Terminated for Cause`, `Leave of Absence`, `Future Start`

**Departments covered:** Production, Sales, IT/IS, Software Engineering, Admin Offices, Executive Office

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x | Core analysis language |
| Jupyter Notebook | Interactive analysis environment |
| Pandas | Data manipulation & cleaning |
| Matplotlib / Seaborn | Statistical visualizations |
| Power BI Desktop | Interactive business dashboard |

---

## Getting Started

### Prerequisites

- Python 3.7+
- Jupyter Notebook or JupyterLab
- Power BI Desktop *(for the `.pbix` file — [download here](https://powerbi.microsoft.com/desktop/))*

### Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/Aakriti-23/HR_Analytics.git
   cd HR_Analytics
   ```

2. **Install Python dependencies**

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Launch the notebook**

   ```bash
   jupyter notebook HR_Analytics.ipynb
   ```

4. **Open the Power BI Dashboard**

   Open `HR_Analytics_Dashboard.pbix` in Power BI Desktop.

---

## Analysis Highlights

The notebook covers:

- **Data Cleaning & Preprocessing** — handling missing exit/termination dates, fixing whitespace in department names, parsing date fields
- **Attrition Analysis** — breakdown of voluntary resignations, retirements, and terminations for cause by department and pay zone
- **Performance Analysis** — distribution of performance scores (Fully Meets / Exceeds / Needs Improvement / PIP) across job roles and departments
- **Survey Insights** — engagement, satisfaction, and work-life balance score trends across the organisation
- **Training Effectiveness** — analysing training outcomes, costs, and duration by program type
- **Demographic Breakdown** — attrition and performance segmented by gender, race, and marital status

The Power BI dashboard provides interactive filtering across all these dimensions.

---

## Key Insights

- Termination types span **voluntary resignation, retirement, and involuntary** — each driven by different employee profiles
- **Engagement and satisfaction scores** differ notably across departments, highlighting team-level culture gaps
- **Pay Zone** (A / B / C) correlates with both employee type distribution and attrition patterns
- Training programs vary significantly in **cost and duration**, with outcomes worth tracking against performance scores
- Employees on **PIP (Performance Improvement Plans)** represent a distinct at-risk segment for future attrition

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Author

**Aakriti** · [GitHub](https://github.com/Aakriti-23)
