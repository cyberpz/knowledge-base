
## Clone repo
git clone <repo>

## create VirtualHost
# write in site-available (see Tech/Unix/Install VirtualHost)
a2ensite <file.conf>
systemctl reload apache2

# SSL Certificates
## if certbot not installed (see Tech/Unix/Install Certbot)

# PHPmyadmin
echo "deb http://ftp.debian.org/debian unstable main contrib" > /etc/apt/sources.list.d/debian.list
apt update
apt -y install phpmyadmin php-mbstring php-gettext

