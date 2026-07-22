
Goal: Complete the room.

  Q: Which VPN service was used to send the anonymous email from the .eml file?
  A: Analyzing exhibit_a.eml, we find the sender's IP to be `193.32.249.132`, and looking this up on WHOIS, we find which company this IP belongs to. Researching about this company, we find they also provide VPN services to another VPN company, this VPN company is the answer.

  Q: What is the full street address of the petrol station where the missing vehicle was last seen?
  A: The picture `exhibit_b.png` can give vital information about the name of the gas station. A location mentioned in the memo can give a hint as to the location where the target gas station is asked of us to find.

  Q: At what time did the suspicious action take place in the route planning system on March 25th, 2026?
  A: Since we are asked to report the time a suspicious activity took place in the system, a logging system would be beneficial to have. We do have a logging system, called `access_log.csv`, reading which we find a suspicious activity reported as exporting confidential data. This timestamp is the required answer.

  Q: What is the employee ID of the person who sent the anonymous email?
  A: The anonymouse employee said they were working that night, so the logs must reflect this. We can observe in `access_log.csv`, that right after the "Export" entry, there is another entry that same night with the employee id that is the answer. This is also the last entry for the night, as the next log reflects activity on the next day.

  Q: What is the employee ID of the employee responsible for leaking the shipment details?
  A: This is simply the employee ID of the employee responsible for exporting (and leaking) the route.

  Q: What is the leaker's full name?
  A: We already have the burner-email. its mentioned in   `comms_export.csv`. Using this in something like epieos.com (google account info), we can find a google review about the same gas station, with the full real name of the leaker.


Learnings:
  - A lot of information can be extracted from email logs and headers, keep them handy.
  - Epieos.com, can be useful at times.
  - Logs can be your best friend. 

Completed! this was a pretty fun experience, I really learned a lot of new things in this one. The difficulty really felt up a notch, just what I liked.
