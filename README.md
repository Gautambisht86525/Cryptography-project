# 🔐 Caesar Cipher Brute-Force Attack Simulator

An interactive web-based project that demonstrates how the **Caesar Cipher** works and how its small key space makes it vulnerable to a **brute-force attack**.

The project allows users to encrypt a message using a Caesar Cipher and then visually simulate an attacker trying every possible key to recover the original plaintext.

---

## 📌 About the Project

The **Caesar Cipher Brute-Force Attack Simulator** is an educational cryptography project designed to demonstrate both **Caesar Cipher encryption** and its vulnerability to **brute-force attacks**.

The user first enters a plaintext message and selects an encryption key between **1 and 25**. The application encrypts the message using the Caesar Cipher.

After encryption, a simulated attacker attempts to decrypt the ciphertext by testing every possible key.

Each attempt is displayed on the screen so that the brute-force process can be observed step by step.

---

## ✨ Features

* 🔒 Encrypt plaintext using the Caesar Cipher
* 🔑 Select an encryption key from **1–25**
* ⚔️ Simulate a brute-force attack
* 🔄 Test all possible Caesar Cipher keys
* 🔍 Display every decryption attempt
* ✅ Highlight the correct decrypted message
* ⚠️ Detect text that may resemble English
* 📊 Display attack progress
* ⏱️ Track elapsed attack time
* 🔢 Count the number of attempts
* 🎚️ Adjustable attack speed
* ⏹️ Start and stop the attack simulation
* 📱 Responsive web interface
* 🌐 Runs completely inside the browser

---

## ⚙️ How It Works

### 1. Enter the Plaintext

The user enters a message that they want to encrypt.

Example:

```text
HELLO WORLD
```

### 2. Select an Encryption Key

The user selects a Caesar Cipher shift between **1 and 25**.

For example:

```text
Key = 3
```

### 3. Encrypt the Message

Each alphabetic character is shifted according to the selected key.

For example:

```text
Plaintext:
HELLO WORLD

Key:
3

Ciphertext:
KHOOR ZRUOG
```

### 4. Launch the Brute-Force Attack

The attacker does not need to know the original encryption key.

Instead, the simulator tries every possible key:

```text
Key 1  → Decryption Attempt
Key 2  → Decryption Attempt
Key 3  → Decryption Attempt
...
Key 25 → Decryption Attempt
```

Eventually, one of the keys produces the original plaintext.

---

## 🔍 Result Classification

The application visually classifies each decryption attempt.

### ✅ Correct Match

The decrypted text matches the original plaintext.

### ⚠️ Looks Like English

The result contains words or patterns that may resemble English text according to the project's basic heuristic.

### ❌ Not English

The decrypted output does not appear to contain recognizable English patterns.

---

## 📊 Attack Statistics

During the brute-force attack, the simulator displays:

* Number of attempted keys
* Time elapsed
* Number of correct matches found
* Current key being tested
* Current decrypted text
* Overall attack progress

A progress bar visually represents the brute-force process.

---

## 📁 Project Structure

```text
Cryptography-project/
│
├── CODE/
│   └── index.html
│
└── README.md
```

The entire application is currently implemented inside a single `index.html` file containing the HTML, CSS, and JavaScript.

---

## 💻 Technologies Used

### HTML5

Used to create the structure and elements of the web application.

### CSS3

Used for:

* Interface styling
* Responsive layout
* Buttons
* Result highlighting
* Progress bar
* Attack statistics

### JavaScript

Used to implement:

* Caesar Cipher encryption
* Caesar Cipher decryption
* Brute-force attack simulation
* Key testing
* English-text heuristic
* Attack timing
* Progress calculation
* DOM manipulation
* Attack statistics

---

## 🚀 How to Run the Project

No backend, database, framework, or package installation is required.

### Step 1 — Clone the Repository

```bash
git clone https://github.com/Gautambisht86525/Cryptography-project.git
```

### Step 2 — Open the Project

```bash
cd Cryptography-project
```

### Step 3 — Open

```text
CODE/index.html
```

in any modern web browser.

You can also open the project using **Visual Studio Code** and run `index.html` using a local development extension such as Live Server.

---

## 🧪 Example

Suppose the user enters:

```text
HELLO WORLD
```

and selects:

```text
Encryption Key = 3
```

The Caesar Cipher produces:

```text
KHOOR ZRUOG
```

The brute-force simulator then tests the possible keys until the original message is recovered.

When the correct shift is tested:

```text
HELLO WORLD
```

is displayed as:

```text
✅ CORRECT MATCH!
```

---

## 🧠 What This Project Demonstrates

The project demonstrates an important concept in cryptography:

> A cipher with a very small key space can be vulnerable to exhaustive brute-force searching.

The Caesar Cipher has only a small number of possible shifts. Therefore, an attacker can simply try every possible key until meaningful plaintext is obtained.

This is one of the reasons why the Caesar Cipher should **not** be used for real-world secure communication.

---

## 🎯 Learning Outcomes

Through this project, you can understand:

* Basic cryptography concepts
* Caesar Cipher encryption
* Caesar Cipher decryption
* Substitution ciphers
* Encryption keys
* Brute-force attacks
* Exhaustive key searching
* Weakness of small key spaces
* Basic cryptanalysis concepts
* JavaScript-based algorithm simulation
* DOM manipulation
* Interactive web application development

---

## ⚠️ Limitations

This project is designed primarily for **educational demonstration**.

Current limitations include:

* Only the Caesar Cipher is implemented.
* The brute-force attack checks Caesar keys from **1–25**.
* English detection uses a basic word-based heuristic.
* It is not a complete cryptanalysis system.
* Exact-match detection compares the attempted plaintext with the original plaintext stored by the application.
* It should not be used for protecting sensitive or confidential information.

---

## 🎓 Educational Purpose

This project was developed to understand the fundamentals of **cryptography, Caesar Cipher encryption, decryption, and brute-force attacks** through an interactive visual simulation.

It demonstrates why classical encryption algorithms with small key spaces are vulnerable to exhaustive attacks.

---

## 👨‍💻 Author

**Gautam Bisht**

GitHub: [@Gautambisht86525](https://github.com/Gautambisht86525)

---

## ⭐ Support

If you found this project useful for learning cryptography, consider giving the repository a **star ⭐**.
