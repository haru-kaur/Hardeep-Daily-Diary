# Date - 20 June 2024
# SMALL PROJECT ON AUTHENTICATION AND AUTHORIZATION

# Day 6: AUTHENTICATION CHECKER
- Next 2 days I will be focusing on a very basic project which is used to Authenticate where an individual is having a access to system or not.
- Today is my 1st day for implementation of my project.

---

# Day 1: Project Setup and Hashing Logic Implementation

## Understand Hashing Concepts:
- Password hashing is used to store passwords securely. When users create a password, it should never be stored in plaintext. Hashing transforms the password into a fixed-length, irreversible string.
- SHA-256 (Secure Hash Algorithm) is a widely-used hashing algorithm that produces a unique 256-bit (32-byte) hash for each input.

---

### Set Up Development Environment:

1. Install Python (if not already installed).
2. Create a new folder for the project (e.g. Authenticate_project).
3. Create a Python file (e.g. auth.py) where you'll write the hashing and authentication code.

---

### Implement Hashing Function
1. Hashing Function: Write the function hash_password() to hash the user’s password using SHA-256. 
- Here’s the code for that:

```python

import hashlib

# Function to hash a password using SHA-256
def hash_password(password):
    # Create a new sha256 hash object
    hashed = hashlib.sha256()
    # Update the hash object with the password (convert string to bytes)
    hashed.update(password.encode('utf-8'))
    # Return the hexadecimal digest of the hashed password
    return hashed.hexdigest()

# Test the hashing function
if __name__ == "__main__":
    password = input("Enter a password to hash: ")
    hashed_password = hash_password(password)
    print("Hashed password:", hashed_password)

```

### Explanation:
This function takes the plaintext password, encodes it into bytes (since SHA-256 works on bytes), updates the hash object, and returns the hashed password in hexadecimal form.

---

2. Testing Hashing Function: Run the code and check if the same password generates the same hash. Test with different passwords to ensure unique hashes are generated:

---
## Output

```python
Enter a password to hash: mysecretpassword
Hashed password: 2c6ee24b09816a6f14f95d1698b24ead
```
