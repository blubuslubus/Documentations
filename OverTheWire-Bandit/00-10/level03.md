
Goal: To retrieve password stored in a file called ```--spaces in this filename--``` located in the home directory.

Commands Used:
  - ```ls``` to list file names in the directory
  - ```cat``` to attempt to read the contents of the file

Procedure:
  - I used ```ls``` to check for the file names in this directory. I believe this is simply standard practice now, and need not be mentioned. I will try to, regardless.
  - Having found the file, I used ```cat --spaces in this filename--```, despite the spaces to see what would happen.
  - Then, I opted to add ```./``` before all spaces to find if that makes a difference for spaces too.
  - Looking into the additional readings provided, I understood that quotation marks around entire file name, including the spaces, is the simple solution.
  - Realising that the ```--``` preceding "spaces" in the filename will cause another misunderstanding of another function or option, so I preceded the filename within quotes with ```--```, learning from the previous level.

Learnings:
  - If spaces are included after ```cat```, each word separated by spaces is treated as its own filename, and the system will attempt to look for that filename.
  - ```./``` seems to be successful to use only when preceding ```--``` to signify "no functions ahead".
  - Use quotation marks for filenames with spaces.

Conclusion: Completed level 03 successfully.
