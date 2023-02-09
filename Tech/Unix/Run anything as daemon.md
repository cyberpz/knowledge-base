#DEBIAN 
To run it as a full daemon from a shell, you'll need to use setsid and redirect its output. You can redirect the output to a logfile, or to /dev/null to discard it. Assuming your script is called myscript.sh, use the following command:

```
setsid myscript.sh >/dev/null 2>&1 < /dev/null &
```

This will completely detach the process from your current shell (stdin, stdout and stderr). If you want to keep the output in a logfile, replace the first `/dev/null` with your /path/to/logfile.

You have to redirect the output, otherwise it will not run as a true daemon (it will depend on your shell to read and write output).

[Source](https://stackoverflow.com/questions/19233529/run-bash-script-as-daemon)