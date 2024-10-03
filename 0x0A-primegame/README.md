# Prime Game ReadMe

For this project, I leverage mine understanding of prime numbers, game theory, and algorithm optimization to solve a competitive game scenario. The challenge involves determining the winner of a game based on the strategic removal of prime numbers and their multiples from a set of consecutive integers.


## Game Rules

- The game begins with a set of consecutive integers starting from 1 up to a number `n`.
- Maria goes first and picks a prime number from the set.
- Once a prime number is chosen, both that prime and all its multiples are removed from the set.
- Ben then takes his turn and picks a remaining prime number.
- The game continues until no prime numbers remain.
- The player unable to make a move loses the round.

### Example:

For `x = 3` rounds with `nums = [4, 5, 1]`:

- **Round 1: `n = 4`**
  - Maria picks 2 (removes 2 and its multiple 4), leaving {1, 3}.
  - Ben picks 3 (removes 3), leaving {1}.
  - Maria has no moves left—Ben wins this round.

- **Round 2: `n = 5`**
  - Maria picks 2 (removes 2 and 4), leaving {1, 3, 5}.
  - Ben picks 3 (removes 3), leaving {1, 5}.
  - Maria picks 5 (removes 5), leaving {1}.
  - Ben has no moves left—Maria wins this round.

- **Round 3: `n = 1`**
  - No primes available—Ben wins by default.

## Task Description

You will implement the function `isWinner(x, nums)` where:
- `x` is the number of rounds.
- `nums` is an array where each element represents the number of integers (`n`) in the set for that round.


## Example Usage

Here's how you can test the `isWinner` function using `main_0.py`.

### Input:
In this example, the game runs for 5 rounds with the following values of `n`: `[2, 5, 1, 4, 3]`.

```python
#!/usr/bin/python3

isWinner = __import__('0-prime_game').isWinner

print("Winner: {}".format(isWinner(5, [2, 5, 1, 4, 3])))


### Output:
`Winner: Ben`

