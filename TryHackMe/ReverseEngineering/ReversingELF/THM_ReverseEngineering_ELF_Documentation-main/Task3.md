
Goal: Find the flag/password.

Commands used:
  - `strings`
  - `echo`
  - `base64 -d`

Procedure:
  - This time, using `strings` gave a lot more information than I expected.
  - Some of the text clearly looked encoded at first, and observing it further I thought it must be base64, because it seems to be a pattern to introduce it amongst beginners. Nice.
  - This text, I piped through `base63 -d` to decode and the password/flag is right there.

Learnings:
  - Practice finding and using base64 encoded text.
