# Install a classic database for domestic use
```sh
apt update
apt install mariadb-server
mysql_secure_installation
```

### Define User and Privileges
```mysql
GRANT ALL ON *.* TO '<user>'@'localhost' IDENTIFIED BY '<password>' WITH GRANT OPTION;

FLUSH PRIVILEGES;

exit ;
```

# IMPORT existing dump 
```sh
mysql -u admin -p
CREATE DATABASE new_database;
mysql -u admin -p new_database < data-dump.sql
```

