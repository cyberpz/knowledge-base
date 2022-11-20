# Install
apt update;
apt install apache2 curl git;
apt install php libapache2-mod-php;


# CLI commands for IPTABLES
/sbin/iptables -I INPUT -p tcp --dport 80 -m state --state NEW,ESTABLISHED -j ACCEPT
/sbin/iptables -I INPUT -p tcp --dport 433 -m state --state NEW,ESTABLISHED -j ACCEPT

# or Manual add IPTABLES
vim /etc/sysconfig/iptables
# Add these to the File
-A INPUT -m state --state NEW,ESTABLISHED -p tcp --dport 80 -j ACCEPT
-A INPUT -m state --state NEW,ESTABLISHED -p tcp --dport 443 -j ACCEPT

vim /etc/apache2/apache2.conf
# append this 
"<FilesMatch \.php$> SetHandler application/x-httpd-php </FilesMatch>" 

systemctl restart apache2


# Prepare Certbot for HTTPS
apt install snapd
snap refresh core
snap install --classic certbot
ln -s /snap/bin/certbot /usr/bin/certbot 

reboot;

# ready to clone repo and install Virtual host install SSL ... 
