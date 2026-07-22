
Goal: find flag/password.

Commands used:
  - ltrace

Procedure:
  - This time using `strings`, some of the text reads out that they used strcmp. This is my first time hearing about strcmp, finally something new!
  - Looking into it for a bit, I found that ltrace can be used to trace and understand flow of control in a compiled binary executable, like in my case, apart from other uses. Powerful!
  - Using ltrace to execute the file, and supplying a random password, we can see the system comparing our password (which is how strcmp works) to the other string (which is the real password). This way we can find the password:

Learnings:
  - `strcmp` is a C/C++ library standard function that compares two strings to see if they are identical.
  - `ltrace` can be used to debug or understand flow of control in compiled executables, finding memory leaks, etc.
