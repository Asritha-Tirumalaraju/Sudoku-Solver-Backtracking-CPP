🧩 Sudoku Solver in C++

This project is a C++ implementation of a **9×9 Sudoku solver** that uses a **backtracking algorithm** to compute solutions efficiently.  
It is designed with a strong focus on **correctness, input validation, and structured logic**.
🚀 Highlights

1. Backtracking Algorithm
  Explores possible values using a depth-first approach and reverses decisions when constraints are violated.

 2.Input Validation
  Ensures the initial puzzle follows Sudoku rules before attempting to solve it.

3.Efficient Grid Handling
  Uses mathematical indexing to quickly access and validate 3×3 sub-grids.

4.Readable Output
  Prints the Sudoku board in a clear and organized format.

🧠 How the Program Works
🔁 Solving Strategy

The solver:
●Searches for empty cells (`0`)
●Attempts values from **1 to 9**
● Checks validity before placing a number
●Continues recursively until the grid is complete

If a number leads to an invalid state, the algorithm backtracks and tries a different value.


 ✅ Grid Validation

Before solving, the program verifies that:
●Each row contains unique numbers (excluding zeros)
●Each column has no duplicates
● Each 3×3 sub-grid follows Sudoku rules

This avoids wasting time on unsolvable inputs.
 📍 Sub-Grid Calculation

●To locate a 3×3 box, the program computes:

 Row start → `(row / 3) * 3`  
Column start → `(col / 3) * 3`  

This allows fast validation within sub-grids.

---

🛠️ Getting Started## 

### Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/sudoku-solver-cpp.git
```

### Compile the code
```bash
g++ main.cpp -o sudoku
```

### Run the program
```bash
./sudoku
```

---

## 📂 Files Included

```
main.cpp   -> Contains the full implementation
README.md  -> Project documentation
```

---

## 📥 Input Guidelines

- Provide 9 rows with 9 numbers each
- Use `0` to represent empty cells

---

## 📤 Program Output

- Displays the entered Sudoku grid
- Shows the solved puzzle (if possible)
- Prints appropriate error messages for:
  - Invalid input
  - Rule violations
  - No solution cases



