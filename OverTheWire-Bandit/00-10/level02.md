
Goal: Retrieve password from "-" file in home directory

Commands Used:
  - ```ls``` to list the file names in the directory
  - ```cat``` to read the contents of the file holding the password

Procedure:
  - I immediately opted to check for the files I was given to work with using ```ls```, and found only one file named ```-```.
  - First,  I simply used the ```cat``` command to attempt to read the contents, but this was unsatisfactory use of the syntax, and the shell assumed I was still writing out my entire command. Doing so resulted in every input of mine being repeated, echoed, back to me. This was my first time experiencing this mysterious event.
  - Having studied the additional reading material, I corrected my error and retrieved the password.

Learnings:
  - Looking into it online, I realised what the issue was, and understood that simply pressing ```ctrl+c``` would fix this issue.
  - I learned from the additional reading material provided that a single ```-``` is understood by linux as the precedence of a function or command, and that I had to write ```./``` before the dash to read the file's contents

Conclusions: Completed level 02 successfully.
