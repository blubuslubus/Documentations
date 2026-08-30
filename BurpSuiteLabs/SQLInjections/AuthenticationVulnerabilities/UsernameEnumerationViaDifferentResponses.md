## Lab: Username enumeration via different responses

Difficulty: Apprentice

Procedure:
  - The Username and Password wordlist is provided to us. I turned on intercept mode and send a sample POST request with guessed credentials on the lab-website provided.
  - Now, check the HTTPS POST request and highlight the sample username you used, it would look like ```username=<sampleuser>```, highlight ```<sampleuser>``` and send it to intruder.
  - Select Sniper attack type, and paste the given username wordlist under the Payload configuration and begin attack. In doing so, we have effectively guided BurpSuite to send requests with all the words from the wordlist as usernames, and now we will look for any record of response that is different from the rest since it will have a different error response, maybe some error like "incorrect password" for a username that exists, instead of the generic "username not found" for a non-existing user.
  - Sure enough, once we find the correct username, we repeat the process with the correct username and a random password, and try to find the unique response that stands out, either by the length of the response or the status code.
  - In this way, we can narrow down the username and its password to gain authentication through username enumeration.

Status: Solved

<img width="1091" height="201" alt="image" src="https://github.com/user-attachments/assets/94f5da0c-65e8-4c9a-a813-e4321331e5df" />








