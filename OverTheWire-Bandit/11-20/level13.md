
Goal: To retrieve the password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14.

Commands used:
  - ```ls -a```, to list all files and directories.
  - ```cat```, to read contents of the file.
  - ```scp```, to securely send the file to my pc.

Procedure:
  - Most of the trial and error involved fumbling with incorrect ports, permissions, and password confusions. At one point I was convinced I needed a linux environment (I am on windows currently).
  - In the end all I had to do was to ```scp``` the ```sshkey.private``` onto my computer, and login to the user with it.

Learnings:
  - Usage and purpose of ```scp```.
  - A lot about file permissions.
  - A lot more detail about ```ssh```.

Conclusion: Completed Level 13 successfully.
