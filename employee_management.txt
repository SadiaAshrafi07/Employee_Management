-----------------------------------
create database assignment;
use assignment;
-----------------------------------

create table employee(id int primary key auto_increment comment 'Unique Employee ID',
name varchar(50) not null,
department varchar(50) not null,
salary decimal(10,2) not null,
join_date date not null) comment='Stores Employee details';

------------------------------------

insert into employee(name,department,salary,join_date)
values
('John Doe','HR',50000.00,'2024-01-15'),
('Jane Smith','IT',60000.00,'2024-03-22'),
('Alice Johnson','Finance',55000.00,'2024-07-30'),
('Bob Brown','IT',62000.00,'2025-02-10'),
('Charlie Davis','HR',48000.00,'2025-05-05');

-------------------------------------
alter table employee modify salary decimal(10,2) comment='Employee Monthly Salary';

----------------------------------------
select distinct department from employee;
-------------------------------------------
select name 'Employee Name',salary 'Employee Salary' from employee;

---------------------------------------------

 insert into employee(name,department,salary,join_date)
                                           -> values('Eva Green','Finanace',54000.00,'2024-07-23');
										   
select * from employee;										   