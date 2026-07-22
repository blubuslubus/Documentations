
Goal: To find the password somewhere in the server that is owned by user bandit7, group bandit6, and is 33bytes in size.

Commands used:
  - ```ls``` to list files and directories.
  - ```cd``` to change directories.
  - ```find``` to find for file with target attributes.

Procedure:
  - Using ```cd``` to get into ```inhere``` folder I found using ```ls```, I am greeted with 20 folders which may hold the password.
  - Using ```find . -size 1033c ! -executable``` I found the exact file and directory.
  - Using ```cat```, I read the contents of the file and found the password.

Learnings:
  - Using the ```find``` command better with more of its flags.

Conclusion: Completed Level 06 successfully.
