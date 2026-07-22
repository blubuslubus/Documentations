
Goal: Find the Password to the executable, and find the Flag

Commands used:
  - `strings`

Procedure:
  - I am aware that the `strings` command extracts human-readable text (by default, atleast of length 4) without really committing to execution. This helps us read some content of the code if we happen to be lucky, or if we know some human-readable or predictable string is longer than the specified length (or default length of 4).
  - Simply running `strings` against the executable, I find the password hidden in plain sight (not really hidden).

Learning:
  - Practice using `strings`.
