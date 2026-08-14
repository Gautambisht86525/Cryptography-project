# 🔐 Caesar Cipher Brute-Force Attack Simulator

An interactive web-based cryptography project that demonstrates how the **Caesar Cipher** works and how its small key space makes it vulnerable to a **brute-force attack**.

The project allows users to encrypt a message using a Caesar Cipher and then visually simulate an attacker trying every possible key to recover the original plaintext.

---

## 📌 About the Project

The **Caesar Cipher Brute-Force Attack Simulator** is an educational project developed to demonstrate the fundamentals of classical cryptography and brute-force attacks.

The application follows two main stages:

1. **Encryption** — The user enters plaintext and selects a Caesar Cipher key.
2. **Brute-Force Attack** — The simulator attempts every possible key from **1 to 25** and displays the resulting decryptions.

The application provides a visual representation of the attack process, including the current key, decrypted message, number of attempts, elapsed time, and attack progress.

---

## ✨ Features

* 🔒 Caesar Cipher encryption
* 🔓 Caesar Cipher decryption
* 🔑 Encryption key selection from **1–25**
* ⚔️ Brute-force attack simulation
* 🔄 Automatic testing of possible keys
* 🔍 Display of every decryption attempt
* ✅ Identification of the correct plaintext
* ⚠️ Basic English-text detection
* 📊 Real-time attack progress
* ⏱️ Attack time tracking
* 🔢 Attempt counter
* 🎚️ Adjustable attack speed
* ⏹️ Start/Stop attack controls
* 📱 Responsive web interface

---

## 🔐 What is a Caesar Cipher?

The **Caesar Cipher** is a classical substitution cipher in which each letter of the plaintext is shifted by a fixed number of positions in the alphabet.

For example, using a shift of `3`:

```text
A → D
B → E
C → F
...
X → A
Y → B
Z → C
```

Therefore:

```text
HELLO WORLD
```

becomes:

```text
KHOOR ZRUOG
```

The number `3` is the encryption key.

---

## ⚔️ What is a Brute-Force Attack?

A **brute-force attack** attempts to discover the correct key by trying all possible keys.

Since the Caesar Cipher has only **25 non-trivial possible shifts**, an attacker can easily test every key.

The simulator performs this process automatically:

```text
Encrypted Message
       ↓
    Try Key 1
       ↓
    Try Key 2
       ↓
    Try Key 3
       ↓
      ...
       ↓
   Try Key 25
       ↓
Correct Plaintext
```

This demonstrates why the Caesar Cipher is considered insecure for modern applications.

---

## ⚙️ How the Project Works

### Step 1 — Enter Plaintext

The user enters a message.

Example:

```text
HELLO WORLD
```

### Step 2 — Select Encryption Key

The user chooses a key between:

```text
1 – 25
```

For example:

```text
Key = 3
```

### Step 3 — Encrypt

The application applies the Caesar Cipher:

```text
HELLO WORLD
     ↓
KHOOR ZRUOG
```

### Step 4 — Start Brute-Force Attack

The simulated attacker starts testing possible keys.

For example:

```text
Key 1  → Attempt
Key 2  → Attempt
Key 3  → Attempt
Key 4  → Attempt
...
Key 25 → Attempt
```

### Step 5 — Analyze Results

Each result is evaluated and displayed.

The application can identify:

* ✅ **Correct Match**
* ⚠️ **Looks Like English**
* ❌ **Not English**

---

## 📊 Attack Statistics

While the attack is running, the interface displays:

| Statistic      | Description                   |
| -------------- | ----------------------------- |
| Attempts       | Number of keys tested         |
| Time           | Time taken by the attack      |
| Found          | Number of correct matches     |
| Progress       | Percentage of keys tested     |
| Current Key    | Key currently being tested    |
| Decrypted Text | Result of the current attempt |

---

## 🧠 English Text Detection

The simulator includes a simple heuristic to determine whether a decrypted message may resemble English.

It checks the decrypted text for common English words such as:

