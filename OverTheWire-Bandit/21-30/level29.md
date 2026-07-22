
Goal: There is a git repository at ssh://bandit29-git@bandit.labs.overthewire.org/home/bandit29-git/repo via the port 2220. The password for the user bandit29-git is the same as for the user bandit29.

Commands used:
  - ```ls```.
  - ```cd```.
  - ```git branch```.
  - ```cat```.
  - ```git checkout```.
  - ```git log```.

Procedure:
  - Same stuff as the previous couple levels, but this time we have to deal with branches.
  - checking for all the ```git branch```, we see a bunch of branches.
  - Snooping around a little, and messing with some of the previous versions of the ```git log```, we eventually find the password openly.

Learnings:
  - Practice working with different branches, and versions simultaneously.
