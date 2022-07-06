# Reading Class 18

## Encryption, decryption, and cracking

One of the earliest encryption techniques is the Caesar Cipher, invented by Julius Caesar more than two thousand years ago to communicate messages to his allies.
The Caesar Cipher is a great introduction to encryption, decryption, and code cracking.

## Caesar cipher
In cryptography, a Caesar cipher, also known as Caesar's cipher, the shift cipher, Caesar's code or Caesar shift, is one of the simplest and most widely known encryption techniques. It is a type of substitution cipher in which each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet. For example, with a left shift of 3, D would be replaced by A, E would become B, and so on.

Example for encrypting a message

Imagine Caesar wants to send this message:

>> SECRET MEETING AT THE PALACE

Here's what that might look like encrypted:

>> YKIXKZ SKKZOTM GZ ZNK VGRGIK


Decrypting a message

According to historical records, Caesar always used a shift of 3. As long as his message recipient knew the shift amount, it was trivial for them to decode the message.

Imagine Caesar sends this message:

>> EHZDUH EUXWXV

Decrypting depending on this substitution table, where the alphabet is shifted by 3:


A	B	C	D	E	F	G	H	I	J	K	L	M	N	O	P	Q	R	S	T	U	V	W	X	Y	Z
D	E	F	G	H	I	J	K	L	M	N	O	P	Q	R	S	T	U	V	W	X	Y	Z	A	B	C

>> BEWARE BRUTUS