Lab: SQL injection vulnerability in WHERE clause allowing retrieval of hidden data.

Difficulty: Apprentice

Procedure:
  - I spent a short while simply learning about BurpSuite at first, and opted to use my own browser for the tasks as opposed to using the BurpSuite in-built browser.
  - This task mostly helped me in understanding the usage of BurpSuite, I am a little familiar with SQL already.
  - During the injection, I made an error of simply commenting out anything in the commond that follows ```'Gift'```. While this can yield the desired results sometimes, the more efficient and suitable method for such cases is to include an `OR` followed by a comparison that is always `TRUE`, such as `1=1`.

Status: Solved
<img width="941" height="203" alt="image" src="https://github.com/user-attachments/assets/9e273ce1-6cf2-415b-90e6-e70a7367cc43" />
