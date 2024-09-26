# Island Perimeter

This project focuses on creating a function to calculate the perimeter of an island represented by a grid. The grid consists of water and land cells, where water is denoted by `0` and land by `1`.

## About Project

- The function `island_perimeter(grid)` returns the perimeter of the island described in the grid.
- The grid is a list of lists of integers:
  - `0` represents water.
  - `1` represents land.
- Each cell in the grid is a square with a side length of `1`.
- Cells are connected horizontally or vertically (not diagonally).
- The grid is rectangular, with its width and height not exceeding `100`.
- The grid is completely surrounded by water.
- There is only one island (or nothing).
- The island does not have "lakes" (water inside that isn’t connected to the water surrounding the island).

## Tasks

* **0. Island Perimeter**
  * **File:** [0-island_perimeter.py](0-island_perimeter.py)
  * **Function:** `def island_perimeter(grid):`
    - This function calculates the perimeter of the island.
    - **Usage:**
      ```python
      grid = [
          [0, 0, 0, 0, 0, 0],
          [0, 1, 0, 0, 0, 0],
          [0, 1, 0, 0, 0, 0],
          [0, 1, 1, 1, 0, 0],
          [0, 0, 0, 0, 0, 0]
      ]
      print(island_perimeter(grid))  # Output: 12
      ```

## Example

Here is an example of how to use the function:

```python
#!/usr/bin/python3
"""
0-main
"""
island_perimeter = __import__('0-island_perimeter').island_perimeter

if __name__ == "__main__":
    grid = [
        [0, 0, 0, 0, 0, 0],
        [0, 1, 0, 0, 0, 0],
        [0, 1, 0, 0, 0, 0],
        [0, 1, 1, 1, 0, 0],
        [0, 0, 0, 0, 0, 0]
    ]
    print(island_perimeter(grid))  # Output: 12

