# EmployeeDataSet

## How to Use
1. Download raw file. https://github.com/CalvinK2025/EmployeeDataSet/blob/main/Employee_Data_Set.ipynb
2. https://colab.research.google.com/ > Upload.
3. Run the first code cell on the colab to see all the data rendered. 
4. Add your SQL query with a new code cell to practice interesting and complicated questions.

## ER Diagram 
![img](https://github.com/CalvinK2025/EmployeeDataSet/blob/main/EmployeeDataSet.drawio.png)

## Employee Table
```sql
SELECT * FROM Employee;
```
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

## Tasks Table
```sql
SELECT * FROM Tasks;
```
| TaskID | TaskType         | TaskName                    | Description                                      | DifficultyLevel | TimeToComplete | AutoPotential | AssignedEmployeeID |
|--------|-----------------|----------------------------|-------------------------------------------------|----------------|---------------|--------------|------------------|
| 1      | Creative        | Design New Feature        | Design and prototype a new feature for the product. | 3              | 180           | 2            | 1                |
| 2      | Procedural      | Data Cleaning             | Clean and preprocess raw data for analysis.     | 2              | 120           | 3            | 2                |
| 3      | Decision-Making | Product Strategy Meeting  | Attend a meeting to define the roadmap.        | 4              | 90            | 1            | 3                |
| 4      | Procedural      | Employee Onboarding      | Assist in onboarding new employees.            | 2              | 150           | 3            | 4                |
| 5      | Creative        | Develop New Software     | Write and develop software for clients.        | 5              | 240           | 1            | 1                |
| 6      | Creative        | Design User Interface    | Design UI for a new application.               | 4              | 200           | 2            | 5                |
| 7      | Procedural      | System Maintenance       | Perform routine maintenance on software.       | 3              | 180           | 4            | 9                |
| 8      | Creative        | Content Strategy         | Develop content strategy for marketing.        | 3              | 150           | 2            | 6                |
| 9      | Decision-Making | HR Policy Review        | Review and update HR policies.                 | 4              | 120           | 1            | 4                |
| 10     | Procedural      | Analyze Business Metrics | Analyze and report on key business metrics.    | 3              | 180           | 3            | 2                |
| 11     | Procedural      | Network Troubleshooting | Troubleshoot and resolve network issues.       | 3              | 120           | 3            | 9                |
| 12     | Creative        | Design Sales Materials   | Create and design sales materials.             | 3              | 150           | 2            | 6                |
| 13     | Decision-Making | Budget Allocation       | Participate in budget allocation decisions.    | 5              | 90            | 1            | 8                |
| 14     | Creative        | Develop Marketing Campaign | Create a new marketing campaign.               | 4              | 200           | 2            | 6                |
| 15     | Procedural      | Write Technical Documentation | Document software features and usage.  | 3              | 180           | 3            | 1                |

## Messages Table
```sql
SELECT * FROM Messages;
```
| MessageID | SenderID | ReceiverID | MessageText                                      | SentDateTime          |
|-----------|----------|------------|-------------------------------------------------|-----------------------|
| 1         | 1        | 2          | Hey Jane, can you help me with the data analysis? | 2025-02-16 10:00:00   |
| 2         | 2        | 1          | Sure, I can assist with that. Let me know the details. | 2025-02-16 10:05:00   |
| 3         | 3        | 4          | Emily, we need to discuss the project roadmap soon. | 2025-02-16 11:00:00   |
| 4         | 4        | 3          | Got it, Michael. Let's schedule a meeting for next week. | 2025-02-16 11:10:00   |
| 5         | 5        | 6          | Sarah, do you have the design specs for the new project? | 2025-02-16 12:00:00   |
| 6         | 6        | 5          | Yes, I'll send them over by the end of the day. | 2025-02-16 12:05:00   |
| 7         | 7        | 8          | Olivia, can you review the marketing content for the campaign? | 2025-02-16 13:00:00   |
| 8         | 8        | 7          | I'll go through it and get back to you shortly. | 2025-02-16 13:10:00   |
| 9         | 9        | 10          | Isabella, I need your help with a financial report. | 2025-02-16 14:00:00   |
| 10        | 10       | 9         | Sure, I'll get on it and send it to you by Thursday. | 2025-02-16 14:05:00   |
| 11        | 11       | 12         | Ava, we have a system outage. Can you help with this? | 2025-02-16 15:00:00   |
| 12        | 12       | 11         | I'm on it. Let's fix this ASAP. | 2025-02-16 15:10:00   |
| 13        | 13       | 14         | Sophia, I need the budget allocation for the upcoming quarter. | 2025-02-16 16:00:00   |
| 14        | 14       | 13         | I'll prepare the documents and send them to you shortly. | 2025-02-16 16:05:00   |
| 15        | 15       | 1         | Benjamin, can you design a new feature for our app? | 2025-02-16 17:00:00   |
| 16        | 16       | 15          | Sure! I'll start working on it today. | 2025-02-16 17:05:00   |
| 17        | 17       | 3          | Michael, do you have the product strategy document ready? | 2025-02-16 18:00:00   |
| 18        | 18       | 1          | Yes, I'll email it to you in a few minutes. | 2025-02-16 18:05:00   |
| 19        | 19       | 7          | Chris, can you troubleshoot the software issue we're facing? | 2025-02-16 19:00:00   |
| 20        | 20       | 5          | I'll check it out and get back to you. | 2025-02-16 19:05:00   |

## Hobby Table
```sql
SELECT * From Hobby;
```
| HobbyID | HobbyName   | Description                                              |
|---------|-------------|----------------------------------------------------------|
| 1       | Photography | Capturing moments and scenes with a camera to preserve memories. |
| 2       | Cooking     | Preparing meals by combining ingredients and following recipes. |
| 3       | Reading     | Engaging in the activity of reading books, articles, or other written materials. |
| 4       | Hiking      | Walking long distances, usually on trails or in nature. |
| 5       | Music       | Playing instruments or listening to music to express emotions or relax. |
| 6       | Gardening   | Cultivating plants and flowers for aesthetic or practical purposes. |
| 7       | Painting    | Creating artwork using various techniques, such as watercolor, oil, or acrylics. |

## Employee_hobby Table
```sql
SELECT * FROM Employee_hobby;
```
| EmployeeHobbyID | EmployeeID | HobbyID |
|-----------------|-----------|---------|
| 1               | 1         | 1       |
| 2               | 2         | 3       |
| 3               | 3         | 4       |
| 4               | 4         | 5       |
| 5               | 5         | 6       |
| 6               | 6         | 7       |
| 7               | 7         | 2       |
| 8               | 8         | 3       |
| 9               | 9         | 4       |
| 10               | 10        | 1       |
| 11              | 11        | 5       |
| 12              | 12        | 6       |
| 13              | 13        | 7       |
| 14              | 14        | 2       |
| 15              | 15        | 3       |

