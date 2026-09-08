Lab: Username enumeration via account lock

Difficulty: Practitioner

Procedure:
  - I'll be honest, this particular lab was very annoying and bothersome to work with on the community edition of Burpsuite.
  - We are expected to enumerate through every username 5 times in succession, and the valid username will eventually show us an error stating something similar to "Try again after 1 minute(s)."
  - Except that attacks are throttled heavily on the community edition.
  - I decided to work around this by feeding the payload configuration with each individual username 5 times, and only computing an attack with 100 payloads at a time.
  - This took extra time and effort, and is way easier on the Professional version of Burpsuite, but this Lab helped me practice some patience too. Oh well~

Status: Solved!

<img width="835" height="172" alt="image" src="https://github.com/user-attachments/assets/010b1617-4552-4ea9-9394-a567c15c9edf" />
