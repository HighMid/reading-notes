## Class 18 notes

1. **What is the basic principle behind the Caesar Cipher, and how was it used historically?**

    [Decryption and Encryption](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)

    - The [Caesar Cipher](https://en.wikipedia.org/wiki/Caesar_cipher) is a substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet. For example, with a shift of 1, 'A' would be replaced by 'B', 'B' would become 'C', and so on.

2. **What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?**

    [RNG in Computers](https://www.howtogeek.com/183051/htg-explains-how-computers-generate-random-numbers/)

    - Symmetric encrpytion is the usage of a key that does both encryption and decryption. This is considered faster as you do not need to compute a key for both encryption and decryption, the challenge with this is how the key is being distributed. 

    - Asymmetric encrpytion is used to provide a public and private key. The public key is shared openly while private keys are meant to be safeguarded. This makes it so if you were to encrypt with one key you would need the other key to decrypt which promotes security.

    - Both of these are used for communication daily as asymmetric uses SSL/TLS to secure a connection between two parties and symmetric for data transfer between two parties.

3. **How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.**

    - TRNG are numbers based off of a physical or random source such as the weather. This is completely random as it is unpreditable and leads to unreprodible results. These are used often in cryptography as this leads to very strong encrpytion by using physical phenomenas like quantum effects, radioactive decay etc. The outcome is truly unpredictable which safeguards against brute force tactics and other attacks

    - PRNG are numbers that are within a computers control but give the illusion of randomness. These produce the same sequence of numbers given the seed, this allows for fast and efficient processing as these do not require a lot of computation to achieve results. Video games often use PRNG as a way to ensure `fair` and `balance` RNG while still giving the player the illusion of randomness.

4. **What’s the difference between encryption and decryption? Explain with an analogy.**

    - Encryption is the act of converting text into ciphertext by using an encryption algorithm and producing a key. This is the act of making something secure by locking it using this key.

    - Decryption is the act of converting ciphertext back to text by using a decryption algorithm and producing a key. This is the act of unlocking sed secure item by unlocking it using this key.