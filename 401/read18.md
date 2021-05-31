# Encruption
 One of the earliest encryption techniques is the Caesar Cipher, invented by Julius Caesar more than two thousand years ago to communicate messages to his allies.
 The Caesar Cipher is a great introduction to encryption, decryption, and code cracking, thanks to its simplicity.
## Encrypting a message

Imagine Caesar wants to send this message:

    SECRET MEETING AT THE PALACE

Here's what that might look like encrypted:

    YKIXKZ SKKZOTM GZ ZNK VGRGIK

 That looks an awfully lot like gobbledygook at first, but this encrypted message is actually very related to the original text.
 The Caesar Cipher is a simple substitution cipher which replaces each original letter with a different letter in the alphabet by shifting the alphabet by a certain amount.

# Decrypting a message
According to historical records, Caesar always used a shift of 3. As long as his message recipient knew the shift amount, it was trivial for them to decode the message.
Imagine Caesar sends this message to a comrade:

    EHZDUH EUXWXV

They can then decode the message with certainty. The first letter "E" was shifted by 3 from "B", the second letter "H" was shifted by 3 from "E", etc. The result is this ominous message:

    BEWARE BRUTUS

# Frequency analysis
 Human languages tend to use some letters more than others. For example, "E" is the most popular letter in the English language. We can analyze the frequency of the characters in the message and identify the most likely "E" and narrow down the possible shift amounts based on that.