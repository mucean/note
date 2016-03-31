## 避免软码
### 方法一：Dump&Reload
    shell> mysqldump -u root -p -t --skip-set-charset --default-character-set=utf8 test charset_test_latin1 > data.sql
    shell> mysql -uroot -p -e 'create table charset_test_latin1 (id int primary key auto_increment, char_col varchar(50)) charset = utf8' test
    shell> mysql -uroot -p  --default-character-set=utf8 test < data.sql

### 方法二：Convert to Binary & Convert Back
    mysql> ALTER TABLE charset_test_latin1 MODIFY COLUMN char_col VARBINARY(50);
    mysql> ALTER TABLE charset_test_latin1 MODIFY COLUMN char_col varchar(50) character set utf8;

博客链接<http://cenalulu.github.io/mysql/mysql-mojibake/>
