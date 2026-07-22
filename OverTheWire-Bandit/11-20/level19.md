
 Goal: To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

 Commands used:
   - ```ls```
   - ```clear```

Procedure:
  - After reading up setuid and understanding how users can temporarily perform tasks with the permissions of another user, I understood we had to cosplay being bandit20 for a bit.
  - I decided using ```bandit20-do``` and reading ```bandit20``` to find the password. This was a mistake, and filled my terminal with a bunch of gibberish. I love our handy ```clear```.
  - I then learned with the power of internet, that we have to specify the full directory and file path to bandit20 which housed the password. In doing so, I found the password.

Learnings:
  - Temporarily using privileges of another user or owner of a file to access it and use their permissions.


   
