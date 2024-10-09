# Date - 10 July 2024
# SMALL PROJECT ON SECURE PASSWORD MANAGEMENT

# Day 17: PASSWORD STRENGTH CHECKER 
- Next 2 days I will be focusing on a very basic project based on **Secure Password Management** i.e. Password Strength Checker which is used to check whether our password is strong or weak.
- It will give proper detail of setting up of a strong password.
- Today is my 1st day for implementation of my project.

---

## Day 1: Project Setup and Password Validation Rules
### Objective:
- Understand the basic structure of the password checker project, including defining password strength rules and basic regular expressions for validation.

---

### Key Concepts:
1. Password Strength: A good password must be long enough and contain a mix of characters, including uppercase, lowercase, digits and special characters.

2. Regular Expressions: Used for pattern matching in strings, helping us enforce password strength rules efficiently.

---

## Code Explanation (Day 1):
### Function Definition (check_password_strength):
- The function takes a password as input and checks it against several rules to determine its strength.
- Password Rules:
    - Rule 1: Password must be at least 8 characters long.
    - Rule 2: Password must contain at least one uppercase letter.
    - Rule 3: Password must contain at least one lowercase letter.
    - Rule 4: Password must contain at least one digit.
    - Rule 5: Password must contain at least one special character (e.g., !@#$%^&*).

---

## Regular Expressions:

- The regular expressions are used in the re.search() function to match patterns in the password:
    - r'[A-Z]': Matches an uppercase letter.
    - r'[a-z]': Matches a lowercase letter.
    - r'[0-9]': Matches a digit.
    - r'[\W_]': Matches a special character (anything that is not a letter or digit).

---

## Code for Day 1:

```python

import re

def check_password_strength(password):
  
    # Rule 1: Check password length
    if len(password) < 8:
        return "Password too short. Must be at least 8 characters."

    # Rule 2: Check for uppercase letter
    if not re.search(r'[A-Z]', password):
        return "Password must contain at least 1 uppercase letter."

    # Rule 3: Check for lowercase letter
    if not re.search(r'[a-z]', password):
        return "Password must contain at least 1 lowercase letter."

    # Rule 4: Check for digits
    if not re.search(r'[0-9]', password):
        return "Password must contain at least 1 digit."

    # Rule 5: Check for special characters
    if not re.search(r'[\W_]', password):
        return "Password must contain at least 1 special character (e.g., !@#$%^&*())."

    # If all rules are satisfied
    return "Password is strong."

# Main function to get user input and check the password
if __name__ == "__main__":
    print("Password Strength Checker")
    password = input("Enter your password: ")
    result = check_password_strength(password)
    print(result)

```

---

## Learning Outcome (Day 1):
- Learned about regular expressions and their use in validating passwords.
- Implemented basic password strength rules and enforced them using conditions in Python.
- Gained an understanding of how to structure a simple program that uses functions and takes user input.