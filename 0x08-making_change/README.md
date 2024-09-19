# 0x08. Making Change

This project focuses on solving the "Making Change" problem by implementing an algorithm to determine the fewest number of coins needed to meet a given total.

## Tasks :page_with_curl:

### 0. Change comes from within

- **[0-making_change.py](./0-making_change.py):** Write a function that determines the fewest number of coins needed to meet a given amount of total.

\"\"\"
Main file for testing
\"\"\"

makeChange = __import__('0-making_change').makeChange

print(makeChange([1, 2, 25], 37))  # Output: 7
print(makeChange([1256, 54, 48, 16, 102], 1453))  # Output: -1

