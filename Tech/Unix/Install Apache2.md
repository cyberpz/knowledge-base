# For Debian distros

```sh
apt update;
apt install apache2 curl git;
apt install php libapache2-mod-php;
```

### CLI commands for IPTABLES
```sh
/sbin/iptables -I INPUT -p tcp --dport 80 -m state --state NEW,ESTABLISHED -j ACCEPT
/sbin/iptables -I INPUT -p tcp --dport 433 -m state --state NEW,ESTABLISHED -j ACCEPT
```

### Manual add IPTABLES
```sh
vim /etc/sysconfig/iptables
```

Add these to the File
```sh
-A INPUT -m state --state NEW,ESTABLISHED -p tcp --dport 80 -j ACCEPT
-A INPUT -m state --state NEW,ESTABLISHED -p tcp --dport 443 -j ACCEPT
```
```sh
vim /etc/apache2/apache2.conf
```

append this:
```txt
"<FilesMatch \.php$> SetHandler application/x-httpd-php </FilesMatch>"
```

go run:
```sh
systemctl restart apache2
```
