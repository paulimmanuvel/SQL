create table emp1(
emp_name varchar(50),
emp_id int,
emp_exp int,
emp_add varchar(50)
)
select * from emp1 
insert into emp1 value("paul",101,2,"erode")
insert into emp1 value("ramya",102,4,"kupandapalayam")
insert into emp1 value("imaya",103,7,"banglore")
insert into emp1 value("ram",104,6,"coimbaotre")
insert into emp1 value("tim",105,"coimbatore")
insert into emp1 value("cook",106,"coimbatore")
update emp1 set emp_add="kumarapalayam" where emp_id=102
alter table emp1 change emp_add emp_address varchar(50)
select count(emp_id) from emp1
select count(emp_id) from emp1 where emp_address="coimbatore"
