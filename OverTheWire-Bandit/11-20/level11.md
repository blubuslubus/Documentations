
Goal: To retrieve password  stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions.

Commands used:
  - ```ls -a```, to list all files and directories.
  - ```cat```, to read the contents of ```data.txt```.
  - ```man```, to understand the ```tr``` command.
  - ```tr```, to decode the rot13 encryption.

Procedure:
  - After finding ```data.txt``` through ```ls -a```, the contents seemed to be encrypted in some way (rot 13).
  - I was aware of this encryption method already, so reading on the ```tr``` command and its usage led me to figuring out the password.

Learnings:
  - Purpose and usage of ```tr```. It cannot be used independently, data has to be fed to it using pipe ```|```.

Conclusion: Completed Level 11 successfully.
