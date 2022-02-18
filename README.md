```sql
select concat('This is ', name, (case when gender='m' then ', he' else ', she' end), ' has email ', email) as 'info' from modul;
```
```sql
+------------------------------------------------+
| info                                           |
+------------------------------------------------+
| This is Vasya, he has email mmm@mmail.com      |
| This is Alex, he has email mmm@gmail.com       |
| This is Alexey, he has email alexey@gmail.com  |
| This is Helen, she has email hell@gmail.com    |
| This is Jenny, she has email eachup@gmail.com  |
| This is Lora, she has email tpicks@gmail.com   |
| This is Lera, she has email tpiffcks@gmail.com |
+------------------------------------------------+
```
```sql
select concat('We have ', count(*), (case when gender='m' then ' boys!' else ' girls!' end)) as 'Gender information' from modul group by gender;
```
```sql
+--------------------+
| Gender information |
+--------------------+
| We have 4 girls!   |
| We have 3 boys!    |
+--------------------+
```
