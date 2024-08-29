# 0x05. N Queens

This project involves solving the N Queens problem using a backtracking algorithm. The goal is to place N non-attacking queens on an N×N chessboard. The program should handle various input scenarios and provide solutions for valid inputs.

## Tasks :page_with_curl:

* **0. N Queens**
  * **[0-nqueens.py](./0-nqueens.py):** Write a Python program that solves the N Queens problem. The program should print every possible solution for placing N non-attacking queens on an N×N chessboard.
    * **Usage:** The program should be executed with the following command:
      ```bash
      ./0-nqueens.py N
      ```
## Usage

\`\`\`bash
nqueens N
\`\`\`

- N is the number of queens.
- N must be an integer greater than or equal to 4.
- The program prints every possible solution to the problem in the format shown below.

\`\`\`bash
$ ./0-nqueens.py 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]
\`\`\`

Each inner list represents the coordinates of a queen on the NxN chessboard.

## Example

In this example, for a 4x4 chessboard, there are two possible solutions:

\`\`\`bash
$ ./0-nqueens.py 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]
\`\`\`

In the output, \`[0, 1]\` indicates a queen placed at the first row and the second column, and so on.
