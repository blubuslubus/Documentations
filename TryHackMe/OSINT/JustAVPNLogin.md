## Name: Just a VPN Login

Link: https://tryhackme.com/room/justavpnlogin?vccr=1

## Procedure:

   Right as we start off, we can notice we have been provided with a threat intelligence database in the form of a static THM website, TryDetectThis. We will be utilising this throughout this room.
  - Question 1: Look up the ip address provided in the text of the room into the static website, and you will find a bunch of information. The AS# can be found in its midst.
  - Question 2: In the "File Relations" section you can find some interesting communications of the ip address.
  - Question 3: Looking up the hash on the static site, we can find the executable file's name in the File detail's basic properties.
  - Question 4: Scrolling down to vendor analysis and looking at Microsoft's entry will give you the clear answer.
  - Question 5: Find the malicious domain and run it through the static site to get its HTTP certificate. There you will find a list of "SUBJECT_ALTERNATIVE_NAMES" or the domains associated.
  - Question 6: Under "Detections and Reports"'s Yara rules, there is a link to a github repo by "kevoreilly", which leads directly to the Lumma. Read through the code and the answer is simply found.
  - Question 7: Look for a certain "Report" section on the static site.
  - Question 8: Answer is in the report, read the contents.
  - Question 9: Answer is in the report, read the contents.
  - Question 10: Answer is in the report, read the contents. Appendix C.

## Conclusion:

   Status: Completed
   
   https://tryhackme.com/room/justavpnlogin?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=686698db83d9427d09bd767b

   
