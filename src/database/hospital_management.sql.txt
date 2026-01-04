CREATE DATABASE hospital_management_syatem;
use hospital_management_syatem;

create table login(ID varchar(20) , PW varchar(20));
insert into login value("techcoder" , "123456789");
insert into login value("Abhishek" , "8863808059");

select DISTINCT * from login;

create  table Room(room_no varchar(20), availability varchar(20), Price varchar(20), Room_type varchar(20));

insert into Room values("100","Available","500","G Bed 1");
insert into Room values("101","Available","500","G Bed 2");
insert into Room values("102","Available","500","G Bed 3");
insert into Room values("103","Available","500","G Bed 4");
insert into Room values("200","Available","1500","Private Room");
insert into Room values("201","Available","1500","Private Room");
insert into Room values("202","Available","1500","Private Room");
insert into Room values("203","Available","1500","Private Room");
insert into Room values("300","Available","3500","ICU Bed 1");
insert into Room values("301","Available","3500","ICU Bed 2");
insert into Room values("302","Available","3500","ICU Bed 3");
insert into Room values("303","Available","3500","ICU Bed 4");
insert into Room values("304","Available","3500","ICU Bed 5");
insert into Room values("305","Available","3500","ICU Bed 6");

Select DISTINCT * from room;

Create table department(Department varchar(100) , Phone_no varchar(20));
Insert into department values("Surgical department",	"123456789");
Insert into department values("Operation theater complex (OT)",	"123456789");
Insert into department values("Paramedical department"	,"123456789");
Insert into department values("Nursing department",	"123456789");

select DISTINCT * from department;

Create table EMP_INFO(Name varchar(20), Age varchar(20) , Phone_number varchar(20) , salary varchar(20) , Gmail varchar(20) , Aadhar_Number varchar(20));
Insert into EMP_INFO values("Doctor2", "40" , 	"9852977367" , 	"55000", "dr2@gmail.com", "123456789151");
Insert into EMP_INFO values("Doctor1" , "30",	"8863808059" ,	"50000", "dr1@gmail.com", "123456789101");
Insert into EMP_INFO values("Doctor3" , "50",	"8863808060" ,	"59000", "dr3@gmail.com", "123456789131");

select DISTINCT * from EMP_INFO;

create table Ambulance(Name varchar(20) , Gender varchar(20) ,  Car_name varchar(20), Available varchar(20) , Location varchar(20));
Insert into Ambulance values("av" , "Male" , "Alto", "Available" , "area 16");
Insert into Ambulance values("Anshu" , "Male" , "Omni", "Available" , "Front gate");
Insert into Ambulance values("Ujjwal " , "Male" , "Force", "Available" , "Backgate");
Insert into Ambulance values("Suhani" , "Female" , "Truck", "Available" , "area 51");

SELECT * FROM Ambulance;

DROP table Ambulance;
DROP table EMP_INFO;
DROP table department;

CREATE TABLE department (
    dept_name VARCHAR(100) PRIMARY KEY,
    phone_number VARCHAR(20)
);
INSERT INTO department (dept_name, phone_number) VALUES
('Cardiology', '1234567890'),
('Neurology', '9876543210'),
('Orthopedics', '8765432109'),
('Pediatrics', '7654321098');


CREATE TABLE doctor (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    department VARCHAR(100),
    education VARCHAR(100),
    specialization VARCHAR(100),
    phone VARCHAR(20),
    fees VARCHAR(20),
    FOREIGN KEY (department) REFERENCES department(dept_name)
);

INSERT INTO doctor (name, department, education, specialization, phone, fees) VALUES
('Dr. Rahul Sharma', 'Cardiology', 'MBBS, MD', 'Heart Specialist', '9998887771' , '1000'),
('Dr. Meena Singh', 'Neurology', 'MBBS, DM', 'Brain Surgeon', '9998887772', '1500'),
('Dr. Ajay Kumar', 'Orthopedics', 'MBBS, MS', 'Bone Specialist', '9998887773' , '1200'),
('Dr. Priya Verma', 'Pediatrics', 'MBBS, MD', 'Child Specialist', '9998887774', '500'),
('Dr. Kunal Sharma', 'Cardiology', 'MBBS, MD', 'Heart Specialist', '9998887652', '1000'),
('Dr. Kusum Singh', 'Neurology', 'MBBS, DM', 'Brain Surgeon', '9998887869', '1500'),
('Dr. Vijay Yadav', 'Orthopedics', 'MBBS, MS', 'Bone Specialist', '9998887695' ,'1200'),
('Dr. Diya Verma', 'Pediatrics', 'MBBS, MD', 'Child Specialist', '9998886354', '500');
SELECT 
    d.dept_name AS 'Department',
    d.phone_number AS 'Dept Phone',
    doc.name AS 'Doctor Name',
    doc.education AS 'Education',
    doc.specialization AS 'Specialization',
    doc.phone AS 'Doctor Phone',
    doc.fees AS 'Doctor fees'
FROM department d
LEFT JOIN doctor doc 
ON d.dept_name = doc.department
ORDER BY d.dept_name;



CREATE TABLE Patient_Info (
    id_type VARCHAR(50),
    number VARCHAR(50) PRIMARY KEY,
    name VARCHAR(100),
    gender VARCHAR(10),
    disease VARCHAR(100),
    department VARCHAR(100),
    doctor VARCHAR(100),
    room_number VARCHAR(20),
    time VARCHAR(100),
    deposit DECIMAL(10,2)
);

Select * FROM Patient_Info;
 
