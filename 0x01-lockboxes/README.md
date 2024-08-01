# 0x01. Lockboxes

This project involves developing a solution to determine if all boxes can be opened. Each box may contain keys to other boxes, and the goal is to unlock all the boxes starting from the first one, which is already unlocked.

## Task :page_with_curl:

* **0. Lockboxes**
  * [0-lockboxes.py](./0-lockboxes.py): Python function that determines if all boxes can be opened given a list of lists, where each list represents the keys in each box.
  * Usage: `python3 0-lockboxes.py`
  * Returns `True` if all boxes can be opened, else returns `False`.
  * The first box `boxes[0]` is unlocked initially.

### Example Usage

1. **Script**: `main_0.py`
   ```python
   #!/usr/bin/python3
   """
   main_0
   """
   canUnlockAll = __import__('0-lockboxes').canUnlockAll

   def print_result(result):
       """
       Print the result
       """
       print(result)

   if __name__ == "__main__":
       boxes1 = [[1], [2], [3], [4], []]
       print_result(canUnlockAll(boxes1))  # True

       boxes2 = [[1, 4, 6], [2], [0, 4, 1], [5, 6, 2], [3], [4, 1], [6]]
       print_result(canUnlockAll(boxes2))  # True

       boxes3 = [[1, 4], [2], [0, 4, 1], [3], [], [4, 1], [5, 6]]
       print_result(canUnlockAll(boxes3))  # False

