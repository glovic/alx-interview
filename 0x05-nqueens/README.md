# 0x05. N Queens

This project involves solving the N Queens problem using a backtracking algorithm. The goal is to place N non-attacking queens on an N×N chessboard. The program should handle various input scenarios and provide solutions for valid inputs.

## Tasks :page_with_curl:

* **0. N Queens**
  * **[0-nqueens.py](./0-nqueens.py):** Write a Python program that solves the N Queens problem. The program should print every possible solution for placing N non-attacking queens on an N×N chessboard.
    * **Usage:** The program should be executed with the following command:
      ```bash
      ./0-nqueens.py N
      ```
    * **Input Validation:**
      * If the user provides the wrong number of arguments, the program should print:
        ```bash
        Usage: nqueens N
        ```
        and exit with status 1.
      * If N is not an integer, the program should print:
        ```bash
        N must be a number
        ```
        and exit with status 1.
      * If N is less than 4, the program should print:
        ```bash
        N must be at least 4
        ```
        and exit with status 1.
    * **Output:** The program should print every possible solution to the problem, with one solution per line, in the following format:
      ```python
      [[row, col], [row, col], ..., [row, col]]
      ```
