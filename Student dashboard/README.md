 # 📊 Student Performance Analytics Dashboard
![Dashboard](https://github.com/Hariharan-T27/academic-performance-dashboard/blob/main/Student%20dashboard/Output%20Images/Dashboard.png)

A **Streamlit-powered analytics dashboard** designed to help educational institutions monitor and improve student outcomes.  
The dashboard provides **early warnings for at-risk students**, analyzes correlations between academic performance and attendance, and supports data-driven academic interventions.

---

## 🚀 Problem Statement

Educational institutions often struggle to identify students who may fail or drop out until it’s too late.  
By analyzing key performance metrics like **marks, attendance, and platform logins**, this dashboard provides **real-time insights** into student performance and risk levels.

---

## 🎯 Objectives

- Identify students at risk of failing or dropping out.  
- Provide **visual analytics** for decision-making.  
- Enable faculty to monitor performance trends.  
- Allow **new student admissions, record updates, and deletions** in real-time.  
- Export updated datasets in **CSV** and **Excel** formats.

---

## 📂 Dataset

The dashboard uses a CSV dataset with the following columns:

- `StudentID` (Auto-generated if missing)  
- `Name`  
- `Marks`  
- `Attendance` (%)  
- `Logins`  
- `Risk` (calculated field: High, Medium, Low)

---
 
## ✨ Features

### 🔹 Dashboard Sections
- **Overview**
  - Displays average marks, attendance, logins, and total students.
  - Add new students with a live preview and risk classification.
  - Export updated datasets in CSV and Excel (with conditional formatting).
  
- **Correlation Analysis**
  - **Heatmap** of correlation between Marks, Attendance, and Logins.
  - **Scatterplot** of Attendance vs Marks.
  - **Absentee Impact Analysis** (Average Marks by Attendance Group).

- **Student Insights**
  - Search students by ID or Name.  
  - Categorize students into:
    - **Top Performing** (>90 Marks)  
    - **Average Performing** (40–90 Marks)  
    - **Struggling** (<40 Marks)  
  - Risk categorization with bar chart distribution.  
  - **Delete student records** with secure confirmation workflow.

---

## 🎨 Theming

Custom theme configured in `config.toml`:

```toml
[theme]
primaryColor = "#16A34A"
backgroundColor = "#F9FAF9"
secondaryBackgroundColor = "#E9F5EE"
textColor = "#1A1A1A"
font = "Sans Serif"
```

## 🛠️ Tech Stack
**Python**: : 3.8 or later  

- **Frontend & Framework:** Streamlit

- **Data Handling:** Pandas

- **Visualization:** Seaborn, Matplotlib

- **Excel Styling:** OpenPyXL

- **UI Enhancements:** streamlit-option-menu


## ⚙️Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Hariharan-T27/academic-performance-dashboard.git
cd student_dashboard

```
    
### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment:
- Windows: 
```bash
.venv\Scripts\activate
```

- Mac/Linux:
```bash
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Dashboard

```bash
streamlit run dashboard.py
```
The app will open in your browser at http://localhost:8501.

## requirements.txt
```bash
streamlit
pandas
seaborn
matplotlib
streamlit-option-menu
openpyxl
```

## Output Images
#### Dashboard Overview
![Dashboard Overview](https://github.com/Hariharan-T27/academic-performance-dashboard/blob/main/Student%20dashboard/Output%20Images/Dashboard%20Overview.png)

#### Correlation Analysis
![Correlation Analysis](https://github.com/Hariharan-T27/academic-performance-dashboard/blob/main/Student%20dashboard/Output%20Images/Correlation%20Analysis.png)

#### Student Insights
![Student Insights](https://github.com/Hariharan-T27/academic-performance-dashboard/blob/main/Student%20dashboard/Output%20Images/Student%20Insights.png)

#### Average and At-Risk Students
![Average and At-Risk Students](https://github.com/Hariharan-T27/academic-performance-dashboard/blob/main/Student%20dashboard/Output%20Images/Student%20Insights%201.png)

#### Risk Categorization
![Risk Categorization](https://github.com/Hariharan-T27/academic-performance-dashboard/blob/main/Student%20dashboard/Output%20Images/Risk%20Categorization.png)



## 📤 Data Export Features

**CSV Export:** Download the updated dataset as a CSV file.

**Excel Export:**

- Includes Summary Sheet with metrics and risk distribution.

- Conditional color-coding for High Risk, Medium Risk, and Low Risk students.

- Auto-adjusted column widths for readability.


## 🔐 Deletion Workflow

- Faculty must search for a student and explicitly confirm the StudentID before deletion.

- A success popup appears after deletion and auto-closes in 5 seconds.

- Prevents accidental data loss.


## 📌 Future Enhancements

- Integration with real-time LMS (Learning Management System) data.

- Predictive analytics using machine learning models.

- Role-based authentication for faculty and administrators.

- Email/SMS alerts for at-risk students.


## 🤝 Contributing
Contributions are welcome!

- Fork the repository

- Create a new branch

- Submit a pull request with your improvements


## 📜 License
This project is licensed under the **MIT License** – you are free to use, modify, and distribute it with attribution.


## 👨‍💻 Author
Developed by Hariharan Thirunagari

**📧 Contact:** thariharan@gmail.com 

**🔗 LinkedIn:** https://www.linkedin.com/in/hariharanthirunagari/

