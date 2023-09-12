
  # Habima Project

## Overview
As the Habima Theater became a part of the municipal corporation, a significant shift occurred in the payment system for employees within the technical departments. This transition moved away from hourly contracts to adopt a Task-Based Payment Method, The new method led to significant changes in the theater's work processes, starting from weekly work schedules to salary calculations.

## My Role
As the COO Assistant at the theater(2022), my primary responsibility was to develop a solution that would enable the implementation of the task-based method.

## The Task-Based Method
The Task-Based Payment Method introduced several key features:

### Task Assignment
Tasks were assigned to employees within the weekly work schedules. When an employee completed multiple tasks consecutively on the same day, they became eligible for a percentage increase over the base task value, capped at 200%. 

Example:
- Base Task Value: $100
- First Task: 100% of base
- Second Task: 20% of base
- Third Task: 20% of base
- Fourth Task: 60% of base

Four tasks in a row on the same day would result in a total payment of $200 for that day.

### Gap Between Tasks
If there was a significant time gap between two assigned tasks, the second task would not receive a 20% increase but would be treated as a new task, starting at 100% of the base task value.

Example:
- 8 am-12 am : Set construction 
- 18 pm-21 pm : Play

For that day, the payment would be 100% + 100%.

### Extra Pay
Employees received additional compensation as mandated by law for night shifts or holidays, which amounted to a 50% increase. This required the recording of clock-in and clock-out times.

### Distance-Based Pay
Tasks also included extra pay based on the distance from the theater, particularly for performances held outside the theater, which could occur anywhere in Israel.

### Base Task Value
The base task value was determined by an employee's seniority within the organization.

### Minimum Total Tasks
A minimum total of tasks per employee per month was established. If an employee did not reach this monthly minimum, the theater would compensate them to meet the minimum requirement.

Example: With all the extra pay and percentage increases, an employee completed 18.6 tasks, while the minimum requirement was 20 tasks. In this case, the employee would be compensated for 20 tasks.

This GitHub project aims to provide insights into the transition to the Task-Based Payment Method and the associated changes in operational procedures at Habima Theater.


## The exsisting work-process (hourly contacrt):
![image](https://github.com/liormat401/Habima-project/assets/126070709/52dabd33-2cc0-4530-bcdc-cc929370151f)

- **Problem 1**: Work schedules were sent to the C.O.O in any format the department manager chose - PDF, Word, Excel.
- **Problem 2**: Clock data couldn't calculate the number of tasks; it only served as proof for extra pay during night shifts or holidays.
- **Problem 3**: Unexpected changes in the weekly work arrangements needed to be supervised.the could cause recalculation of the task percentage values, requiring C.O.O approval to prevent fraud.
  
  For example, an urgent task not in the weekly schedule was assigned to an employee with a time gap instead of one who could complete tasks consecutively.
 - **Problem 4**: By law, employees needed a detailed sheet to know what they were being paid for, something that HR and clock data couldn't provide due to the lack of task-level detail.

## Conclusion
In conclusion, there was no existing software or calculator available for this new payment method; everything was handled through emails. Furthermore, the new method was not finalized, leaving no budget or time for the purchase and customization of an existing solution.

This GitHub project aims to provide insights into the transition to the Task-Based Payment Method and the associated changes in operational procedures at Habima Theater.

## Implementing and Developing a Solution
To address these challenges, I decided to work with Excel. It offers several advantages, including user-friendliness, no need for technical expertise, free usage, easy maintenance, and cloud protection.

### Dedicated Weekly Work Schedule Format
- Data validation: Integrating employee names in the work schedule with the database ensures consistency.
- Conditional formatting: Checks for compliance with labor laws and detects double assignments of employees.
  
  This format was designed to facilitate seamless data import into the database. It allows the database to efficiently calculate the total tasks per employee and their respective percentage values, even in cases with time gaps between tasks.

### Change Request Format
- When there is a change in the schedule, the department manager can fill out a change request form, which includes details about time and task assignment. The form is then submitted for approval from the C.O.O.

### Database
- The main table includes dates, employees, and detailed task payment information.
- Employees Table- contains ID, Employee Number, Name, Date of Start, Seniority (calculated from the last), and Base Task Value (calculated from the last).
- Distance Table contains distance information, including city names, distance classifications, and Distance-Based Pay rates.
- An analysis sheet calculates the monthly wage for the C.O.O and the C.F.O.



This comprehensive solution streamlines the task-based payment process and enhances transparency for both employees and management.



![image](https://github.com/liormat401/Habima-project/assets/126070709/3dcf1681-105d-49ef-9a0a-cfcdac644f6b)

## My real vision

If I had the budget and Dev team,my final vision solution was:
- One system that automates and communicates with all other systems in the Theater including clock-data.
- Differet screens to COO and technical deparntments managers:
  
  ![image](https://github.com/liormat401/Habima-project/assets/126070709/db22737a-dab8-4b19-a53a-f6d60b2f5408)
  _COO screen_

  ![image](https://github.com/liormat401/Habima-project/assets/126070709/72095e24-9762-4932-a44c-3dda123acfc4)
  _Technical Depratment Manager's screen_

- compliance with labor laws checkings and detecting double assignments of employees, while assigning the weekly-work schedule
- 
With two options- send to the coo, and a locked option is to publish to employees. the last he can do only if the C.O.O had locked the weekly work schedule and accepted it in his screen 

![image](https://github.com/liormat401/Habima-project/assets/126070709/b4276f9d-92ea-4eaf-acdf-f46033c90e12)
_Manager's screen for weekly-work schedule_

- Change Request in more user-friendly way for the managers
![image](https://github.com/liormat401/Habima-project/assets/126070709/f8d7be8a-ff20-44ba-bcec-05e3dba077fc)
_Manager changing name as for employee sick and other replaced him_

- Organized screen of requested, with each request from the manager there is clock data(triggered from date and employee ID) for evidence
- ![image](https://github.com/liormat401/Habima-project/assets/126070709/bdc623f3-c330-44e1-b8f1-5173c73cffa0)
  _COO's screen of messages and requests_

  



  


## Personal Reflection
As a junior with zero work experience in a role like this and without the guidance of a senior or a dedicated technology team, I am incredibly proud of what I've accomplished. The journey to think,create and implement these changes has been a tremendous learning experience.

While the solutions I've developed have made impact, I recognize that there is room for improvement. There is need for better automation and dedicated software to handle the work processes described above. This would enhance efficiency.
But as I said above,there was no budget for software if the tasks-method would go back to hourly payment.



Thank you for taking the time to explore this project and my personal reflection:)


