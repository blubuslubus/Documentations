
Goal: A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

Commands used:
  - ```ls```
  - ```cd```
  - ```cat```

Procedure:
  - Seeing a new command, ```cron```, I read its manpages and tried using it, but it only threw errors.
  - Changing directory to the given directory and reading ```cronjob_bandit22``` with ```cat```, led to another directory containing a ```.sh``` file.
  - Reading the ```.sh``` file reveals that the cronjob writes the required password to a directory shown, and simply using ```cat``` on the directory gives us the password.

Learning:
  - Periodic jobs and tasks can be done using cronjobs, and the jobs can be traced to some extent.
