# MotorPH Payroll System

## Project Overview
The MotorPH Payroll System is a Java-based console application designed to automate payroll processing for employees of MotorPH. The system reads employee information and attendance records from CSV files and calculates employee salaries based on their working hours and hourly rate.

The system helps improve payroll accuracy by automating the computation of gross salary, deductions, and net salary.

---

## Program Details

The MotorPH Payroll System is developed using Java in Apache NetBeans IDE. The application processes employee data and attendance logs stored in CSV files to generate payroll results.

The program loads employee details and attendance records at the start of the system and performs payroll computations based on the recorded working hours.

The system supports two user roles:

Employee – allows employees to view their personal information by entering their employee number.

Payroll Staff – allows payroll staff to process payroll for one employee or all employees.

The program calculates employee work hours using attendance records that contain log-in and log-out times. The system applies company payroll rules such as official work hours, break deductions, and cutoff payroll periods.

Payroll is calculated in two cutoff periods each month:
• First cutoff: 1st – 15th of the month  
• Second cutoff: 16th – end of the month

The first cutoff payout does not include deductions, while the second cutoff payout includes all mandatory government deductions.

The system automatically computes the following deductions:
• SSS contribution  
• PhilHealth contribution  
• Pag-IBIG contribution  
• Withholding tax  

After deductions are applied, the program displays the employee's net salary.

---

## System Features

### 1. Login System
The system includes a simple authentication feature with two user roles:
- Employee
- Payroll Staff

Users must enter a valid username and password to access the system.

### 2. Employee Information Viewing
Employees can enter their employee number to view basic personal information such as:
- Employee Number
- Employee Name
- Birthday

### 3. Payroll Processing
Payroll staff can generate payroll reports for:
- One employee
- All employees

The system calculates:
- Total hours worked
- Gross salary
- Government deductions
- Net salary

### 4. Attendance-Based Salary Computation
The system reads attendance logs and calculates working hours based on:
- Log-in time
- Log-out time
- Official work schedule

Payroll rules applied:
- Official work hours: 8:00 AM – 5:00 PM
- Log-ins between 8:00–8:05 AM are treated as on-time
- Early log-ins are not counted
- Overtime hours are not included
- A 1-hour break is deducted daily

### 5. CSV Data Processing
The system reads information from two CSV files:

Employee Details CSV – contains employee records such as name, position, and hourly rate.

Attendance Record CSV – contains employee log-in and log-out records used to compute working hours.

---

## Technologies Used

- Java
- CSV File Handling
- Java Time API (LocalDate, LocalTime)
- Java Collections Framework (Map, List)
- Apache NetBeans IDE

---

## How to Run the Program

1. Download or clone the repository.
2. Open the project using Apache NetBeans IDE.
3. Make sure the CSV files are located in the correct folder inside the project.
4. Run the `MotorPHPayrollSystem.java` file.
5. Enter the login credentials to access the system.

Example login:

Employee  
Username: employee  
Password: 12345  

Payroll Staff  
Username: payroll_staff  
Password: 12345  


### Member Contributions

| Member Name | Contribution |
|-------------|--------------|
| Rose Ann Soriano |Java programming, payroll computation logic  |
| Rose Ann Soriano | CSV data preparation and testing |
| Rose Shainnah Viray| Documentation and project planning |

## Project Plan Link
[Project Plan](https://docs.google.com/spreadsheets/d/1_m45CKZOxXQACvRq4Trh9mC0srFXp7PWaBj8YFjnHbc/edit?usp=sharing)
