
Goal: Complete the room.

Link [https://tryhackme.com/room/somesint]

- Task 1:-

  Q1: Understand the flag format.
  A1: Join the room and clear Task 1

- Task 2:-

  Q: Who hired you?
  A: Read the given background information to find the answer. It is a singular letter which follows after the flag format.

  Q: Who are you investigating? (ks{firstname lastname})
  A: Same as the previous answer, read the given background information.

- Task 3:-

  Q: What is Thomas' favorite holiday?
  A: Looking up his online handle, we find 2 relevant accounts, on Twitter/X and Reddit. I found the answer to this in the Bio (or About Me section) of his Twitter/X account.

  Q; What is Thomas' birth date?
  A: His birthday post can be found on his Reddit account. Do note, the format is MM-DD-YYYY which is not specified. Also in certain timezones, Reddit may show date of post to be 1 day ahead of the date that the room asks of you.

  Q: What is Thomas' fiancee's Twitter handle?
  A: On his Twitter account, he has replied to a picture of a cat that his fiancee had posted. Find her account there.

  Q: What is Thomas' background picture of?
  A: His background picture (of his profile on Twitter/X) is asked. This happens to be the same person he has mentioned in his Bio/About me.

- Task 4:-

  Q: What was the source module used to find these accounts?
  A: Follow the walkthrough given to install the required  tools. Look up the username (in quotes), and in one of the results you will find the answer when you click Browse -> Account on External Site.

  Q: Check the shadowban API. What is the value of "search"?
  A: The result of the link that led to the shadowban.eu seemed to be dead, but it felt uncanny due to the message on it. Anyway, plugging it into the Wayback Machine (say it with me, we love the internet archive and wayback machine!), I found the answer.

- Task 5:-

  Q: Where did Thomas and his fiancee vacation to?
  A: On his fiancee's handle, we can find the image of the location with a caption about the vacation. This image, through a reverse image search, tells us the location.

  Q: When is Francesca's Mother's birthday? (without the year)
  A: On his fiancee's handle, we can find a post wishing about a festival and her mother a happy birthday.

  Q: What is the name of their cat?
  A: The little furball has a dedicated post with their name on his fiancee's handle, which he has reposted.

  Q: What show does Francesca like to watch?
  A: Theres a post about this, with a hashtag.

- Task 6:-

  Q: What is the name of Thomas' coworker?
  A: On old reddit (with the wayback machine), we can see a coworker reply on his birthday post. Their username seems to have both names, and as we have to submit first name and last name both, we can reverse the order of the name and check.

  Q: Where does his coworker live?
  A: The coworker's reddit profile has an instance of mentioning their country in a post, and the state/city in their bio.

  Q: What is the paste ID for the link we found?
  A: This one takes a little time. I went back into the wayback machine and dug around for suspicious links he may have posted (the question does not do a very good job at giving context), but once we find it, the flag is the string at the end of this link.

  Q: Password for the next link?
  A: With no other leads, I clicked the link, which luckily was safe. Viewing in the wayback machine, we can find a Ghostbin entry, that basically is a threat to expose Thomas and his "mistress". Things are getting *interesting* here. Anyway this also contains the password asked of us so there's that.

  Q: What is the name of Thomas' mistress?
  A: Since we have the next link, we can just copy paste it. However, as I learned first-hand just now, we also have to add `/<password>` to the end of the link, so do that. 

  Q: What is Thomas' Email address?
  A: We find the answer in the same note.

Completed! This was very entertaining. Though marked intermediate, I did not find much challenge in this room. Perhaps because I did not have a lot of new things to learn in this room, and am a little comfortable using some of these OSINT tools now. Very fun and engaging nonetheless!
