
Goal: There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

Commands used:
  - ```nc -l -p``` with specified port.
  - ```./suconnect```.

Procedure:
  - I opened two terminals, and on one I opened a remote server with ```nc``` listening to a port I specified.
  - On the other terminal, I sent a ```./suconnect``` request on the same port.
  - Then I matched passwords on both terminals, and got the password to the next level.

Learnings:
  - Listening to a specific port with ```nc```.
