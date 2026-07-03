# School Fees Payment Tracking System

A desktop GUI application, built with **Java Swing**, that helps a school's
accounts office register students, record fee payments across multiple
payment channels, and monitor collections in real time.

Developed for **INF811D: Object Oriented Programming**, MSc Information
Technology Programme, College of Distance Education (CoDE), University of
Cape Coast — 2025/2026 Academic Year.

## Features

- Register students with programme, level and total fees due
- Record payments via **Cash**, **Mobile Money**, or **Bank Transfer**
- Automatic receipt number generation and balance calculation
- Dashboard showing total students, total collected, total outstanding,
  and number of students still in arrears
- Full payment history table
- Search a specific student's fee record or view all students at once
- Input validation and custom exception handling throughout
  (invalid amounts, overpayment, duplicate student IDs, unknown student IDs)

## Object-Oriented Concepts Demonstrated

| Concept | Where |
|---|---|
| Encapsulation | Private fields with getters/setters in `Person`, `FeeInvoice`, `Payment`, etc. |
| Inheritance | `Student` and `Admin` extend `Person`; `CashPayment`, `MobileMoneyPayment`, `BankTransferPayment` extend `Payment` |
| Abstraction | `Person` and `Payment` are abstract classes with abstract methods |
| Polymorphism | `getRoleDescription()` and `getPaymentDetails()` behave differently for each subclass at runtime |
| Exception Handling | Custom checked exceptions: `InvalidAmountException`, `OverpaymentException`, `DuplicateStudentException`, `StudentNotFoundException` |
| Collections | `ArrayList` and `LinkedHashMap` in `FeeManager` |
| Event-driven programming | Swing `ActionListener`s on every button/combo box |

## Project Structure

```
SchoolFeesPaymentTrackingSystem/
├── src/
│   ├── Person.java                 (abstract)
│   ├── Student.java
│   ├── Admin.java
│   ├── FeeInvoice.java
│   ├── Payment.java                (abstract)
│   ├── CashPayment.java
│   ├── MobileMoneyPayment.java
│   ├── BankTransferPayment.java
│   ├── InvalidAmountException.java
│   ├── OverpaymentException.java
│   ├── DuplicateStudentException.java
│   ├── StudentNotFoundException.java
│   ├── FeeManager.java
│   ├── MainFrame.java              (GUI)
│   └── SchoolFeesApp.java          (entry point)
└── README.md
```

## How to Run

Requires JDK 17 or later (no external libraries needed — pure Java Swing).

```bash
cd SchoolFeesPaymentTrackingSystem
javac -d bin src/*.java
java -cp bin SchoolFeesApp
```

The application opens with three sample students and two sample payments
already loaded so the dashboard and tables are not empty on first launch.

## Screenshots
<img width="956" height="504" alt="USER INTERFACE" src="https://github.com/user-attachments/assets/d8d5a4de-242d-48d3-8498-a432b5a99ce8" />
<img width="959" height="500" alt="STUDENT REPORT" src="https://github.com/user-attachments/assets/9b95650f-c7e5-4a94-b712-2832be753e54" />
<img width="940" height="495" alt="REGISTERING STUDENT" src="https://github.com/user-attachments/assets/3b46a694-fe29-464f-9be6-559ef07048ee" />
<img width="947" height="505" alt="RECORD PAYMENT" src="https://github.com/user-attachments/assets/4f071cba-0ce6-4bac-93db-0bf31611c4e1" />
<img width="953" height="505" alt="PAYMENT HISTORY" src="https://github.com/user-attachments/assets/44b47081-a6f5-4e90-ab39-d4eaa0ac9760" />

## Author
Name: Isaac Otabil
Index Number: MS/ITE/25/0014 

