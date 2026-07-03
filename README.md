# School Fees Payment Tracking System

A desktop GUI application, built with **Java Swing**, that helps a school's
accounts office register students, record fee payments across multiple
payment channels, and monitor collections in real time.

Developed as term paper <img width="956" height="504" alt="USER INTERFACE" src="https://github.com/user-attachments/assets/3d5e1bd2-4319-44b5-97b1-fb428cde73db" />
<img width="959" height="500" alt="STUDENT REPORT" src="https://github.com/user-attachments/assets/5ab5c7ad-76ea-4b52-912e-b66353d71c09" />
<img width="940" height="495" alt="REGISTERING STUDENT" src="https://github.com/user-attachments/assets/cb259635-3320-4909-b2c2-10122e211a50" />
<img width="947" height="505" alt="RECORD PAYMENT" src="https://github.com/user-attachments/assets/155e6960-9053-4343-8f07-e243e8d901ff" />
<img width="953" height="505" alt="PAYMENT HISTORY" src="https://github.com/user-attachments/assets/fb4b7b93-cc9e-4ebe-bda4-6a1eac8e9df2" />
for **INF811D: Object Oriented Programming**, MSc Information
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
!
## Author
Name: Isaac Otabil
Index Number: MS/ITE/25/0014 

