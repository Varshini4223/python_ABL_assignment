## Comprehensive Smart Campus Management Simulation
# 1. Problem Statement
A Smart Campus Management System is designed to simplify and automate various activities within a college campus. The system manages student information, attendance records, library operations, fee payments, and campus facility usage.

The main objective of this project is to develop a Python-based simulation that integrates multiple campus management activities into a single system. It accepts student details and allows users to perform different operations through a menu-driven interface.

The system calculates attendance percentages, checks library book availability, tracks fee payment status, and manages campus facility bookings. It also validates user inputs and displays appropriate messages based on the selected operations.

This project demonstrates how Python programming concepts such as conditional statements, loops, functions, lists, dictionaries, and input validation can be used to solve real-world campus management problems.
# 2. Algorithm
1. Start the program.
2. Display the welcome message for the Smart Campus Management System.
3. Accept the student's details, such as student ID, name, department, and year.
4. Display the main menu with the following options:
   - Student Information Management
   - Attendance Management
   - Library Management
   - Fee Payment Management
   - Campus Facility Booking
   - Exit
5. Ask the user to select an operation.
6. Perform the selected operation:
   - Student Information: Display the student's personal and academic details.
   - Attendance Management: Accept the number of classes attended and total classes, calculate the attendance percentage, and display the attendance status.
   - Library Management: Display available books and allow the user to borrow or return a book.
   - Fee Payment Management: Accept the total fee and amount paid, calculate the remaining balance, and display the payment status.
   - Campus Facility Booking: Display available facilities and allow the user to select a facility for booking.
7. Validate all inputs and display suitable error messages for invalid entries.
8. After completing an operation, display the main menu again.

# flowchart TD
    A([Start]) --> B[Display Welcome Message]
    B --> C[Enter Student Details]
    C --> D[Display Main Menu]
    D --> E[/Select an Operation/]
    E --> F{Check Choice}

    F -->|1| G[Display Student Information]
    F -->|2| H[Enter Attendance Details]
    H --> I[Calculate Attendance Percentage]
    I --> J[Display Attendance Status]

    F -->|3| K[Display Library Books]
    K --> L[Borrow or Return Book]

    F -->|4| M[Enter Fee Details]
    M --> N[Calculate Remaining Fee]
    N --> O[Display Payment Status]

    F -->|5| P[Display Campus Facilities]
    P --> Q[Select and Book Facility]

    G --> R{Return to Menu?}
    J --> R
    L --> R
    O --> R
    Q --> R

    R -->|Yes| D
    R -->|No| S[Display Thank You Message]
    F -->|6| S
    F -->|Invalid Choice| T[Display Error Message]
    T --> D

    S --> U([Stop])

# 4. Input
The program accepts the following inputs from the user:
Module	Required Input
Student Information	Student ID, Name, Department, Year
Attendance Management	Total classes, Classes attended
Library Management	Book name, Borrow or Return choice
Fee Payment	Total fee, Amount paid
Facility Booking	Facility name, Booking date, Time slot
Main Menu	User's operation choice

# Sample Input
1. Student Details
Enter Student ID: 101
Enter Student Name: Rahul
Enter Department: CSE-AIML
Enter Year: 1



2. Attendance Details
Enter Total Classes: 50
Enter Classes Attended: 45



3. Library Management
Available Books:
1. Python Programming
2. Data Structures
3. Computer Networks

Enter Book Name: Python Programming
Select Operation: Borrow



4. Fee Payment
Enter Total Fee: 50000
Enter Amount Paid: 30000



5. Campus Facility Booking
Available Facilities:
1. Seminar Hall
2. Computer Lab
3. Sports Ground

Enter Facility Name: Seminar Hall
Enter Booking Date: 05-11-2026
Enter Time Slot: 10:00 AM



6. Main Menu
Enter your choice: 2
10. Repeat the process until the user selects the Exit option.
11. Display a thank-you message.
12. Stop the program.

# Sample Output
===== SMART CAMPUS MANAGEMENT SYSTEM =====

Student ID: 101
Student Name: Rahul
Department: CSE-AIML
Year: 1

Attendance Percentage: 90%
Attendance Status: Satisfactory

Library Status: Python Programming
Book borrowed successfully!

Total Fee: Rs. 50000
Amount Paid: Rs. 30000
Remaining Fee: Rs. 20000
Payment Status: Partially Paid

Facility: Seminar Hall
Booking Date: 05-11-2026
Time Slot: 10:00 AM
Booking Status: Confirmed

Thank you for using Smart Campus Management System!
