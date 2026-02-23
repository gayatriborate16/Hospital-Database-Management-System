# Hospital-Database-Management-System
Designed a real-world Hospital Management Database using MySQL with advanced SQL queries for patient treatment tracking, staff management, and operational insights.

📌 Project Overview

The Hospital Database Management System is a relational SQL project designed to manage hospital operations including patient records, physician assignments, nurse scheduling, appointments, procedures, prescriptions, and room allocation.

This project demonstrates advanced SQL concepts such as:
Complex JOIN operations
Aggregations & grouping
CTE (Common Table Expressions)
Date comparisons
Relational database modeling
Real-world healthcare analytics
The database simulates real hospital workflows and enables analytical querying for operational insights.

🏙 Problem Statement

Hospitals handle multiple interconnected datasets such as patients, physicians, rooms, treatments, and schedules. Without a structured database, managing healthcare operations becomes inefficient.

This project aims to:
Design a normalized relational database
Manage patient treatment workflows
Track physician certifications and procedures
Monitor appointment scheduling
Analyze room availability and staff allocation
The system helps healthcare administrators make data-driven decisions through structured SQL analysis.

📊 Dataset Information

The database contains multiple interconnected entities representing hospital operations:
👨‍⚕️ Staff Tables
physician – Doctors and their roles
nurse – Nurse information and certification status
department – Medical departments
affiliated_with – Physician-department relationships
trained_in – Physician procedure certifications
on_call – Nurse scheduling

🧑‍🦽 Patient & Treatment Tables
patient – Patient demographic details
appointment – Consultation scheduling
stay – Hospital admissions
undergoes – Procedures performed
prescribes – Medication records

🏥 Infrastructure Tables
block – Hospital block structure
room – Room availability

💊 Medical Data Tables
medication
procedures
🧾 Feature Classification

🔹 Operational Features
Appointment scheduling
Room management
Staff allocation

🔹 Clinical Features
Procedure tracking
Certification validation
Medication prescriptions

🔹 Analytical Features
Patient-physician relationships
Nurse assistance tracking
Resource utilization analysis

🚨 Key Insights (From SQL Analysis)

Based on the analytical queries implemented:
Some physicians are affiliated with departments but not marked as primary.
Patients consult multiple physicians through appointments.
Examination Room C has multiple unique patient visits.
Certain appointments do not require nurse assistance.
Room availability varies across floors and blocks.
Advanced analysis identified physicians performing procedures after certification expiration — a critical compliance insight.

🏆 Advanced Analysis

This project goes beyond basic SQL by implementing:

🔎 Multi-table Joins
Linking patients, physicians, nurses, and medications for treatment history.

📈 Aggregation Analytics
Count of unique patients per examination room
Number of physicians per patient
Room availability per floor/block

⚠️ Compliance Monitoring
Using date comparisons to detect physicians performing procedures after certification expiry.

🧠 Resource Optimization
Identifying floors with minimum room availability to support hospital capacity planning.

🛠 Tools & Technologies Used
MySQL
SQL Joins (INNER, LEFT JOIN)
Aggregations & GROUP BY
CTE (WITH Clause)
Date Handling (STR_TO_DATE)
Relational Database Design
Primary & Foreign Key Constraints

🎯 Recommendations

Based on database analysis:
Replace VARCHAR dates with DATE datatype for better performance.

Add indexes on:
patient
physician
appointmentid
Implement triggers to automatically update room availability.
Create dashboards using Power BI/Tableau for visualization.
Add appointment time fields to improve scheduling analytics.

🌱 Conclusion

The Hospital Database Management System demonstrates how relational databases can model complex healthcare workflows. Through structured schema design and advanced SQL queries, this project showcases real-world data management, compliance tracking, and operational analytics.

It highlights practical applications of SQL in healthcare systems and serves as a strong example of data analyst and database design capabilities.
