🏥 Hospital Management System

A robust desktop-based hospital management application developed in Java using Swing for the GUI and MySQL for database management.
This system simulates real-world hospital workflows, providing a secure, efficient, and user-friendly interface for managing patients, rooms, doctors, departments, ambulance services, and discharge processes.

Features
Authentication & Security

Secure Login:
Users must authenticate using valid credentials stored in the MySQL database.

Access Control:
Prevents unauthorized access to hospital data and system modules.

Role-Based Navigation:
Successful login redirects users to the Reception Dashboard.

Reception Dashboard

A centralized control panel that provides access to all hospital operations:

New Patient Registration

Update Patient Details

Doctor Information Management

Department List

Room Status Monitoring

Room Search

Ambulance Services

Patient Discharge

All Patients Information

Patient Management
New Patient Registration

Register patients with:

Name, Age, Gender

Disease, Phone Number

Aadhar Number, Address

Dynamic room allocation

Automatic update of room availability

Update Patient Details

Modify existing patient records

Update:

Room number

Contact details

Age and disease

Changes are instantly reflected in the database

Patient Discharge & Billing

Auto-fetch patient details

Calculate total stay duration

Generate billing automatically

Free room by updating its status to Available

Remove patient from active records

Room Management

View complete room details:

Room Number

Availability Status

Cleaning Status

Room Price

Room Type

Auto-refreshes based on live database data

Room Search

Filter rooms based on:

AC / Non-AC

Single / Double

Availability

Results displayed using a dynamic JTable powered by SQL queries

Doctor Management

Manage doctor information including:

Doctor Name

Qualification

Specialization

Experience

Displayed in a structured tabular format

Department Management

View all hospital departments

Uses SQL JOIN with the Doctor table

Accessible directly from the Reception Dashboard

Ambulance Services

Register ambulance cases

Store patient details:

Name, Age, Gender

Aadhar Number

Simple and fast navigation with Back button support

Technology Stack:-

| **Layer**           | **Technology**                                       |
| ------------------- | ---------------------------------------------------- |
| 🎨 **Frontend**     | Java Swing (JFrame, JPanel, JTable, JButton, Choice) |
| 🗄 **Backend**      | MySQL Database                                       |
| 🔗 **Connectivity** | JDBC                                                 |
| 📚 **Libraries**    | net.proteanit.sql.DbUtils                            |
| 🧩 **Paradigm**     | Object-Oriented Programming                          |

