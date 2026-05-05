# Student Academic Performance Analysis 

A SQL project focused on analyzing student academic performance using normalized datasets.  
This project explores how factors like study hours, attendance, internet access, extracurricular activities, and education level impact final exam performance.

---

## Project Overview

The dataset contains student demographic details, academic habits, and performance metrics.

The project is divided into **3 normalized tables**:

### 1. Student Table
Contains basic student information:
- student_id
- gender
- age

### 2. Performance Table
Contains academic-related information:
- student_id
- education_id
- study_hours_per_week
- attendance_rate
- internet_access
- extracurricular
- previous_score
- final_score
- passed

### 3. Education Table
Contains education category details:
- education_id
- student_education

---

## Database Design

This project follows database normalization principles by separating data into multiple related tables.

### Relationships:
- `student_table.student_id` → `performance_table.student_id`
- `education.education_id` → `performance_table.education_id`

This improves:
- Data consistency
- Reduced redundancy
- Better query performance

---

## Tools Used

- MySQL
- SQL Joins
- CTEs
- Window Functions
- Aggregate Functions
- CASE Statements

---

## SQL Concepts Covered

### Basic Queries
- Retrieve all records
- Filter students based on score
- Sort final scores

### Aggregate Functions
- COUNT()
- AVG()
- MAX()

### Joins
Used joins to combine:
- Student details
- Performance details
- Education categories

### CASE Statements
Classified students into:
- High Performers
- Medium Performers
- Low Performers

### Subqueries
Used subqueries to:
- Find students above average score
- Find highest scoring students

### CTEs
Used Common Table Expressions for:
- Average score analysis
- Combined student performance filtering

### Window Functions
- RANK()
- ROW_NUMBER()
- Running Average

---

## Key Business Questions Solved

✔ Retrieve all student records  
✔ Find students who passed/failed  
✔ Students scoring above 70  
✔ Average final score analysis  
✔ Performance by internet access  
✔ Performance by education category  
✔ Rank students by final scores  
✔ Identify top performers  
✔ Running average calculations  

---

## Sample SQL Query


SELECT student_id, final_score
FROM performance_table
WHERE final_score > 70
ORDER BY final_score DESC;


<img width="1046" height="753" alt="Screenshot 2026-05-05 131242" src="https://github.com/user-attachments/assets/0be38b28-7431-476a-a653-08a0ac78567b" />

<img width="1018" height="752" alt="Screenshot 2026-05-05 131306" src="https://github.com/user-attachments/assets/55e599fd-f3a0-44df-9522-fbe8b764c9ad" />

<img width="968" height="737" alt="Screenshot 2026-05-05 132121" src="https://github.com/user-attachments/assets/e49551b5-c6e2-4f58-9caa-75995c2e647b" />

<img width="1007" height="730" alt="Screenshot 2026-05-05 131434" src="https://github.com/user-attachments/assets/fb055e1b-2945-4126-a05c-2c93a8cf619a" />

<img width="1194" height="741" alt="Screenshot 2026-05-05 131454" src="https://github.com/user-attachments/assets/2e663690-b33e-448f-9336-fd6fdca967d1" />

<img width="1094" height="736" alt="Screenshot 2026-05-05 131513" src="https://github.com/user-attachments/assets/e20ab729-1cfb-417e-b74f-5c8b4ef7bc87" />

<img width="1077" height="744" alt="Screenshot 2026-05-05 131531" src="https://github.com/user-attachments/assets/e0da6353-f9af-4fa6-a2fb-c41d82799638" />

<img width="1204" height="747" alt="Screenshot 2026-05-05 131547" src="https://github.com/user-attachments/assets/b8974f65-8d3b-440f-bd5f-d40ad8f8f62c" />

<img width="1052" height="739" alt="Screenshot 2026-05-05 131603" src="https://github.com/user-attachments/assets/5ad16fe0-3056-491d-b195-eeb6ca05cf77" />

### ⚙️ Connect with Me

<p align="center">
<a href="mailto:febijustin4@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/febi~justin/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>


