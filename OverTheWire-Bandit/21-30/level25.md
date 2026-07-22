
Goal: Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.

Commands used:
  - ```cat```.
  - ```grep```.

Procedure:
  - From our experience on bandit until now, we know where all passwords for the users are stored. ```cat /etc/passwd```, we can see user bandit26 uses the shell ```/usr/bin/showtext```.
  - The contents of this script tell us that a ```more``` command reads out the contents of file ```text.txt```, and an ```exit(0)``` follows.
  - What this means is, once the textfile's contents are all displayed, ```exit(0)``` is executed.
  - The simple bypass is to not let the contents be displayed, i.e. resize the terminal to a much smaller size.
  - In doing so, we have managed to not get kicked out of the logging immediately, but this is only half of the story. We now need to find the password.
  - As suggested, we will use vim. Vim has a command mode, so utilising the feature we set the scripts shell to /bin/bash which will allow us to login as bandit26.
  - Executing the script then will have us logged as bandit26, and the password is available too.

Learnings:
  - About the ```more``` command.
  - Further usage of vim
