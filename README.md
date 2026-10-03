# 🔗 Simple Blockchain in Python

<p align="center">
  <b>A lightweight, educational implementation of a decentralized blockchain built from scratch in Python.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue.svg" alt="Python Version">
  <img src="https://img.shields.io/badge/Status-Completed-success.svg" alt="Status">
  <img src="https://img.shields.io/badge/Bootcamp-2024-orange.svg" alt="Bootcamp 2024">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
</p>

---

## 🚀 Overview

This repository features a minimal yet fully functional **Blockchain** data structure developed in Python. Designed as a capstone/demonstration project for the **2024 Python Bootcamp**, this project bridges core programming fundamentals with advanced decentralized data concepts, implementing cryptographic hashing, consensus mechanisms (Proof of Work), and immutable block linking.

---

## ✨ Core Features

*   **Immutable Ledger Architecture (`Block` class):** Stores cryptographic indices, timestamp logs, secure transaction lists, and previous hash references to ensure data integrity.
*   **Cryptographic Security (`SHA-256`):** Leverages Python's built-in `hashlib` to securely hash block data dictionaries serialized via JSON.
*   **Proof of Work Consensus (`PoW`):** Implements a difficulty-based mining algorithm requiring computational effort to append valid new blocks.
*   **Genesis Block Generation:** Automatically initializes the foundation of the chain with custom default hashes.
*   **Transaction Management:** Manages unconfirmed transaction queues and securely anchors verified data blocks onto the chain.

---

## 🛠️ Technologies Used

*   **Python 3.x** (Object-Oriented Programming, Decorators, Properties)
*   `hashlib` (SHA-256 cryptographic hashing)
*   `json` (Data serialization and dictionary sorting)
*   `time` (Timestamp generation for blocks)

---

## 📦 Code Structure & Architecture

The project is split into two foundational classes:

1.  **`Block`**: Represents individual blocks containing an index, a list of transactions, a timestamp, a unique hash, and the hash of the preceding block.
2.  **`Blockchain`**: Manages the entire chain lifecycle, handling validation, mining difficulty, proof-of-work validation, and transaction queuing.

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3 installed on your machine. No external package installations are required since the script relies entirely on Python's standard library.

### Running the Script

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. Navigate to the project directory and execute the script:
   ```bash
   python blockchain.py
   ```

---

## 💡 Example Usage

The script includes a built-in simulation that instantiates the blockchain, creates new transactions, mines a block via Proof of Work, and outputs the final block's details:

```python
# Initialize blockchain
a = Blockchain()

# Add transactions
a.new_transaction('sdf3453245dfsdf-1')
a.new_transaction('awerqw4564sdfb5-2')

# Mine a new block with the unconfirmed transactions
a.mine()

# Print the latest block information
len_bc = len(a.chain)
print(a.print_block(len_bc - 1))
```

---

## 🎯 Skills Highlighted (2024 Python Bootcamp)

*   **Object-Oriented Programming (OOP):** Implementation of clean classes, encapsulation, and `@property` decorators.
*   **Data Structures & Algorithms:** Managing arrays, queues, and cryptographic linking constraints.
*   **Problem Solving & Security:** Applying hashing functions and cryptographic puzzles (Proof of Work) to ensure data immutability.

---

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.
