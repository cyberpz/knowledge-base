
# clone the repo
cd /etc/apache2/sites-available
echo "
<VirtualHost *:80>
ServerAdmin webmaster@localhost
DocumentRoot /var/www/html/xxx
ServerName xxx.peppuz.it 
RewriteEngine on
RewriteCond %{SERVER_NAME} =xxx.peppuz.it
RewriteRule ^ https://%{SERVER_NAME}%{REQUEST_URI} [END,NE,R=permanent]
</VirtualHost>" >> temp.conf;

certbot --apache -d xxx.peppuz.it # per ogni dominio/subdomain
