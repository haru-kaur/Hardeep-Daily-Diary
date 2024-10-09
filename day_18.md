# Date - 11 July 2024
# SMALL PROJECT ON SECURE PASSWORD MANAGEMENT

# Day 18: PASSWORD STRENGTH CHECKER
- Next 2 days I will be focusing on a very basic project based on **Secure Password Management** i.e. Password Strength Checker which is used to check whether our password is strong or weak.
- It will give proper detail of setting up of a strong password.
- Today is my 2nd day for implementation of my project.

---

## Day 2: Testing, Refining, and Optimization
### Objective:
- Improve the user experience by refining the program, adding comments for clarity, and optimizing the password-checking logic.

---

### Key Concepts:
1. User Input Handling: Provide a more user-friendly interface for input and output.

2. Code Optimization: Refactor and improve readability, such as combining rules or handling edge cases.

---

## Code Explanation (Day 2):

1. Refinement:
    - Added more user-friendly print statements to explain what the program does.
    - Organized the code into a clean, easy-to-read format.

2. Testing:
    - Tested the program with various password inputs to ensure that all rules are applied correctly. Examples include:
    Short passwords (e.g., "123").
    - Passwords with missing characters (e.g., "abcdefgh")
    - Strong passwords that meet all rules (e.g., "Abc!1234")

3. Optimization:
- Instead of checking each rule one by one and returning immediately, the logic could be expanded to provide detailed feedback on all failed rules at once.

---

## Code for Day 2:

``` python

import re

def check_password_strength(password):
    # Initialize an empty list to store the errors
    errors = []

    # Rule 1: Check password length
    if len(password) < 8:
        errors.append("Password too short. Must be at least 8 characters.")

    # Rule 2: Check for uppercase letter
    if not re.search(r'[A-Z]', password):
        errors.append("Password must contain at least 1 uppercase letter.")

    # Rule 3: Check for lowercase letter
    if not re.search(r'[a-z]', password):
        errors.append("Password must contain at least 1 lowercase letter.")

    # Rule 4: Check for digits
    if not re.search(r'[0-9]', password):
        errors.append("Password must contain at least 1 digit.")

    # Rule 5: Check for special characters
    if not re.search(r'[\W_]', password):
        errors.append("Password must contain at least 1 special character (e.g., !@#$%^&*()).")

    # If no errors, the password is strong
    if not errors:
        return "Password is strong."

    # Return all errors if any rules are violated
    return "\n".join(errors)

# Main function to get user input and check the password
if __name__ == "__main__":
    print("Welcome to the Password Strength Checker!")
    password = input("Enter your password: ")
    result = check_password_strength(password)
    print(result)

``` 

## Learning Outcome (Day 2):
- Improved the user interface by giving clearer error messages for each failed rule.
- Learned how to optimize error handling by collecting all issues in a list and displaying them together at the end.
- Conducted tests and verified the correctness of the program by applying various test cases to ensure all rules are enforced.

---

## Project Conclusion:
The Password Strength Checker project provided an opportunity to learn about password validation and error handling using Python and regular expressions. Over two days, the program was enhanced from a basic rule-checking script to a more user-friendly tool with detailed feedback and robust password validation.






