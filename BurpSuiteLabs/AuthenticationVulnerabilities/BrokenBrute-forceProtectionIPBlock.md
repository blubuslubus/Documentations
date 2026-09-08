## Lab: Broken brute-force protection, IP block

Difficulty: Practitioner

Procedure:
  - To be straightforward, a little experimenting around shows that `X-Forwarded-For` header is supported.
  - I utilised this, and used pitchfork attack to enumerate through the username list, as well as password.
  - The counter on the header was also set to change, in order to emulate sending out a different IP to protect against IP block.

Status: Solved!

<img width="799" height="183" alt="image" src="https://github.com/user-attachments/assets/74c39dfe-a41d-4f3d-863e-ce26769c4e09" />
