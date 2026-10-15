## Hacker Holidays · The Byte Lotus Hotel

The Byte Lotus Hotel is a fictional resort featured in TryHackMe's Hacker Holidays 2026 cybersecurity event.

## Day 0 - The Brochure

Link: https://tryhackme.com/room/hh-thebrochure-081f3e36

  - Download the Task Files and extract, out comes the brochure attachment.
  - Put the image through reverse search engine and lookup the social media account that comes up.
  - Try finding accounts related, perhaps following or followed by this account.
  - On one such account, there are 3 parts of a mysterious hash, specifically base64.
  - Run it through cyberchef's From Base64 and out comes the flag.

Status: Completed

https://tryhackme.com/room/hh-thebrochure-081f3e36?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=686698db83d9427d09bd767b

## Day 1 - Arrival

Link: https://tryhackme.com/room/hh-theconciergeknows-2d7eb4d9

  - Open up the ai agent to talk to.
  - Try your methods first, but the simple solution is to make the agent believe you are already someone it knows. Rather, you are already someone who has escalated privileges and access.

Status: Completed

https://tryhackme.com/room/hh-theconciergeknows-2d7eb4d9?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=686698db83d9427d09bd767b

## Day 2 - Room 404

Link: https://tryhackme.com/room/hh-room404-804573bf

  - The website (given ip hosted on port 8080) seems to barely function. No button works, and the websites source code is a dead end too. So I opted to enumerate through common directories with gobuster. Found ```.git```.
  - I opted to donwload the git onto my machine and restore the working tree. A Readme.md is among some of the files recovered, reading which gives us the flag.

Status: Completed

https://tryhackme.com/room/hh-room404-804573bf?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=686698db83d9427d09bd767b

## Day 3 - Complimentary

Link: https://tryhackme.com/room/hh-room404-804573bf?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=686698db83d9427d09bd767b

  - 


