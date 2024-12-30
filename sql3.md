create table stu(
name varchar(50),
mark int,
dept varchar(50)
)
select * from stu
insert into stu value("paul",45,"CSE")
insert into stu value("robert",46,"CSBS")
insert into stu value("prabha",30,"ECE")
insert into stu value("Virat",28,"Sports")
insert into stu value("koli",38,"CSE")
insert into stu value("sri",43,"CSBS")
select * from stu where dept="CSE"
select name,mark from stu order by name desc
select name , mark from stu order by mark asc
select count(name), dept from stu group by dept
select sum(mark),dept from stu group by dept
select count(name),dept from stu group by dept order by count(name) asc
