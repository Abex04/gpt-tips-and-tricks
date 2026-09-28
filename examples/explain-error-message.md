# Example: Explain an Error Message

**Prompt from:** [`debugging-prompts.md`](../prompts/debugging-prompts.md) → "Explain an Error Message"

## Prompt used

```text
I am a beginner programmer. Explain this error message in simple terms.

Tell me:
1. What the error means
2. What usually causes it
3. How I can fix it
4. How I can prevent it in the future

Error:
TypeError: can only concatenate str (not "int") to str
```

## GPT's response

### 1. What the error means

Python is trying to join text (`str`) with a number (`int`), but it doesn't know how to do that automatically.

```python
age = 20
print("I am " + age + " years old")
```

Python sees `"I am " + 20`. The first value is a string, while `20` is an integer.

### 2. What usually causes it

```python
name = "John"
age = 20

print("My name is " + name + " and I am " + age)
```

`name` is a string, so `"My name is " + name` works. But `age` is an integer, so `"and I am " + age` gives the error.

### 3. How to fix it

**Option A: Convert the number to a string**

```python
age = 20
print("I am " + str(age) + " years old")
```

**Option B: Use an f-string (recommended)**

```python
age = 20
print(f"I am {age} years old")
```

**Option C: Use `print()` with commas**

```python
age = 20
print("I am", age, "years old")
```

### 4. How to prevent it in the future

- String + String → works
- Number + Number → works
- String + Number → error

```python
"Hello " + "John"       # works
10 + 5                  # works
"Age: " + 20            # error
```

When combining text and variables, f-strings are a great habit:

```python
name = "John"
age = 20
print(f"My name is {name} and I am {age} years old.")
```

**Simple rule:** think of strings as text and integers as numbers. If you see this error, look for a `+` and check whether you're combining text with a number.

## Why this prompt works

Asking for four separate parts (meaning, cause, fix, prevention) forces the answer to go beyond "here's the fix" and actually teach the concept, which is the point when you're learning.
