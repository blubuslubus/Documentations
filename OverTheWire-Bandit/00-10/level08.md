
Goal: Retrieve the password that is stored in the file data.txt and is the only line of text that occurs only once.

Commands used:
  - ```ls -a```, to list all files and directories.
  - ```sort```, to sort output in ascending order from ```data.txt```.
  - ```uniq -u```, to retrieve the only unique line (occurs only once).

Procedure:
  - I first attempted to use ```uniq data.txt``` but immediately realised this is incorrect.
  - Realising my mistake and using the additional reading material, I decide to sort the data to make it productive for ```uniq``` to compare.
  - This is also a little far from the correct answer. Realising this mistake, I added ```-u``` flag to ```uniq``` and found the password.

Learnings:
  - Purpose and usage of ```|``` pipe.
  - Purpose and some usages and flags of ```uniq```.
  - ```uniq``` is often used in pairs with ```sort```.

Conclusion: Completed Level 08 successfully.
