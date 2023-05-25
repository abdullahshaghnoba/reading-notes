# Encryption, Decryption & Hacking

## importances of Encryption, Decryption & Hacking
1. Encryption: Protecting sensitive data using encryption algorithms like AES, RSA, or DES.
2. Decryption: Retrieving the original data from encrypted form, ensuring data confidentiality.
3. Hacking: Assessing system vulnerabilities, securing systems, and understanding cybersecurity concepts.

---

## What is the basic principle behind the Caesar Cipher, and how was it used historically?

### Answer: The basic principle behind the Caesar Cipher is a shift of each letter in the plaintext by a fixed number of positions in the alphabet.

---

## What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?

### Answer: 
### The key differences between symmetric and asymmetric encryption are as follows:

#### Symmetric Encryption:

#### Uses a single shared key for both encryption and decryption.
#### Faster and more efficient than asymmetric encryption.
#### Key distribution between communicating parties is challenging.
#### Suitable for encrypting large amounts of data.
#### Examples of symmetric encryption algorithms include AES, DES, and 3DES.

#### Asymmetric Encryption:

#### Uses a pair of mathematically related keys: a public key for encryption and a private key for decryption.
#### Slower and computationally more expensive than symmetric encryption.
#### Enables secure key exchange and authentication.
#### Widely used for secure communication and digital signatures.
#### Examples of asymmetric encryption algorithms include RSA, Diffie-Hellman, and ECC.
#### In secure communication today, asymmetric encryption is primarily used for key exchange and digital signatures.

---

## How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.

### Answer: 
### TRNG relies on unpredictable physical processes like atmospheric noise or radioactive decay to generate truly random numbers. It is used in cryptography for tasks requiring absolute randomness, such as key generation.

### PRNG algorithms use deterministic computations and a seed value to generate random-like numbers. The sequence is predictable if the seed is known. PRNGs are commonly used in cryptography for tasks like key generation, but not for sensitive operations like generating nonces.

---

## What’s the difference between encryption and decryption? Explain with an analogy.

### Answer: Encryption is the process of transforming plaintext into ciphertext using an encryption algorithm and a secret key. It's like locking a message inside a secure box with a unique key.

### Decryption is the reverse process of converting ciphertext back into plaintext using the same encryption algorithm and the corresponding secret key. It's like unlocking the secure box and retrieving the original message.

### In analogy, encryption is akin to placing a letter in a locked box, while decryption is opening the box with the correct key to read the letter inside.

## Things I want to know more about None