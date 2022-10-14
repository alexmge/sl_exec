# sl_exec
Just an sl script to prank people who forgot to i3lock

Run this command in a terminal downloads the script `sl` in the current directory and run it in an infinite loop while disabling pretty much any possible interruption signal.

```bash
 curl -s https://raw.githubusercontent.com/alexmge/sl_exec/main/sl -o sl && chmod +x sl && trap '' seq 1 20; stty -ixon;  while true; do ./sl; done
```

*Keeping the whitespace in front of the command is important as it prevents the command from being added to the logs !*
