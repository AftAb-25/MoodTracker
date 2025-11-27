# MoodTracker
# 🧠 MoodTracker Smart Contract (Beginner Project)

This is a **very simple beginner-level Solidity smart contract** that allows users to **store and read a mood** on the blockchain.  
It is perfect for students who are just starting with **Blockchain & Smart Contracts**.

---

## 📌 Project Idea

A **Mood Tracker** where:
- You can **set your mood** (like "happy", "sad", "excited")
- You can **read the saved mood**
- No inputs are required during deployment

---

## 🛠 Tech Used

- **Solidity** (Smart Contract Language)
- **Remix IDE** (For testing & deployment)

---

## 📄 Smart Contract Code

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract MoodTracker {

    // This variable stores the mood
    string public mood;

    // Function to set the mood
    function setMood(string memory _mood) public {
        mood = _mood;
    }

    // Function to get the mood
    function getMood() public view returns (string memory) {
        return mood;
    }
}
