# 🐛 Debugging Prompts

Prompts for using GPT as a debugging assistant while learning software development.

## 1. Find the Bug

```text
Analyze this code and find the bug.

Please:
1. Identify the problem
2. Explain why it happens
3. Show the corrected code
4. Explain the fix in simple terms

Code:
[PASTE CODE HERE]
```

## 2. Explain an Error Message

```text
I am a beginner programmer. Explain this error message in simple terms.

Tell me:
1. What the error means
2. What usually causes it
3. How I can fix it
4. How I can prevent it in the future

Error:
[PASTE ERROR HERE]
```

## 3. Code Runs but Gives Wrong Output

```text
This code runs without errors, but the output is not what I expect.

Expected output: [DESCRIBE WHAT YOU EXPECTED]
Actual output: [DESCRIBE WHAT YOU GOT]

Please:
1. Walk through the logic step by step to find where it diverges from what I expect
2. Identify the root cause
3. Show the corrected code
4. Explain the fix in simple terms

Code:
[PASTE CODE HERE]
```

## 4. Rubber-Duck Debugging (Step-by-Step Trace)

```text
Act as a rubber duck debugging partner. Do not fix my code yet.

Instead, walk through this code line by line and ask me questions to help me
figure out the bug myself. Point out what each section is supposed to do,
and prompt me to check my assumptions before we move on to the next part.

Code:
[PASTE CODE HERE]
```

## 5. Diagnose Slow / Inefficient Code

```text
This code works, but it feels slow or inefficient.

Please:
1. Identify parts of the code that are likely causing performance issues
2. Explain why they are slow (e.g. unnecessary loops, repeated calculations, inefficient data structures)
3. Suggest a more efficient approach
4. Show the improved code

Code:
[PASTE CODE HERE]
```
