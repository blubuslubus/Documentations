## Lab: Username enumeration via subtly different responses

Difficulty: Practitioner

Procedure:
  - Similar to the one before this, except this time before starting the first attack, go to settings and under Grep - Extract, click add and from a response, select the `Invalid username or password`. All other relevant settings will be auto-adjusted.
  - Now during an attack, a new column will show up, and analysing it will show that one of the responses is slightly different. This is our clue.
  - This indicates a small mistake made by the programmer, basically when the username is checked and found correct, password is checked, but the error message is slightly different from other responses.
  - Note of this username, and then simply enumerate through all passwords from the wordlist.

Status: Completed

<img width="1152" height="201" alt="image" src="https://github.com/user-attachments/assets/201afd0d-5f23-4815-8203-b66f636fc7a0" />
