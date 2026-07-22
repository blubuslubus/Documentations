
Goal: To retrieve the password of next level by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.

Commands Used:
  - ```ncat```
  - ```cat```

Procedure:
  - To use the SSL/TLS encryption, we simply used ```ncat --ssl```.
  - Piping the password of the current level to port 30001 on localhost with ```ncat --ssl``` as opposed to ```nc```, we can use the SSL/TLS encryption.

Learnings:
  - Purpose of TLS, or as called SSL despite SSL being discontinued in 2015 but being catchy.
  - Usage of the encryption.
