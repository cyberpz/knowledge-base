I used to lunch personal scripts on Tmux, but it has a lot of vulnerabilities, so i had to find a simple way to stay safe and lunch anything on detached mode, so that when the ssh session is terminated the execution won't block nor stop. 

```sh 
# Fist way
setsid script.sh >/dev/null 2>&1 < /dev/null &
```

```sh
# Second way
nohup script.sh </dev/null &>/dev/null &
```