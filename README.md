## 数据库
### 数据库备份与还原
- homestead 数控库的账号与密码
  ```
  账号：homestead
  密码：secret
  ```
- ubuntu系统中备份mysql
  - [table1 table2]省略则备份所有表
    备份输出也可以指定路径
    ```
    $ mysqldump -uusername -p dbname [table1 table2] > BackupName.sql
    ```
### mysql数据库基本操作
- 启用关闭数据库
  ```
  net start mysql_serverName  // 启用数据库服务器
  net stop mysql_serverName  // 关闭数据库服务器
  ```
- 登录与退出数据库
  ```
  mysql -uroot  -proot123  // -u用户名，-p密码，-V查看版本，-h主机地址
  exit | quit | \q   // 退出
  ```
- 显示数据库列表
  ```
  show databases;
  ```
- 删除数据库
  ```
  drop database dbname;
  ```