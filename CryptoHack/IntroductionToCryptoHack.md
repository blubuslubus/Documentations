Link: [https://cryptohack.org/courses/intro/course_details/]

## Finding Flags:
  - This is a tutorial, the flag is provided and we are taught the format and how to submit it.

## Great Snakes:
  - The resource provided, ```great_snakes.py```, is an example of the XOR Cipher.
  - Simply executing the code in python will give us the flag
  - XOR Cipher - A XOR operation is performed on every binary of the input against a cipher key (0x32 in this case, which translates to the number "50" in Hexadecimal) to give the resulting output. This is a Symmetric Encryption, and reversible since the plaintext can be obtained by performing XOR on the ciphertext with the key again.

## ASCII:
  - An array of integers is provided and we are told that these integers are the ordinate values of the required ASCII values.
  - Depending on personal preferences, we can either convert every value individually and piece them together to decrypt the flag, or simply create a short and simple script in python (as recommended) or any other language one is comfortable in to compute and spew out the flag.
  - In python, the ```chr()``` function can be used to compute the ASCII counterpart of an ordinate value given, and `ord()` for vice versa.

## Hex:
  - We are given a ciphertext encrypted in Hex, and need to simply convert it from Hex to printable ASCII form.
  - The course recommends us to once again use python for the computing. We are suggested to use `bytes.fromhex()` function to obtain bytes, and also that hex() can be operated on on the string to get its hex representation. I would recommend to use `decode()` alongside.
  - Aside from python, I would very strongly suggest learning and using CyberChef instead, often known as the Swiss-Army-Knife for cyber.

## Base64:
  - We are given a hex string, and suggested to first decode it into bytes, then pass it through `base64.b64encode()` of the base64 module in python. Doing so works perfectly fine.
  - Another method that I opted to use is once again CyberChef, and the recipe is simply `From Hex` `To Base64` set to Alphabet.
  - Do note that the flag you obtain may look a little different to the other flags, but worry not. I believe this is done deliberately to portray how Base64 is web-safe.

## Bytes and Big Integers:
  - We are given a Big Integer, which can be a little annoying to work with sometimes. For this, I suggest using Python too and not CyberChef.
  - Install PyCryptodome, with is a package useful for hashing, RSA, and many other cryptographic aims.
  - Convert the bytes of the given BigInt using `long_to_bytes()` and decode it as usual to obtain the flag.

## XOR Starter:
  - I have discussed the XOR Cipher here already, but as a refresher, every bit of the plaintext and key are compared and an XOR operation is performed (if both inputs are same, output is 0, if both inputs are different, output is 1).
  - Once again I recommend using CyberChef as it is much more efficient, but there is no harm in practicing in python either.
  - Do note, in CyberChef select Decimal type when inputing the key.

## XOR Properties:
  - The Commutative, Associative, Identity and Self-Inverse properties of XOR are discussed here. We are given Key1, XOR of Key1 and Key2, XOR of Key2 and Key3, and all 3 keys XOR'ed with the flag.
  - The simplest way to understand how we can undo the encryption on the flag is by simply performing XOR on it against all 3 keys. And we can find all 3 keys by performing XOR on Key1 and Key2^Key1 to find Key2, and once again with Key2 and Key2^Key3 to find Key3.
  - I recommend using python scripting for this as it is a good exercise for both working with logically and understanding a clearer picture of python scripting.

## Favourite Byte:
  - This one is a glimpse of brute-forcing the key. Since the encryption uses a single-byte key, we can simply brute-force our way by performing XOR with all 255 bytes, which is rather quick in python if you would like to try, and similarly easy on CyberChef.
  - Alternatively, you can use the known plaintext (`crypto{`) to find the key too. Easiest way to go about this is to XOR the first byte of ciphertext with the hex of the first letter of plaintext which is 'c'.

## You either know, XOR you don't:
  - This one is an example of a repeating-byte key. This strategy works easily i nCTFs since we have a bit of the known plaintext of the flag in the form of the flag format (```cryto{```).
  - By performing XOR operation on the given ciphertext hex and the first 6 bytes of the plaintext, we can find a partial key, and then deduce the full key (Hint: Key is 7 characters long).
  - I solved this using both the tools as per my convenience. I used python to find the partial key itself, then CyberChef to decrypt the ciphertext with the repeating key.



You have reached the end of this document. This concludes the Introduction to Cryptography course module at CryptoHack. I enjoyed going through these, and learned a little about practical experience with XOR cipher too, eventhough I had theoretical preliminary knowledge about it.

   
