
Goal: To retrieve password stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed.

Commands used:
  - ```ls -a```, to list all files and directories.
  - ```cd```, to change directories.
  - ```cp```, to copy the file to a temporary directory.
  - ```xxd -r```, to reverse the hexadecimal encoding.
  - ```tar -xvf```, to unzip tar archives and know the output filename.
  - ```gunzip```, to unzip ```gz``` layers.
  - ```bunzip2```, to unzip ```bz2```.
  - ```mv```, to rename files with the right extension.

Procedure:
  - I did not have permissions to write or create directories in the main directory, so I made one in ```/tmp``` and used it as my workspace. Deleted this when I was done.
  - After copying ```data.txt``` to my workspace, I converted it to the usable binary format from the hexadecimal format it was present in using ```xxd -r```.
  - Using the ```file``` command on the file would tell me exactly which type of unzipping program I need to.
  - After learning about the unzipping methods and commands, I got down the layers into ```data8.txt```, which held the password.

Learnings:
  - Copying a file to another directory.
  - Deleting a directory.
  - Encoding and decoding to and from hexadecimal encryption.
  - Using tar archive, gzip, and bz2.
  - Renaming a file.

Conclusion: Completed Level 12 successfully.
