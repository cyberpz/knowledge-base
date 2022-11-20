
# HTTPD path
cd /etc/httpd/conf.d

# Aggiungi un nuovo virtual host
vim oraristp.conf

# Prima di lanciare certbot
# Registra il sottodominio a DNS 
# quindi poi lancia:
certbot --apache
