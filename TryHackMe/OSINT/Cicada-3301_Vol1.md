## Cicada 3301 Vol:1 

Link: https://tryhackme.com/room/cicada3301vol1

## Procedure:

#### Task 1:
  - Download the material

#### Task 2:
  - Analyze the audio in Sonic Visualizer, create an audio spectrogram of it.
  - The spectrogram reveals a qr-code, which leads us to a pastebin link with an encrypted passphraes and key.

#### Task 3:
  - Find what encryption was used (try using ```hashid``` in bash).
  - Decrypt the passphrase and the key. Notice that the passphrase even now seems to be encrypted in another cipher.
  - The hint tells us about a certain French Diplomat, so the cipher used must be Vigenere cipher.

#### Task 4:
  - We are asked to use steg-tools, and the one that first and immediately comes to my mind is steghide.
  - I recommend using steghide too, and the passphrase is the one after decrypting the Vigenere cipher.
  - Doing so we can obtain an imgur link.

#### Task 5:
  - For this one, we have to use one of the steg-tools used in the original Cicada3301.
  - The list can be found online, but for the sake of this room, we are to use Outguess.

#### Tasl 6:
  - The txt file obtained contains a hash and the key to a book-cipher.
  - The hash can be cracked through an online lookup (SHA512 being reverse engineered is near impossible).
  - The hash leads us to the book (in our case, document) on which we use the key provided, and it leads us to a shortened link that finally takes us to a song on Soundcloud.

## Conclusion:
  - Solved Successfully! I enjoyed this room especially the end. Good song.

  - https://tryhackme.com/room/cicada3301vol1?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=686698db83d9427d09bd767b
