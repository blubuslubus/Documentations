
Goal: To find the password in the ```inhere``` directory which is human-readable, is 1033bytes in size, and is not executable.

Commands Used:
  - ```ls``` to list filenames and directory.
  - ```cd``` to change directory.
  - ```file``` to check the type of data in the files.
  - ```cat``` to read file contents.

Procedure:  
  - I began by entering the ```inhere``` directory, and listing the files revealed -files 00-09.
  - Using the ```file``` command on all files, I found -file07 to be of ASCII text (the only human readable format) amongst the other data files.
  - Due note had to be taken in the syntax to include ```--``` before the filename as the filename contained a dash (-) in the beginning.
  - Using ```cat``` allowed me to retrieve the password from ```-file07```.
  - I then experimented around to find other potential paths I could have taken to arrive at this conclusion.

Learnings:
  - Instead of naming each file in the ```file```, I could simply use asterisk symbol to denote all files in current directory. ```file -- ./*```

Conclusion: Completed level 05 successfully.
