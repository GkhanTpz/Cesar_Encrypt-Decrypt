# Caesar Cipher Encryption and Decryption in C

This repository contains two C programs: one for encrypting messages using a Caesar Cipher and another for decrypting messages encrypted by the same method.

## Caesar Cipher Overview
The **Caesar Cipher** is a type of substitution cipher where each letter in the plaintext is shifted by a fixed number of positions down the alphabet. For example, with a shift of 1, 'A' becomes 'B', 'B' becomes 'C', and so on.

### Decryption Program
This program takes an encrypted message and a key (shift value) as input and returns the original message by shifting the characters backward.

- **Input**: 
  - An encrypted message (text) 
  - A key (integer)
- **Process**: 
  - For each character in the message:
    - If it is a lowercase letter (`a-z`), it is shifted backward by the key value.
    - If it is an uppercase letter (`A-Z`), it is also shifted backward, with a wrap-around if the shift goes past the start of the alphabet.
- **Output**: The decrypted message.

### Encryption Program
This program takes a plaintext message and a key (shift value) as input and returns the encrypted message by shifting the characters forward.

- **Input**: 
  - A plaintext message (text)
  - A key (integer)
- **Process**: 
  - For each character in the message:
    - If it is a lowercase letter (`a-z`), it is shifted forward by the key value.
    - If it is an uppercase letter (`A-Z`), it is shifted forward with a wrap-around if the shift goes past the end of the alphabet.
- **Output**: The encrypted message.

### How to Compile and Run
1. Save the decryption program as `decrypt.c` and the encryption program as `encrypt.c`.
2. Compile the programs using `gcc` or any C compiler:
   ```bash
   gcc decrypt.c -o decrypt
   gcc encrypt.c -o encrypt
   ```
3. Run the programs:
   ```bash
   ./decrypt
   ./encrypt
   ```

---
