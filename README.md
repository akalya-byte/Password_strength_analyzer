# Password_strength_analyzer

## **Domain:**
Cryptography and Network Security


## **Problem Statement:**

Weak passwords are one of the biggest threats to cybersecurity. Many users still choose passwords that can be easily guessed or cracked through brute force attacks.
The goal of this project is to **design a system that analyzes and evaluates the strength of passwords** based on cryptographic and security metrics such as entropy, complexity, and resistance to attacks.

## **Objectives:**

1. To build a tool that evaluates the strength of user-entered passwords.
2. To analyze password robustness using various security parameters (length, special characters, digits, uppercase, lowercase).
3. To demonstrate cryptographic entropy calculation for measuring password strength.
4. To educate users on creating strong, secure passwords resistant to dictionary and brute-force attacks.


## **System Design / Architecture:**

**Modules:**

1. **User Input Module:** Accepts the password from the user.
2. **Analysis Module:**

   * Checks password length and character diversity.
   * Calculates **entropy** (based on Shannon entropy formula).
   * Detects patterns like sequential numbers or common words.
3. **Scoring Module:**

   * Assigns a score (Weak / Medium / Strong / Very Strong).
4. **Feedback Module:**

   * Provides suggestions to make the password stronger (e.g., “Add special characters” or “Increase length”).

**Optional Add-on:**

* Integrate a **hashing module (SHA-256)** to show how passwords are stored securely in systems.

---

##  **Tools and Technologies:**

| Component                  | Suggested Option                         |
| -------------------------- | ---------------------------------------- |
| **Programming Language**   | Python / Java / Android (Kotlin or Java) |
| **Libraries (for Python)** | `re` (regex), `math`, `hashlib`          |
| **Platform**               | Desktop or Web-based                     |
| **IDE**                    | PyCharm / VS Code / Android Studio       |

---

## **Algorithm (Logic in Steps):**

1. Take password input from the user.
2. Check for character variety:

   * Lowercase letters
   * Uppercase letters
   * Numbers
   * Special symbols
3. Calculate **password entropy (H)** using:
   [
   H = L \times \log_2(N)
   ]
   where

   * *L* = length of password
   * *N* = possible symbol set size (e.g., 26 for lowercase, 10 for digits, etc.)
4. Based on entropy value:

   * < 28 bits → **Very Weak**
   * 28–35 bits → **Weak**
   * 36–59 bits → **Reasonable**
   * 60–127 bits → **Strong**
   * ≥ 128 bits → **Very Strong**
5. Display rating and suggestions.

prepare a **mini project report (Word/PDF)** for submission — with intro, architecture diagram, code snippet, and conclusion?
I can generate that next for you.
