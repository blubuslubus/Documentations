## Lab: 2FA broken logic

Difficulty: Practitioner

Procedure:
  - I opted to recon with the given account credentials, and in doing so we can notice a few alarming things.
  - Firstly, `verify` is used to determine which user's account is being accessed.
  - Secondly, the cookie assigned to a particular session with valid username & password is available to retrieve quite easily.
  - And lastly, `mfa-code` is the parameter which submits the otp code for the actual 2FA method.
  - Since the session-id/cookie is readily available for us, we can do a little replacement. Simply login with our given credentials, but through the intercept on BurpSuite, alter the request to be send from account `carlos` instead of `wiener` by replacing the value of the `verify` parameter. This tells us a 2FA code is generated for the account `carlos`.
  - Now, submit an invalid 2FA otp code, since we do not yet know what the code is, and intercept it.
  - Use Sniper attack tool and set the `mfa-code` parameter as the payload, and run the attack to bruteforce the 4-digit code.
  - The correct response (302) can be loaded into browser and the lab is solved.

Status: Solved!

<img width="442" height="160" alt="image" src="https://github.com/user-attachments/assets/13456cc2-11da-4009-a9d9-52bc9f8d0df3" />
