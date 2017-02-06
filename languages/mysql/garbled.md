## 避免软码
要避免乱码，只要做到“三位一体”，即客户端，MySQL character-set-client，table charset三个字符集完全一致就可以保证一定不会有乱码出现了，如果出现乱码可以用以下方法解决
#### 方法一：Dump&Reload
    shell> mysqldump -u root -p -t --skip-set-charset --default-character-set=utf8 test charset_test_latin1 > data.sql
    shell> mysql -uroot -p -e 'create table charset_test_latin1 (id int primary key auto_increment, char_col varchar(50)) charset = utf8' test
    shell> mysql -uroot -p  --default-character-set=utf8 test < data.sql

#### 方法二：Convert to Binary & Convert Back
    mysql> ALTER TABLE charset_test_latin1 MODIFY COLUMN char_col VARBINARY(50);
    mysql> ALTER TABLE charset_test_latin1 MODIFY COLUMN char_col varchar(50) character set utf8;

博客链接<http://cenalulu.github.io/mysql/mysql-mojibake/>
