
Goal: Find the right input which gives the output "Good game", i.e. the flag.

Commands used:
  - `ltrace`

Procedure:
  - First I used `strings` on the executable, which wasn't very useful.
  - Then I decided to execute it to see what I have to work with. I know that normally, executing random stuff is dangerous, but since this is from THM I have some trust going forward.
  - Executing it, I realised I could probably see the underlying comparison checks using ltrace again, so I executed it once again with `ltrace`, and gave a random input.
  - On the last line, I find the string that is actually used for comparing, and this is the flag.

Learnings:
  - Creative ways of setting up authorization, but not effective.
  - Practice of `ltrace`.
