
Goal: Find the password/flag.

Commands used:
  - `strings`.
  - `grep`.
  - `ltrace`
  - `r2` - radare2

Procedure:
  - Using `strings`, I decided to use `grep` looking for phrases like "pwd", "pass", etc, to no avail.
  - Using `ltrace`, I thought of trying to find the password during a check inside a function. However, the author used another check inside another function which I can not view using ltrace.
  - I opted to use radare2, as it was recommended in the challenge, and took a while to learn it.
  - At first I tried using V mode, but it was all too much for me.
  - In the end, I realised that the actual password check is done bit-by-bit, in the secondary function check, and found the password there.

Learnings:
  - I felt understanding of a case where password checks can be layered in security, quite literally.
  - Usage and purpose of radare2.
