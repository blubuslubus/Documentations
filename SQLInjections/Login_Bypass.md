Lab: SQL injection vulnerability allowing login bypass

Difficulty: Apprentice

Procedure:
  - When attempting to login, we are asked to input our username and password in a field. The exploit lies here, as in our username we can simply input our injection commands `administrator'--`. In systems, the first account that usually exists is the admin account.
  - In doing so, the sql command is evaluated with `username = administrator` and everything after gets ignored due to `--`.

Status: Solved
<img width="934" height="177" alt="image" src="https://github.com/user-attachments/assets/05a342f8-7f52-44bb-b053-d6286a3bc86c" />
