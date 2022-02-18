```sql
select concat('We have ', count(*), (case when gender='m' then ' boys!' else ' girls!' end)) as 'Gender information' from modul group by gender;


select concat('This is ', name, (case when gender='m' then ', he' else ', she' end), ' has email ', email) as 'info' from modul;
```
