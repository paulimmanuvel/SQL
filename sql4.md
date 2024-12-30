create table emp(
emp_id int,
emp_fname varchar(50),
emp_lname varchar(50),
emp_dept varchar(50),
emp_sal int
)
select * from emp
insert into emp value(1,"john","doe","HR",55000)
insert into emp value(2,"paul","imm","Buss",67000)
insert into emp value(3,"ram","prabha","HR",69000)
insert into emp value(4,"tim","cook","Buss",90000)
insert into emp value(5,"alen","prem","lead",100000)
insert into emp value(6,"virat","koli","lead",120000)
select * from emp order by emp_lname asc
select * from emp where emp_dept="HR" order by emp_sal desc
select count(emp_id),emp_dept from emp group by emp_dept
select avg(emp_sal),emp_dept from emp group by emp_dept order by emp_dept asc
select avg(emp_sal),emp_dept from emp group by emp_dept order by avg(emp_sal) desc limit 1
