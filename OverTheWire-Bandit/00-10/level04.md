
Goal: To retrieve the password stored in the only human-readable file in the ```inhere``` directory

Commands Used:
  - ```ls``` to check for further directories.
  - ```du``` to check for disk space occupied by any hidden files.
  - ```cd``` to change directories.
  - ```file``` to find the true details of the hidden file.
  - ```cat``` to read data.

Procedure:
  - After getting into ```inhere```, immediately using ```du``` revealed a hidden entity, "```.```" of size 24.
  - First, confusing ```.``` to be the actual filename, I attempted to enter it using ```cd```, to no avail.
  - Using ```find .```, the ```./...Hiding-From-You``` file name was revealed.
  - This was after some time of pure confusion, so this newfound discovery actually led to me getting a bit too excited, and I tried to cd into the file as though it was a folder. Rookie mistake?
  - Using ```cat``` to read the contents, I found the flag. 

Learnings:
  - Having no additional reading materials provided for this room, I used the good old search engine to learn more about this.
  - In Linux, any file/folder beginning with ```.``` is considered "hidden".
  - The purpose of hidden files was to hide system config files when using ```ls```. As such, ```ls``` ignores all hidden files. This explains why using ```ls``` clearly had its limits in this level.
  - If I intend to use ```ls```, I should include the ```-a``` flag to follow up, it stands for "all", and shows all files (even hidden ones).
  - I find this quite interesting. This was the first level where I faced additional challenge and felt the thrill of overcoming it.

Conclusion: Completed Level 04 successfully.
