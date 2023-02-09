# Install a classic database for domestic use
apt update
apt install mariadb-server
mysql_secure_installation

## (Optional) Adjusting User Authentication and Privileges
mysql

MariaDB [(none)]> GRANT ALL ON *.* TO 'admin'@'localhost' IDENTIFIED BY 'password' WITH GRANT OPTION;

MariaDB [(none)]> FLUSH PRIVILEGES;

MariaDB [(none)]> exit ;

# IMPORT existing dump 
mysql -u admin -p
CREATE DATABASE new_database;
mysql -u admin -p new_database < data-dump.sql

