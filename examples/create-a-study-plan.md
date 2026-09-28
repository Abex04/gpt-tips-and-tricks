# Example: Create a Study Plan

**Prompt from:** [`study-prompts.md`](../prompts/study-prompts.md) → "Create a Study Plan"

> **Note:** GPT's full response was a complete 28-day plan with exercises for every day. This is a shortened excerpt showing the structure and a few sample days. The wording below is GPT's own.

## Prompt used

```text
Create a realistic study plan for learning Python.

My current level: BEGINNER
Time available each day: 1 hour
Goal: Build a small project after 4 weeks

Break the plan into small daily tasks and include practice exercises.
```

## GPT's response (excerpt)

Since you're a beginner with 1 hour per day, the goal should be **consistency + practice**, not trying to learn all of Python in 4 weeks.

By the end of the 4 weeks, you should be able to build a small command-line project using variables, conditions, loops, functions, lists/dictionaries, and basic file handling.

### Your daily 1-hour structure

- **15 min**: Learn a concept
- **30 min**: Write code yourself
- **10 min**: Practice exercises
- **5 min**: Review what you learned

**Important:** Don't just read the examples. Type them yourself and deliberately make mistakes. Debugging is part of learning programming.

### Week 1: Python Fundamentals

**Goal:** Understand Python's basic building blocks.

**Day 2: Variables and data types**

Learn: variables, `str`, `int`, `float`, `bool`, `type()`

```python
name = "Alex"
age = 20
height = 1.75
student = True

print(name)
print(age)
print(type(age))
```

Exercise: create variables for your name, your age, your favorite number, and whether you are a student. Then print them.

**Day 7: Review + Mini Project**

Don't learn anything new today. Review Days 1-6. Then build a **Number Guessing Game**: the computer chooses a number, and the user tries to guess it. Your program should tell the user "Too high", "Too low", or "Correct!"

### Week 4: Build Your First Real Project

**Goal:** Put everything together.

For your first project, I recommend a **Command-Line To-Do Manager** because it's achievable in four weeks but still teaches useful programming concepts.

```text
====================
     TO-DO APP
====================

1. Add task
2. View tasks
3. Complete task
4. Delete task
5. Quit

Choose an option:
```

### Your 4-week progress

| Week | Main Topics | Result |
|---|---|---|
| 1 | Variables, input, operators, conditions | Basic Python programs |
| 2 | Loops, lists, dictionaries | Programs that process data |
| 3 | Functions, return, debugging | Better-organized programs |
| 4 | Project development | Complete To-Do App |

### One rule I'd strongly recommend

Don't spend your entire hour watching tutorials. For every 15 minutes of learning, spend at least 30 minutes actually writing code.

And when you get an error, don't immediately copy the solution. First ask yourself:

- What line caused the error?
- What was Python expecting?
- What did I actually give it?
- What can I change to fix it?

That habit will make you a much stronger programmer than simply memorizing Python syntax.

## Why this prompt works

Giving GPT three concrete constraints (your level, your daily time, and a goal) produces a plan sized to your real situation instead of a generic "learn Python" list. Ending the prompt with "include practice exercises" is what turns it from a reading list into something you can actually follow.
