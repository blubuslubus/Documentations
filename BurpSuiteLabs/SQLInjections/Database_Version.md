Lab: SQL injection attack, querying the database type and version on Oracle

Difficulty: Practitioner

Procedure:
  - Immediately looking at the different categories of items available to us, we can tell that this is our entry towards the injection.
  - Using `UNION`, I tried to get the version, but this resulted in an internal server error as the number of columns to retrieve I provided was only one (banner), while the command checks for 2.
  - I rectified this by simply adding `null` column to the check, and solved the task.

Status: Solved
<img width="940" height="221" alt="image" src="https://github.com/user-attachments/assets/579f33cd-1f1e-4962-b863-b42db8579e9e" />
