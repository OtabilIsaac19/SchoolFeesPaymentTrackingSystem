# School Fees Payment Tracking System

## Project Description

This **School Fees Payment Tracking System** is a GUI-based Java application developed to help schools record, monitor, and manage student school fees payments. The system allows users to add student payment records, calculate outstanding balances, view payment status, and search for student fee information.

This project was individually developed for **INF811D: Object Oriented Programming** as a semester term paper/practical project.

## Features

- Add student fee payment records
- Store student details such as Student ID, name, and programme/class
- Record total school fees and amount paid
- Automatically calculate outstanding balance
- Display payment status as:
  - Fully Paid
  - Partially Paid
  - Not Paid
- Search student payment records
- Update payment information
- Validate user input
- Display records using a graphical user interface

## Technologies Used

- Java
- Java GUI Framework: Java Swing or JavaFX
- Object-Oriented Programming
- IntelliJ IDEA / NetBeans / Eclipse / VS Code

## Object-Oriented Programming Concepts Applied

### Encapsulation

Class attributes are kept private and accessed through getter and setter methods. This protects student and payment data from direct modification.

### Inheritance

The system can use a parent class such as `Person`, with `Student` inheriting common properties like ID and name.

### Polymorphism

Methods such as `displayDetails()` can be overridden in different classes to show different types of information.

### Abstraction

Abstract classes or interfaces can be used to define important payment operations such as calculating balance and checking payment status.

## Suggested Project Structure

```text
SchoolFeesPaymentTrackingSystem/
│
├── src/
│   ├── Main.java
│   ├── Student.java
│   ├── Payment.java
│   ├── FeeRecord.java
│   └── FeeManager.java
│
├── screenshots/
│   ├── dashboard.png
│   ├── add-record.png
│   └── payment-status.png
│
├── README.md
└── School_Fees_Payment_Tracking_System_Technical_Report.docx
```

## How to Run the Application

1. Download or clone this repository.
2. Open the project in your preferred Java IDE, such as IntelliJ IDEA, NetBeans, Eclipse, or VS Code.
3. Make sure Java is installed on your computer.
4. Open the `src` folder.
5. Run the `Main.java` file.
6. Use the graphical interface to manage student fee payment records.

## Sample Use of the System

1. Enter the student ID, student name, programme/class, total fees, amount paid, and payment date.
2. Click the **Add Record** button.
3. The system calculates the outstanding balance automatically.
4. The payment status is displayed as Fully Paid, Partially Paid, or Not Paid.
5. Use the search function to find a student record.

## Screenshots
<img width="956" height="504" alt="USER INTERFACE" src="https://github.com/user-attachments/assets/dd391981-58d9-47b0-8233-94bbed7caa49" />
<img width="959" height="500" alt="STUDENT REPORT" src="https://github.com/user-attachments/assets/178bcc57-8f8b-461e-8e85-072f6b78d924" />
<img width="940" height="495" alt="REGISTERING STUDENT" src="https://github.com/user-attachments/assets/015a702d-5ccc-474a-8a4b-8cee266f09ab" />
<img width="947" height="505" alt="RECORD PAYMENT" src="https://github.com/user-attachments/assets/a6adef5e-75c1-4c21-82bd-6d657b610118" />
<img width="953" height="505" alt="PAYMENT HISTORY" src="https://github.com/user-attachments/assets/44369660-d350-4975-bbaf-dbb4218bb8ae" />




## Author

**Name:** Isaac Otabil  
**Index Number:** MS/ITE/25/0014

**Programme:** MSc Information Technology  
**Course:** INF811D - Object Oriented Programming  
**Institution:** University of Cape Coast  

## GitHub Repository

GitHub repository link here:https://github.com/Isaac1519/SchoolFeesPaymentTrackingSystem


```text
https://github.com/Isaac1519/SchoolFeesPaymentTrackingSystem
```

## Conclusion

The School Fees Payment Tracking System provides a simple and organized way to manage student school fees payments. It improves accuracy, reduces manual record-keeping errors, and demonstrates the practical application of Object-Oriented Programming concepts in Java.
