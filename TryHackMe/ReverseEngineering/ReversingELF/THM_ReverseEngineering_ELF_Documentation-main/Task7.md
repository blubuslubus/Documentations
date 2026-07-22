
Goal: Find the flag/password.

program used:
  - ghidra

Procedure:
  - this was hard. My first time using ghidra.
  - I got tired of the loops i was going in using terminal commands, so I decided to try decompiling the executable and read the code, which is much easier.
  - I decided to use ghidra, spent a good time learning the ropes.
  - Then I got too caaught up in the function `giveFlag`, where I thought I was going the right way for a while, but it was such a cumbersome task it just had to be the wrong approach.
  - Going through every function, I noticed something eyecatching in the "main" function. go figure.
  - In it, I find a unique hardcoded check, to check for a specific input instead of the usual 1, 2 or 3 that the program asks of you.
  - Using this specific input, the flag is revealed to us.

Learnings:
  - Hands-on reverse engineering with Ghidra.
