
## Clone repo
git clone <repo>

## VirtualHost
# write Virtual host in site-available (see Install VirtualHost)
a2ensite <file.conf>
systemctl reload apache2

# SSL Certificates
## if certbot not installed
apt install snapd
snap install core
snap install --classic certbot
ln -s /snap/bin/certbot /usr/bin/certbot
certbot --apache -d peppuz.it # per ogni dominio/subdomain


# PHPmyadmin
echo "deb http://ftp.debian.org/debian unstable main contrib" > /etc/apt/sources.list.d/debian.list
apt update
apt -y install phpmyadmin php-mbstring php-gettext

