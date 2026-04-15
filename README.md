# 🧩 Sudoku Solver using CSP (Constraint Satisfaction Problem)

## 📌 Overview

This project implements a **Sudoku solver** using **Constraint Satisfaction Problem (CSP)** techniques. The solver is designed to handle puzzles of varying difficulty (easy → very hard) using advanced AI search strategies.

---

## 🚀 Features

* ✅ Backtracking Search
* ✅ Forward Checking
* ✅ AC-3 Algorithm (Arc Consistency)
* ✅ MRV (Minimum Remaining Values) Heuristic
* ✅ Step & Backtrack Counting (for performance analysis)
* ✅ Supports multiple difficulty levels

---

## 🧠 Algorithms Used

### 1. Backtracking Search

A depth-first search approach that assigns values to variables and backtracks when constraints are violated.

### 2. Forward Checking

After assigning a value, it removes inconsistent values from neighboring variables' domains.

### 3. AC-3 (Arc Consistency)

Ensures that for every pair of variables, their domains remain consistent throughout the solving process.

### 4. MRV Heuristic

Selects the variable with the smallest domain to reduce the branching factor and improve efficiency.

---

## 📂 Project Structure

```
.
├── sudoku_solver.py
├── README.md
```

---

## 📥 Input Format

Each Sudoku puzzle is represented as a list of 9 strings:

* Each string = one row
* '0' represents an empty cell

Example:

```
530070000
600195000
098000060
800060003
400803001
700020006
060000280
000419005
000080079
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/sudoku-csp-solver.git
cd sudoku-csp-solver
```

2. Run the solver:

```bash
python sudoku_solver.py
```

---

## 📊 Example Output

```
Solving hard.txt...

Initial Puzzle:
3 0 0 0 0 0 0 0 0
...

Solved Puzzle:
3 4 1 6 8 2 9 5 7
...

Total Steps: 2451
Total Backtracks: 312
```

---

## 📈 Performance Analysis

| Difficulty | Steps     | Backtracks |
| ---------- | --------- | ---------- |
| Easy       | Low       | Low        |
| Medium     | Moderate  | Moderate   |
| Hard       | High      | High       |
| Very Hard  | Very High | Very High  |

> Note: Exact numbers may vary depending on system and implementation details.

---

## 💡 Key Learnings

* CSP techniques significantly reduce brute-force search
* AC-3 improves efficiency by pruning invalid domains early
* Heuristics like MRV drastically improve performance

---

## 🔧 Future Improvements

* Implement Least Constraining Value (LCV)
* Add GUI visualization
* Benchmark against other solving strategies
* Add puzzle generator

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork this repo and submit a pull request.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

Your Name

---

## ⭐ If you like this project

Give it a star on GitHub ⭐
