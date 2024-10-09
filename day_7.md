# Date - 21 June 2024
# SMALL PROJECT ON AUTHENTICATION AND AUTHORIZATION

# Day 7: AUTHENTICATION CHECKER
- Next 2 days I will be focusing on a very basic project which is used to Authenticate where an individual is having a access to system or not.
- Today is my 2nd day for implementation of my project.

---

# Day 2: Implement Authentication and Finalize the System
##  Authentication Logic
1. Develop Authentication Flow: Now that we have a working password hashing function, let’s build the authenticate_user() function. This will simulate user registration (storing the hashed password) and login (checking the entered password against the stored hash).

---

```python

import hashlib

# Function to hash a password
def hash_password(password):
    hashed = hashlib.sha256()
    hashed.update(password.encode('utf-8'))
    return hashed.hexdigest()

# Function to authenticate the user
def authenticate_user():
    # Ask user to create a password
    password = input("Create a password: ")

    # Hash the password
    stored_hash = hash_password(password)
    print("\nPassword has been securely stored (hashed).")

    # Simulate login
    print("\nLogin process")
    login_password = input("Enter your password to log in: ")

    # Hash the entered password
    login_hash = hash_password(login_password)

    # Compare the entered hash with the stored hash
    if login_hash == stored_hash:
        print("Access granted. Welcome!")
    else:
        print("Access denied. Incorrect password.")

# Run the program
if __name__ == "__main__":
    authenticate_user()

```

2. Testing the Authentication System:
- First, create a password (e.g., "mypassword").
- Then, attempt to log in by entering the correct password ("mypassword") and the incorrect one ("wrongpassword") to see if the system grants or denies access correctly.

---

### Example Run:

```python
Create a password: mypassword

Password has been securely stored (hashed).

Login process
Enter your password to log in: mypassword
Access granted. Welcome!

```
---

### Incorrect Password:

```python

Create a password: mypassword

Password has been securely stored (hashed).

Login process
Enter your password to log in: wrongpassword
Access denied. Incorrect password.

```
---

## Final Enhancements and Documentation
1. Refine User Interaction:
- Add some basic error handling for cases like empty input or invalid characters.
- Improve the user experience by printing clearer instructions or messages.

2. Error Handling (Optional Enhancement): Here’s an enhancement that checks if the user input is empty or too short:

---

```python

def authenticate_user():
    # Ask user to create a password with basic validation
    while True:
        password = input("Create a password (min 6 characters): ")
        if len(password) < 6:
            print("Password too short. Please try again.")
        else:
            break

    # Hash the password
    stored_hash = hash_password(password)
    print("\nPassword has been securely stored (hashed).")

    # Simulate login with error handling for empty input
    print("\nLogin process")
    while True:
        login_password = input("Enter your password to log in: ")
        if len(login_password) == 0:
            print("Password cannot be empty. Please enter your password.")
        else:
            break

    # Hash the entered password
    login_hash = hash_password(login_password)

    # Compare the entered hash with the stored hash
    if login_hash == stored_hash:
        print("Access granted. Welcome!")
    else:
        print("Access denied. Incorrect password.")

```

---

3. Documentation:
- Document your code with comments explaining the logic behind each function.

---

## Final Project Summary:
In this project, I implemented a simple password authentication system using SHA-256 hashing. The system works by hashing the password during registration and comparing the hashed version during login. This ensures that passwords are never stored in plaintext, increasing security. We added error handling to improve user interaction, and the project demonstrates essential concepts in secure password storage and authentication.

