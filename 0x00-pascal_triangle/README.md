# Pascal's Triangle

This project involves creating a function to generate Pascal's Triangle up to a given number of rows. Pascal's Triangle is a triangular array of binomial coefficients.

## Task :page_with_curl:

* **0. Pascal's Triangle**
  * [0-pascal_triangle.py](./0-pascal_triangle.py): Python function that returns a list of lists of integers representing Pascal’s Triangle of `n` rows.
  * Usage: `python3 0-pascal_triangle.py`
  * Returns an empty list if `n <= 0`.
  * You can assume `n` will always be an integer.

### Example Usage

1. **Script**: `0-main.py`
   ```python
   #!/usr/bin/python3
   """
   0-main
   """
   pascal_triangle = __import__('0-pascal_triangle').pascal_triangle

   def print_triangle(triangle):
       """
       Print the triangle
       """
       for row in triangle:
           print("[{}]".format(",".join([str(x) for x in row])))

   if __name__ == "__main__":
       print_triangle(pascal_triangle(5))

