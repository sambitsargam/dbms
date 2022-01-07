<h1>EXP 8 ANSWERS</h1>

1
```
Select Fname from employee where dno=any (Select dnum from project where pname='Product z');
```
2
```
Select Fname,address,salary from employee where (salary,dno)=any(select salary,dno from employee where fname='Ahmad');
```
3
```
Select Fname,super_ssn from employee where salary>(select max(salary) from employee where dno=4);
```
4
```
Select Dno,mgr_ssn from department where dnumber=any(select dnum from project whrere plocation='Stafford');
```
5
```
Select ssn,fname from employee where dno in(select dno from employee where fname like '%m%');
```
6
```
Select ssn,fname from employee join dependent d on e.ssn=d.ssn where dependent_name like 'A%';
```
7
```
Select ssn,fname,dno from employee where dno=any(select dno from employee where fname='Joyce') and fname!='Joyce';
```
8
```

```
9
```
Select pname,pnumber,plocation from project where plocation='Houston';
```
10
```
Select dnumber,dname from department d join project p on d.dnumber=p.dnum where plocation-'Sugarland';
```
11
```
Select fname from employee where not exists (select * from dependent d where ssn=essn);
```
<img src=screenshot.jpeg>
