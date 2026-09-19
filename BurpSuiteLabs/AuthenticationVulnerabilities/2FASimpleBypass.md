## Lab: 2FA simple bypass

Difficulty: Apprentice

Procedure:
  - Given my own account's credentials, I opted to first login with it and observe the environment after we are logged in. Immediately in the lab, we can find a new option to view mails we get.
  - We use this mail client simulator to get our otp for the 2 Factor authentication done for our account in order to have access of the account. 2 FA or 2 Factor Authentication basically means the use is asked and checked for authentication by 2 different types of authentications, often these are simply a password that user remembers and an authentication tool like Google Authenticator working in pairs.
  - Keen observation can note a peculiarity in the url of the site once we are logged in. there is `/my-account` at the end of the url, which could simply mean that we are allowed access of the account after the password check, making the second factor authentication check useless.
  - Simply adding `/my account` at the end of the url's `.net` will allow us full access of this compromised account.

Status: Complete
