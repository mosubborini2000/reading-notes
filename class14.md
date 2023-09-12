Hashing:
Hashing is a process used in computer science and cryptography to convert any input, such as text, numbers, or files, into a fixed-size string of characters, which is typically a sequence of letters and numbers. This output, known as a "hash value" or "hash code," is unique to the input data, meaning that even a tiny change in the input will result in a significantly different hash value. Hashing is a one-way function, which means it's easy to compute the hash value from the input, but it's nearly impossible to reverse the process and determine the original input from the hash value.

Explanation of Hash Functions for a Non-Technical Friend:
Imagine a hash function as a magic machine that turns anything you put into it into a secret code that looks like a jumble of letters and numbers. For example, if you put in the word "apple," the machine might give you something like "5a8f1b91c3d81f7a." Now, here's the cool part: no matter how many times you put "apple" into the machine, it will always give you the same secret code, but if you change even a single letter in the word, the secret code will look completely different. This makes it really hard for someone to figure out the original word just by looking at the secret code.

Salting a Password:
To "salt" a password means to add a random piece of data (called a "salt") to the password before hashing it. This random salt is unique for each user and ensures that even if two users have the same password, their hash values will be different because of the unique salt. Salting is a crucial security measure because it prevents attackers from using precomputed tables (rainbow tables) to crack passwords more easily.

Information Needed to Access the Salt String:
A hacker would typically need direct access to the database where the passwords are stored to find the salt string. It's not something that should be publicly available. Protecting the salt is important because it adds an extra layer of security to the password hashing process.

Blowfish and Computation Speed:
Blowfish is a block cipher that can adjust its encryption speed based on the computer's processing power. It does this by using a variable number of encryption rounds, which can be increased to make the encryption process more computationally intensive. This flexibility allows Blowfish to remain secure against increasingly powerful computers.

Issues with Common Java Password Hashes:

Java Password Hash: This refers to using a simple hash function like SHA-1 or MD5 to hash passwords. The problem is that these hash functions are fast and can be easily brute-forced or cracked using modern hardware and techniques. They are no longer considered secure for password storage.

Java Password Encryption: Using encryption algorithms like AES to store passwords is not ideal either. Encryption is a two-way process, and if the encryption key is compromised, attackers can decrypt the stored passwords. Additionally, encryption does not provide the same level of security as proper password hashing with techniques like salting and key stretching.