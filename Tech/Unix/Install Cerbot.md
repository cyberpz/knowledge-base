# Install Certbot for HTTPS requests

## Via SNAP
```sh
apt install snapd
snap refresh core
snap install --classic certbot
ln -s /snap/bin/certbot /usr/bin/certbot 

reboot;
```
#### ready to clone repo and install Virtual host install SSL certs 

## Via APT
```sh
apt install certbot python-certbot-apache
```

Test it!
