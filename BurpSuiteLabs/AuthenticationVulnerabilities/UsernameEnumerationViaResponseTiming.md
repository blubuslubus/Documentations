## Lab: Username enumeration via response timing

Difficulty: Practitioner

Procedure:
  - We are given a set of valid credentials. Experimenting around with them, we find that the workflow is simple. Check for the username, and if the username exists then and only then check for the password. If the password is a long set of gibberish (incase of a valid username), then response time is noticably higher.
  - This information is crucial. First, we can proxy the POST request and send it to intruder. Now then, this is a good palce to use pitchfork attack, where we can select mutliple aspects of the request to iterate and alter.
  - Also, `X-Forwarded-For` header can be taken advantage of here, so include it and set its value to any number for now. Now set both this value and the username as iterables by adding $ sign, and insert the username wordlist as the payload for username, and `number` type payload for the header with a list of atleast 100 numbers.
  - Simply run the attack and sort the responses by response time. Notice the one that is considerably higher than the others, the username related to the highest response time is the username we attack.
  - Now do the same thing with the password wordlist payload as done often times else, and the lab is cleared.

Status: Solved

<img width="935" height="177" alt="image" src="https://github.com/user-attachments/assets/571cd68d-68a9-4d1b-81f3-5ffac40d6f07" />

