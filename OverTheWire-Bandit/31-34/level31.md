
Goal:There is a git repository at ssh://bandit31-git@bandit.labs.overthewire.org/home/bandit31-git/repo via the port 2220. The password for the user bandit31-git is the same as for the user bandit31.

Commands used:
  - `ls`
  - `cat`
  - `git` commands

Procedure:
  - Reading the README.md after cloning tells us directly to push key.txt.
  - Doing so, we realise that it is a part of `.gitignore`, so we have to force the push.
  - This is simply done by adding a `-f` flag to force the push, and we get the password.

Learnings:
  - Practice of git commands.
