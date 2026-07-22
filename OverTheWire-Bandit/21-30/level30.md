
Goal: There is a git repository at ssh://bandit30-git@bandit.labs.overthewire.org/home/bandit30-git/repo via the port 2220. The password for the user bandit30-git is the same as for the user bandit30.

Commands Used:
  - ```cd```
  - `cat`
  - `git clone`
  - `git branch`
  - `git log`

Procedure:
  - Doing the same procedure as the past few levels did not yield any promising leads. I could not find anything to exploit
  - As suggested, learning about ```tag``` was the solution to this level.
  - Using `tag` showed something named "secret", and contained the password.

Learnings:
  - Usage and purpose of `tag`
