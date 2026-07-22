
Goal: After all this git stuff, it’s time for another escape. Good luck!

Commands used:
  - `ls`
  - `cat`

Procedure:
  - It is easy to observe that whatever we input into the terminal gets capitalised, so our inputs are overwritten in the shell.
  - To bypass such a conflict, we can input $0 which does not get capitalised for the terminal to evaluate, but then allows us to use our commands as normal without capitalisation.
  - This allows us to simply retrieve the password.

Learnings:
  - Purpose and evaluation of $0 to escape a sort of softlock condition set by the current terminal.