```text
THE
AND
FOR
ARE
YOU
NOT
ALL
CAN
ONE
OUR
```

This is only an **educational heuristic** and is not a complete cryptanalysis or language-processing system.

---

## 🛠️ Technologies Used

### HTML5

Used to build the structure of the web application.

### CSS3

Used for:

* User interface design
* Layout
* Buttons
* Progress bar
* Statistics cards
* Result highlighting
* Responsive design

### JavaScript

Used to implement:

* Caesar Cipher encryption
* Caesar Cipher decryption
* Brute-force attack
* Key testing
* English-text detection
* Attack timing
* Progress calculation
* Statistics
* DOM manipulation
* Start/Stop functionality

---

## 📁 Project Structure

```text
CaesaCipher-Brute-Force-Attack-Simulator/
│
├── CODE/
│   └── index.html
│
└── README.md
```

---

## 🚀 How to Run

This project is completely client-side and does not require:

* Backend server
* Database
* External libraries
* Package installation

### Method 1 — Open Directly

1. Clone the repository.
2. Open the project folder.
3. Navigate to:

```text
CODE/index.html
```

4. Open `index.html` in a web browser.

### Method 2 — Using Visual Studio Code

1. Open the project in **Visual Studio Code**.
2. Open:

```text
CODE/index.html
```

3. Run it in your browser.

You can also use the **Live Server** extension for a local development server.

---

## 🧪 Example

### Input

```text
Plaintext:
HELLO WORLD

Encryption Key:
3
```

### Encryption

```text
HELLO WORLD
     ↓
KHOOR ZRUOG
```

### Brute-Force Simulation

The application starts trying different keys:

```text
Key 1 → JGNNQ YQTNF
Key 2 → IFMMP XPSME
Key 3 → HELLO WORLD ✅
...
```

The correct plaintext is highlighted when the simulator reaches the appropriate key.

---

## 🎯 Objective

The main objective of this project is to demonstrate:

* How the Caesar Cipher encrypts data
* How encryption keys work
* How decryption can recover the original message
* How brute-force attacks work
* Why small key spaces are insecure
* How cryptographic concepts can be visualized using a web application

---

## 🎓 Learning Outcomes

After working with this project, you can understand:

* Fundamentals of cryptography
* Classical substitution ciphers
* Caesar Cipher encryption
* Caesar Cipher decryption
* Brute-force attacks
* Exhaustive key searching
* Key-space security
* Basic cryptanalysis concepts
* JavaScript algorithm implementation
* DOM manipulation
* Interactive web development

---

## ⚠️ Limitations

This project is intended for **educational purposes only**.

Current limitations include:

* Only the Caesar Cipher is implemented.
* The brute-force attack checks keys from **1 to 25**.
* English detection uses a basic word-based heuristic.
* It is not a complete cryptanalysis system.
* The exact correct-match check uses the original plaintext stored by the application.
* It should not be used to protect confidential or sensitive information.

---

## 🔒 Security Note

The Caesar Cipher is **not secure for real-world communication** because its key space is extremely small.

Modern secure communication systems use significantly stronger cryptographic algorithms with much larger key spaces and carefully designed security properties.

This project should therefore be considered a **cryptography learning and visualization tool**, not a security product.

---

## 📚 Concepts Demonstrated

```text
Cryptography
     │
     ├── Caesar Cipher
     │      ├── Encryption
     │      └── Decryption
     │
     └── Cryptanalysis
            │
            └── Brute-Force Attack
                   ├── Key Testing
                   ├── Plaintext Recovery
                   └── Result Analysis
```

---

## 👨‍💻 Author

**Gautam Bisht**

GitHub: [@Gautambisht98](https://github.com/Gautambisht98)

---

## ⭐ Acknowledgement

This project was created as an educational implementation to understand the working principles of **classical cryptography and brute-force attacks** through an interactive web interface.

---

## ⭐ Support

If you found this project useful for learning, consider giving the repository a **star ⭐**.
