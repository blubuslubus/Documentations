
Goal: To retrieve the password of next level by submitting the password of the current level to port 30000 on localhost.

Commands Used:
  - ```ls```
  - ```cd```
  - ```netcat``` or ```nc```, to connect to the specified port 30000 then pipe the password to it.

Procedure:
  - The previous level stated that the password is stored in ```/etc/bandit_pass/bandit14```, so a simple cat command can retrieve the password with this information.
  - Having retrieved the password from the given directory, as we are now logged in as bandit14, we simply submit this password to port 30000 using ```nc``` and get the password for next level.

Learnings:
  - Usage and purpose of ```nc```.
