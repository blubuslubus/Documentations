
Goal: There is a git repository at ssh://bandit28-git@bandit.labs.overthewire.org/home/bandit28-git/repo via the port 2220. The password for the user bandit28-git is the same as for the user bandit28.

Commands used:
  - ```git clone```
  - ```ls```
  - ```cd```
  - ```cat```
  - ```git log```
  - ```git show```

Procedure:
  - Doing the exact same steps as the previous level, we find the password is now modified, and to find it we would have to dig into previous versions of the file in hopes that the exposed password will be visible.
  - Running ```git log``` with the README.md file, we see all previous commits, with the id.
  - Using ```git show``` with the commit id of the latest commit before the one labelled with the message "fix info leak", we can read the password.

Learnings:
  - Reading version history and using the information to read old, edited information of commits on git.
