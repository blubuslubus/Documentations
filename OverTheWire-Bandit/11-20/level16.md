
Goal: To retrieve password of next level by submitting the password of the current level to a port on localhost in the range 31000 to 32000 listening and speaking SSL/TLS.

Commands used:
  - ```nmap```
  - ```touch```

Procedure:
  - I used ```map -p 31000-32000 localhost``` and found 5 open ports.
  - This time I opted to use openssl to get familiar, and using it on the right port i found a private sshkey.
  - This time using touch, I created a temp privatefile with the key, changed its permissions as before and used it to login to bandit17
  - Then simply using ```cat``` I could retrieve the password for bandit17.

Learnings:
  - Using ```nmap```, powerful tool.
  - Practicing using private ssh keys.
