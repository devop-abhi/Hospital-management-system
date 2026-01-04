🏥 𝐇𝐨𝐬𝐩𝐢𝐭𝐚𝐥 𝐌𝐚𝐧𝐚𝐠𝐞𝐦𝐞𝐧𝐭 𝐒𝐲𝐬𝐭𝐞𝐦
Java Swing • MySQL • JDBC

A fully-featured desktop-based Hospital Management System designed to automate and streamline:

Patient Registration, Room Allocation, Doctor & Department Management, Ambulance Tracking, and Discharge Workflows.

Built using Java Swing for an interactive GUI and MySQL for robust database operations — delivering a clean, efficient, and user-friendly experience.

🚀 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬
🔐 1. Login & Authentication

✔ Validates user credentials from MySQL

✔ Prevents unauthorized access

✔ Redirects to Reception Dashboard upon successful login

🧭 2. Reception Dashboard

A centralized control panel connecting all hospital operations:

➕ New Patient Registration

🔄 Update Patient Details

👨‍⚕️ Doctor Information

🏛 Department List

🛏 Room Status

🔍 Search Room

🚑 Ambulance Service

📤 Patient Discharge

📋 All Patients Information

📝 3. New Patient Registration

Register patients with:

Name, Age, Gender

Disease, Phone Number

Aadhar Number, Address

🛏 Dynamic room assignment

🔄 Auto-updates room availability status

✏️ 4. Update Patient Details

✏ Modify existing patient records

🔢 Edit room number, contact details, age, disease, etc.

⚡ Instant reflection of updates in the database

📤 5. Patient Discharge Module

📥 Auto-fetches patient details

📅 Calculates stay duration

💰 Generates billing

🛏 Frees room (status set to Available)

🧹 Removes patient from active list

🛏 6. Room Management

Displays complete room information, including:

🔢 Room Number

🟢 Availability Status

🧼 Cleaning Status

💸 Price & Room Type

♻ Auto-refresh using live database data

🔍 7. Search Room

Filter rooms using SQL-powered dynamic search:

❄ AC / 🚫 Non-AC

🛏 Single / Double

🟢 Availability

📊 Dynamic JTable with real-time filters

👨‍⚕️ 8. Doctor Module

📛 Doctor Name

🎓 Qualification

🧪 Specialization

📈 Experience

📋 Displayed in a structured table view

🏢 9. Department Module

🏢 Displays all hospital departments

🔗 Uses SQL JOIN with Doctor table

🌐 Quick access from Reception Dashboard

🚑 10. Ambulance Module

📝 Register ambulance cases

👤 Stores patient details:

Name, Age, Gender

Aadhar Number, etc.

🔙 Easy navigation with Back button

Technology Stack:-

| **Layer**           | **Technology**                                       |
| ------------------- | ---------------------------------------------------- |
| 🎨 **Frontend**     | Java Swing (JFrame, JPanel, JTable, JButton, Choice) |
| 🗄 **Backend**      | MySQL Database                                       |
| 🔗 **Connectivity** | JDBC                                                 |
| 📚 **Libraries**    | net.proteanit.sql.DbUtils                            |
| 🧩 **Paradigm**     | Object-Oriented Programming                          |

