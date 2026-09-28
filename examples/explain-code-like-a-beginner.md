# Example: Explain Code Like a Beginner

**Prompt from:** [`coding-prompts.md`](../prompts/coding-prompts.md) → "Explain Code Like a Beginner"

> **Note:** GPT's full response was much longer (it explained all 7 lines). This is a shortened excerpt showing the most instructive parts. The wording below is GPT's own.

## Prompt used

```text
Explain this code step by step as if I am a beginner learning programming.

For each important line, explain:
1. What it does
2. Why it is needed
3. What would happen if it were removed or changed

Code:
def find_max(numbers):
    largest = numbers[0]
    for n in numbers:
        if n > largest:
            largest = n
    return largest

print(find_max([3, 7, 2, 9, 4]))
```

## GPT's response (excerpt)

The program's goal is simple: **find the largest number in a list of numbers.**

For the list `[3, 7, 2, 9, 4]`, the answer should be `9`.

### `largest = numbers[0]`

**What does it do?**

It takes the first number in the list and stores it in a variable called `largest`. Remember that Python lists start counting at 0:

```text
Index:     0  1  2  3  4
           ↓  ↓  ↓  ↓  ↓
Numbers:   3  7  2  9  4
```

**Why is it needed?**

We need some number to start comparing against. The program initially says: "I'll assume the first number is the largest." Then it checks whether the other numbers are bigger.

**What if we changed it?**

If you wrote `largest = 0`, it might work for a list of positive numbers. But it would fail for a list containing only negative numbers like `[-5, -2, -10]`. The program would incorrectly keep 0 as the largest number, even though 0 isn't in the list. That's why using `numbers[0]` is safer.

### `if n > largest:`

This is a condition. It asks: "Is the current number bigger than the largest number I've found so far?"

**What if we changed `>`?**

If you wrote `if n < largest:`, the program would be looking for the smallest number instead of the largest. So the direction of the comparison matters.

### Tracing the entire program

| Step | n | largest |
|---|---|---|
| Start | — | 3 |
| 1 | 3 | 3 |
| 2 | 7 | 7 |
| 3 | 2 | 7 |
| 4 | 9 | 9 |
| 5 | 4 | 9 |
| End | — | 9 |

### The big idea

```text
1. Start with the first number.
2. Assume it is the largest.
3. Look at each number.
4. Is this number bigger?
   Yes → remember it as the new largest.
   No  → keep the current largest.
5. After checking everything, return the largest.
```

## Why this prompt works

Asking "what would happen if it were removed or changed" for each line pushes GPT past describing the code and into explaining why each line exists. The `largest = 0` example above is exactly the kind of insight a beginner wouldn't think to ask about.
