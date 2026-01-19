# ♟️ Chess System: Enterprise-Level OOP Application

> **A complete Chess Logic Engine implemented in Java**
> *Stack: Java (JDK) · Software Design Patterns · Custom Exception Framework*

This project is a full-featured Chess System, architected to demonstrate advanced mastery of **Software Engineering principles**. It goes beyond a simple game by implementing a decoupled, modular structure where the board mechanics are separated from the specific rules of chess.

---

## 🏗️ System Architecture

The application is built using a layered approach, ensuring that logic is encapsulated and the system remains easily extensible.

### Key Architectural Layers:

* **Boardgame Layer:** A generic engine for managing grids (`Board`), positions (`Position`), and generic game pieces (`Piece`). This demonstrates the principle of **Reusability**.
* **Chess Layer:** A specialized domain layer that implements official international chess rules. It handles complex game states including:
* **Special Moves:** Castling (Roque), En Passant, and Pawn Promotion.
* **Logic Checkers:** Check and Checkmate detection algorithms.
* **Turn Management:** Orchestrated by the `ChessMatch` controller.



### Applied Design Principles:

* **Polymorphism:** The system uses a base `ChessPiece` class, allowing specific piece logic (e.g., `King`, `Queen`, `Knight`) to be determined dynamically at runtime.
* **Encapsulation:** Rigorous use of access modifiers to protect the integrity of the board state.
* **Custom Exception Handling:** Implementation of a specialized hierarchy (`BoardException` -> `ChessException`) to manage game-specific errors gracefully.

---

## 🛠️ Technical Highlights

* **Logic Matrix Engine:** Every piece calculates its own "Possible Moves" matrix, considering obstacles, capture opportunities, and its unique movement patterns.
* **Move History & Piece Tracking:** Maintains real-time lists of captured pieces and pieces currently on the board.
* **ANSI Console UI:** A custom CLI interface that utilizes ANSI color codes to provide a clear and visually distinct representation of the board directly in the terminal.

---

## 🚀 How to Run

### Prerequisites

* [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/downloads/) (Version 8 or higher).

### Installation and Execution

1. **Clone the repository:**
```bash
git clone https://github.com/PauloRaphael/Chess-System-Java.git

```


2. **Navigate to the `src` folder.**
3. **Compile the application:**
```bash
javac application/Program.java

```


4. **Start the game:**
```bash
java application/Program

```

---

**Author:** [Paulo Raphael](https://www.google.com/search?q=https://github.com/PauloRaphael)
*Automation Engineer specializing in Hyperautomation & Enterprise Architecture.*
