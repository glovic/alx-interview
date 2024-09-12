# 0x07. Rotate 2D Matrix

This project involves rotating a given n x n 2D matrix by 90 degrees clockwise. The task focuses on performing the operation in place without returning anything.

## Tasks :page_with_curl:

* **0. Rotate 2D Matrix**
  * **[0-rotate_2d_matrix.py](./0-rotate_2d_matrix.py), [main_0.py](./main_0.py):** Given an n x n 2D matrix, rotate it 90 degrees clockwise. The matrix must be edited **in-place**.
  
    * **Prototype:**
      ```python
      def rotate_2d_matrix(matrix):
      ```

    * **Example:**
      ```python
      #!/usr/bin/python3
      """
      Test 0x07 - Rotate 2D Matrix
      """
      rotate_2d_matrix = __import__('0-rotate_2d_matrix').rotate_2d_matrix

      if __name__ == "__main__":
          matrix = [
              [1, 2, 3],
              [4, 5, 6],
              [7, 8, 9]
          ]

          rotate_2d_matrix(matrix)
          print(matrix)
      ```

    * **Output:**
      ```bash
      jessevhedden$ ./main_0.py
      [[7, 4, 1],
       [8, 5, 2],
       [9, 6, 3]]
      jessevhedden$
      ```
