
Goal: A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.
You do not need to create new connections each time

Commands used:
  - ```nc```.
  - ```chmod +x```.
  - ```mkdir```.
  - ```cd```.
  - ```ls```.
  - ```grep```

Procedure:
  - Using ```nc``` to connect to the listening port, the clear solution was to simply bruteforce as the goal suggests.
  - AdHoc, I created a simple ```for loop``` script to go through all digits from 0000-9999 and grep-ing when asked for the credential.

Learnings:
  - Further usage and practice of scripting.
  - Bruteforcing hands-on experience
