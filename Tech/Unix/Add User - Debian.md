New user:
```sh
adduser <username>
```

Add to sudoers
```sh
usermod -aG sudo <username>
```

Check if included in sudoers
```sh
getent group sudo
```

