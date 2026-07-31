Link: [https://cryptohack.org/courses/intro/fflags/]

Finding Flags:
  - This is a tutorial, the flag is provided and we are taught the format and how to submit it.

Great Snakes:
  - The resource provided, ```great_snakes.py```, is an example of the XOR Cipher.
  - Simply executing the code in python will give us the flag
  - XOR Cipher - A XOR operation is performed on every binary of the input against a cipher key (0x32 in this case, which translates to the number "50" in Hexadecimal) to give the resulting output. This is a Symmetric Encryption, and reversible since the plaintext can be obtained by performing XOR on the ciphertext with the key again.

ASCII:
  - An array of integers is provided and we are told that these integers are the ordinate values of the required ASCII values.
  - Depending on personal preferences, we can either convert every value individually and piece them together to decrypt the flag, or simply create a short and simple script in python (as recommended) or any other language one is comfortable in to compute and spew out the flag.
  - In python, the ```chr()``` function can be used to compute the ASCII counterpart of an ordinate value given, and `ord()` for vice versa.


   
