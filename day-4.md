# Date - 18 June 2024
# INTRODUCTION TO CRYPTOGRAPHY


# Day 4: Introduction to Cryptography
Cryptography was the highlight of today’s session. I’ve always been curious about how encryption works, so today’s lesson was particularly exciting for me. We started with the basics—understanding the difference between encryption and decryption. Encryption and decryption are fundamental concepts in cryptography which is the practice of securing communication and data by transforming information into a form that is unreadable to unauthorized parties.

--- 

## 1. Encryption:
Encryption is the process of converting plaintext (readable data) into ciphertext (unreadable data) using a specific algorithm and a secret key. The purpose of encryption is to protect the confidentiality of the data, ensuring that even if someone intercepts the data, they won't be able to understand it without the appropriate key.

1. Plaintext: The original, readable message or data.
2. Ciphertext: The transformed, encrypted version of the plaintext that appears as random or garbled text.
3. Encryption Algorithm: The method or formula used to perform the transformation.
4. Key: A secret value used in the encryption process. The key can be a string of characters or a number, depending on the encryption method.


### Example of Encryption:
Imagine you want to send the message "HELLO" securely. Using an encryption algorithm and a secret key, the message "HELLO" could be encrypted into something like "KHOOR." Without the key, the encrypted message is unreadable.

---

## 2. Decryption:
Decryption is the process of converting ciphertext back into plaintext using an algorithm and a key. The goal of decryption is to reverse the encryption process, making the data readable again for the intended recipient.

1. Decryption Algorithm: The method used to reverse the encryption and convert ciphertext back into plaintext.
2. Key: The same key used for encryption in symmetric encryption or a related key in asymmetric encryption.

### Example of Decryption:
If you receive the message "KHOOR" and you have the correct key (the same one used for encryption), you can decrypt it back to the original message "HELLO."

---

### Types of Encryption
There are two main types of encryption: Symmetric Encryption and Asymmetric Encryption.

1. Symmetric Encryption:
In symmetric encryption, the same key is used for both encryption and decryption. This means that both the sender and the recipient must securely share the same key before they can communicate securely.

- Key: Shared between the sender and receiver. If someone intercepts the key, they can decrypt the message.

- Strength: Fast and efficient for encrypting large amounts of data. Challenge: Secure key distribution; if the key is compromised, so is the communication.

2. Asymmetric Encryption:
Asymmetric encryption uses two different keys: a public key and a private key. The public key is used to encrypt data, and the private key is used to decrypt it. The two keys are mathematically related, but the private key cannot be easily derived from the public key.

- Key: Public key is shared openly, while the private key is kept secret.

- Strength: Secure key exchange without needing to share a secret key in advance. Challenge: Slower compared to symmetric encryption, especially with large amounts of data.

### Example:
1. Public Key Encryption: If Alice wants to send a secure message to Bob, she can use Bob’s public key to encrypt the message. Only Bob’s private key can decrypt it, ensuring only he can read the message.

2. Private Key Decryption: Bob uses his private key to decrypt the message.

---

## Today's Learning Summary:
Today I learned that encryption and decryption are core to keeping data secure, protecting it from unauthorized access, and ensuring privacy in digital communications. Symmetric encryption is fast and efficient but requires secure key sharing, while asymmetric encryption offers more security through public-private key pairs but can be slower.




