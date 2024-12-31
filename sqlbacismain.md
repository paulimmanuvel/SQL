create table student (
id int,
name varchar(50),
age int
)
select * from student
alter table student add grade varchar(50)
alter table student change grade f_grade varchar(50)
insert into student value(101,"paul",20,"A")
insert into student value(102,"immi",21,"C")
insert into student value(103,"luke",22,"A")
insert into student value(104,"adam",21,"B")
insert into student value(105,"robert",22,"A")
insert into student value(106,"sri",24,"c")
insert into student value(107,"prabha",20,"f")
insert into student value(108,"ram",19,"A")
update student set age=21 where id=101
delete from student where id=101
select * from student where age>21
select * from student where name in ("adam" , "sri")
select * from student where f_grade in ("A","B") and age>20
select * from student order by age asc
select * from student where age between 18 and 23
select * from student where age<20
select * from student where f_grade>"C"
select count(*) from student
select avg(age),f_grade from student group by f_grade
select avg(age) from student where f_grade in ("A" , "B")
select count(*),f_grade from student group by f_grade order by f_grade asc
select avg(age),f_grade from student group by f_grade order by avg(age) asc
select count(age),f_grade from student group by f_grade order by count(age) desc limit 1
select avg(age),f_grade from student group by f_grade having avg(age)>20 
select count(f_grade),f_grade from student group by f_grade having count(f_grade)<3
select avg(age),f_grade from student group by f_grade having avg(age) between 21 and 25
select * from student order by age asc
select * from student where f_grade in ("A","B") order by f_grade desc
select * from student order by f_grade asc
