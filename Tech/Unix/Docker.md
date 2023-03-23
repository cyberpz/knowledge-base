# Install 
https://docs.docker.com/engine/install/debian/
🤍


# Remove

jesus christ, i've been struggling with removin docker from debian.
Here's few commands to purge it from debian.

```sh
# identify
dpkg -l | grep -i docker 

sudo apt-get purge -y docker-ce docker-ce-cli
sudo apt-get autoremove -y --purge docker-ce docker-ce-cli

# in case of more versions
sudo apt-get purge -y docker-engine docker docker.io docker-ce docker-ce-cli sudo apt-get autoremove -y --purge docker-engine docker docker.io docker-ce

# Remove all the Docker related files
sudo rm -rf /var/lib/docker /etc/docker 
sudo rm /etc/apparmor.d/docker 
sudo groupdel docker 
sudo rm -rf /var/run/docker.sock

# Remove network bridges
ifconfig docker0 down
brctl delbr docker0
```