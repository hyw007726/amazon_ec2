# ec2安装mysql (amazon linux)

1. yum install wget
2. wget 官方rpm
3. rpm -ivh rpm文件
4. yum install mysql-community-server
5. systemctl start mysqld
6. sudo grep 'temporary password' /var/log/mysqld.log 查看密码
7. mysql -u root -h localhost -p 登入
8. ALTER USER 'userName'@'localhost' IDENTIFIED BY 'New-Password-Here'; 修改密码，大小写+符号
