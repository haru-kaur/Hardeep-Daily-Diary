# Date - 19 June 2024
# AUTHENTICATION AND AUTHORIZATION

# Day 5: Authentication and Authorization
- Today’s I focused on two critical concepts in cyber security: Authentication and Authorization. At first, the terms seemed interchangeable but I quickly realized that they have distinct meanings. Authentication is the process of verifying the identity of a user while authorization determines what resources the authenticated user has access to.

- Authentication and Authorization are two critical concepts in the field of information security. While they are often used together, they serve distinct purposes in controlling access to systems and resources.

---

## 1. Authentication:
Authentication is the process of verifying the identity of a user, device, or system. In other words, it’s about answering the question "Who are you?". It ensures that the entity trying to access a system is indeed who they claim to be.

### Types of Authentication:
1. Something you know (Knowledge-based):
- Examples: Passwords, PINs, answers to security questions.
- The user proves their identity by correctly entering information that only they should know.

2. Something you have (Possession-based):
- Examples: Smartcards, one-time password (OTP) tokens, mobile devices, hardware security keys (e.g., YubiKey).
- The user provides evidence that they have a physical object to authenticate.

3. Something you are (Biometric-based):
- Examples: Fingerprints, face recognition, iris scans, voice recognition.
- The user proves their identity by providing a biological or behavioral characteristic.

4. Something you do (Behavioral):
- Examples: Typing patterns, mouse movement, how a user interacts with a system.
- The system monitors behavioral patterns to authenticate the user.

### Example of Authentication:
When you log into a website using your username and password, the website checks whether the password matches the one stored in the system for your account. If it does, the website knows that you are the person who owns that account (assuming no one else has access to your password). This is authentication in action.

### Authentication Methods:
1. Single-factor authentication (SFA): Requires only one method of authentication (e.g., a password).
2. Two-factor authentication (2FA): Requires two different forms of authentication (e.g., password + OTP from a phone).
3. Multi-factor authentication (MFA): Requires two or more forms of authentication from different categories (e.g., password + fingerprint + OTP).

---

## 2. Authorization:
- Authorization occurs after authentication and determines what the authenticated user is allowed to do. In other words, once the system knows who you are (via authentication), it needs to decide what resources you can access or what actions you are allowed to perform.
- Authorization is about permission and access control.

### Types of Authorization:
1. Role-based access control (RBAC):
- Users are assigned to specific roles, and each role has defined permissions (e.g., admin, editor, viewer). Each role can access certain resources based on the roles and permissions set by the system.

2. Discretionary access control (DAC):
- Users control access to their own resources. For example, file owners can grant or deny access to specific users or groups.

3. Mandatory access control (MAC):
- Access is controlled by a central authority and is based on security labels. It’s often used in highly secure environments where access to resources is tightly controlled based on predefined rules.

### Example of Authorization:
1. After successfully logging in to a system (authentication), you may try to access certain resources like files, applications, or features. Authorization checks will determine whether you have permission to access those resources. For example:
2. If you log into a corporate network, you may have access to your files, but not to sensitive financial reports reserved for the finance team.
3. A user who logs into a website might be allowed to view public pages, but only an admin can modify content or view private user data.

---

- I learned about the various methods of authentication, starting with something as simple as passwords. However, we also discussed why relying solely on passwords can be risky, especially with the prevalence of password cracking techniques like brute force attacks and dictionary attacks. Multi-factor authentication (MFA) was introduced as a way to strengthen authentication. MFA combines something you know (a password), something you have (a security token or mobile device), and something you are (biometrics, like fingerprints).

- Next, we moved on to authorization, where I learned how systems control access to resources. This is typically managed through roles and permissions, where users are assigned certain roles, each with specific permissions. For example, an administrator might have full access to a system, while a regular user has limited access. We looked at the principle of least privilege, which dictates that users should be granted only the permissions they need to perform their tasks—nothing more.

---

## Today's Learning Summary:
Today I learned that Authentication verifies the identity of a user, device, or system, answering "Who are you?" It typically involves methods like passwords, OTPs, or biometrics. Authorization, on the other hand, determines what an authenticated user can do, answering "What are you allowed to do?" It is based on roles and permissions, like allowing an admin to access sensitive data while restricting a regular user. While authentication confirms identity, authorization controls access and permissions, ensuring security and proper access control.