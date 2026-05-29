# 🎮 Quantum Duel

Quantum Duel is a simple two-player game built using Python and Qiskit to demonstrate basic quantum computing concepts through interactive gameplay.

Instead of traditional moves, players use **quantum gates** to change the state of a qubit. After both players make their moves, the qubit is measured using a quantum simulator and the result decides the winner of the round.

The game is designed to make quantum computing easier to understand in a practical and engaging way.

---

## 🧠 Quantum Concepts Used

### 1. Qubit
A qubit (quantum bit) is the basic unit of quantum computing.

Unlike a classical bit:
- **0 or 1** → classical bit
- **0 and 1 probabilistically** → qubit

---

### 2. Superposition
A qubit can exist in more than one state at the same time.

This creates probabilistic outcomes and makes the game less predictable than traditional games.

---

### 3. Quantum Measurement
After all moves are made, the qubit is measured.

Measurement collapses the quantum state into:
- **0**
- **1**

The measured result determines the round winner.

---

### 4. Interference
Some gate combinations affect how probabilities behave.

This means player choices can strengthen or cancel certain outcomes.

---

## ⚛️ Gates Used

### X Gate
- Flips the qubit
- **|0⟩ → |1⟩**
- **|1⟩ → |0⟩**

---

### H Gate (Hadamard)
- Creates superposition
- Gives the qubit a probability of measuring as 0 or 1

---

### Z Gate
- Applies a phase flip
- Changes interference without directly flipping the output

---

## 🎮 Game Rules

- The game is played by **2 players**
- Total rounds are played one at a time
- A fresh qubit is created every round
- Player order is randomized for fairness
- Each player selects **one gate**:
  - X
  - H
  - Z
- Both gates are applied to the qubit
- The qubit is measured using the simulator
- The measurement result decides the winner of that round:
  - More **1s** → Player A scores
  - More **0s** → Player B scores
- Final score after all rounds decides the game winner

---

## 🛠 Technologies Used

- **Python**
- **Qiskit**
- **Qiskit Aer**
- **Tkinter**

---

## ▶️ Run the Project

Install dependencies:

```bash
pip install qiskit
pip install qiskit-aer
