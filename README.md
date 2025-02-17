# EmployeeDataSet
## ER Diagram 
![img](https://github.com/CalvinK2025/EmployeeDataSet/blob/main/EmployeeDataSet.drawio.png)

## Employee Table

```sql
SELECT * FROM Employee;

| EmployeeId | FirstName | LastName  | Email                      | PhoneNumber   | HireDate   | JobTitle            | Department       | Salary | ManagerID |
|------------|----------|-----------|----------------------------|--------------|------------|---------------------|------------------|--------|-----------|
| 1          | John     | Doe       | john.doe@example.com       | 123-456-7890 | 2023-03-15 | Software Engineer   | Technology       | 75000  | NaN       |
| 2          | Jane     | Smith     | jane.smith@example.com     | 234-567-8901 | 2022-07-10 | Data Scientist      | Technology       | 80000  | 1.0       |
| 3          | Michael  | Johnson   | michael.johnson@example.com | 345-678-9012 | 2021-05-22 | Product Manager     | Technology       | 95000  | 2.0       |
| 4          | Emily    | Davis     | emily.davis@example.com    | 456-789-0123 | 2020-11-14 | HR Specialist       | Human Resources  | 60000  | NaN       |
| 5          | David    | Brown     | david.brown@example.com    | 567-890-1234 | 2019-09-05 | UX Designer         | Technology       | 72000  | 1.0       |
| 6          | Sarah    | Wilson    | sarah.wilson@example.com   | 678-901-2345 | 2021-01-30 | Marketing Manager   | Marketing        | 85000  | NaN       |
| 7          | Chris    | Moore     | chris.moore@example.com    | 789-012-3456 | 2022-12-12 | HR Manager          | Human Resources  | 90000  | 4.0       |
| 8          | Olivia   | Taylor    | olivia.taylor@example.com  | 890-123-4567 | 2018-06-07 | Business Analyst    | Finance          | 70000  | NaN       |
| 9          | James    | Anderson  | james.anderson@example.com | 901-234-5678 | 2020-03-19 | Network Engineer    | Technology       | 80000  | 1.0       |
| 10         | Isabella | Thomas    | isabella.thomas@example.com | 012-345-6789 | 2022-08-30 | Content Strategist  | Marketing        | 75000  | 6.0       |

```




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
