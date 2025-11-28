🏥 𝐇𝐨𝐬𝐩𝐢𝐭𝐚𝐥 𝐌𝐚𝐧𝐚𝐠𝐞𝐦𝐞𝐧𝐭 𝐒𝐲𝐬𝐭𝐞𝐦
Java Swing + MySQL + JDBC

A fully-featured desktop-based Hospital Management System designed to automate patient registration, room allocation, doctor & department management, ambulance tracking, and discharge workflows.
The system is built using Java Swing for GUI and MySQL for database operations — offering a clean, efficient, and user-friendly experience.

🚀 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬
🔐 1. Login & Authentication

✔ Validates user credentials from MySQL

✔ Prevents unauthorized access

✔ Redirects to Reception dashboard upon success

🏥 2. Reception Dashboard

A centralized module connecting all features:

➕ New Patient Registration

🔄 Update Patient Details

👨‍⚕️ Doctor Information

🏛 Department List

🛏 Room Status

🔍 Search Room

🚑 Ambulance Service

📤 Patient Discharge

📋 All Patients Info

🧾 3. New Patient Registration

📝 Register patients with name, age, gender, disease, phone, Aadhar, address

🛏 Dynamic room assignment

🔄 Auto-updates room availability status

🔄 4. Update Patient Details

✏ Modify existing patient data

🔢 Edit room number, contact, age, disease, etc.

⚡ Instant reflection of updates in DB

📤 5. Patient Discharge Module

📥 Auto fetch patient details

📅 Calculates stay duration

💰 Generates billing

🛏 Frees room (sets status to Available)

🧹 Removes patient from active list

🏨 6. Room Management

Displays complete room details including:

🔢 Room number

🟢 Availability

🧼 Cleaning status

💸 Price & type

♻ Auto-refresh based on DB data

🔍 7. Search Room

Filter rooms by:

❄ AC / 🚫 Non-AC

🛏 Single / Double

🟢 Availability

📊 Dynamic JTable with SQL filters

👨‍⚕️ 8. Doctor Module

📛 Doctor name

🎓 Qualification

🧪 Specialization

📈 Experience

📋 Displayed in organized table view

🏛 9. Department Module

🏢 Shows all departments

🔗 SQL JOIN with doctor table

🌐 Easy access from Reception dashboard

🚑 10. Ambulance Module

📝 Register ambulance cases

👤 Stores patient info (name, age, gender, Aadhar, etc.)

🔙 Quick navigation with Back button
