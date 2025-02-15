# EmployeeDataSet
## ER Diagram 
![img](https://github.com/CalvinK2025/EmployeeDataSet/blob/main/EmployeeDataSet.drawio.png)

## Employee Table
Here's your data in Markdown format:  

```md
## Employee Table

```sql
SELECT * FROM Employee;
```

| EmployeeId | FirstName | LastName | Email                   | PhoneNumber   | HireDate   | JobTitle           | Department  | Salary | ManagerID |
|------------|----------|----------|-------------------------|--------------|------------|--------------------|-------------|--------|-----------|
| 1          | John     | Doe      | john.doe@example.com    | 123-456-7890 | 2024-01-15 | Software Engineer  | Technology  | 60000  | NaN       |
| 2          | Jane     | Smith    | jane.smith@example.com  | 987-654-3210 | 2023-05-20 | Data Scientist     | Analytics   | 75000  | 1.0       |
| 3          | Bob      | Johnson  | bob.johnson@example.com | 555-123-4567 | 2022-11-10 | Project Manager    | Management  | 80000  | 1.0       |

---

## Tasks Table

```sql
SELECT * FROM Tasks;
```

| TaskID | TaskType          | TaskName                    | Description                          | DifficultyLevel | TimeToComplete | AutoPotential | AssignedEmployeeID |
|--------|------------------|----------------------------|-------------------------------------|----------------|---------------|---------------|------------------|
| 1      | Creative         | Design Website Mockup      | Create initial website wireframes  | 3              | 120           | 2             | 2                |
| 2      | Procedural       | Data Cleaning             | Cleanse and prepare customer data  | 2              | 60            | 4             | 2                |
| 3      | Decision-Making  | Project Prioritization    | Prioritize upcoming projects       | 4              | 30            | 1             | 3                |
| 4      | Creative         | Develop Marketing Campaign | Plan a marketing campaign          | 5              | 240           | 1             | 1                |
| 5      | Procedural       | Code Review               | Review code for bugs and efficiency | 2              | 90            | 3             | 1                |
```

This Markdown will render the SQL queries and tables properly in GitHub or any Markdown-supported platform. Let me know if you need any changes! 🚀
