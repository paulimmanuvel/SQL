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
insert into student value(109,"lal",29,"A")
update student set age=21 where id=101
delete from student where id=108
select * from student where age>19 order by age asc
select * from student where name in ("paul","sri")
select * from student where f_grade in ("A" ,"B") and age >
select * from student where age between 20 and 22
select * from student where age < 21
select * from student where f_grade < "C" order by f_grade asc
select count(*) from student
select avg(age) from student 
select avg(age) from student where f_grade in ("A","B")
select count(f_grade),f_grade from student group  by f_grade order by f_grade asc
select avg(age),f_grade from student group by f_grade
select count(id) from student group by f_grade order by count(id) desc limit 1
select avg(age),f_grade from student group by f_grade having avg(age)>20
select count(f_grade),f_grade from student group by f_grade having count(f_grade) >3
select avg(age),f_grade from student group by f_grade having avg(age) between 20 and 22
select * from student order by age asc
select * from student where f_grade in ("A","B") ORDER by age desc
select * from student order by f_grade asc 
delete from student 
select max(age) from student where age<(select max(age) from student)
select max(age),f_grade from student group by f_grade
select count(age),age from student group by age having count(age)>1
select name from student where name like 'r%'
select name from student where name not like '%m%'
select count(age),age from student group by age having count(age)>1
select max(age),f_grade from student group by f_grade 
select * from student where name like "%a%"
select * from student where name like "____"
select * from student where name  like "s_i" 
select * from student where name like "%l%" 
select * from student where name like"p%%a"
select * from student where row<=4
select row_number , name from student
select max(age),f_grade from student group by f_grade
