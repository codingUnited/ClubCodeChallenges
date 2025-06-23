# ✅ Templates/Checklists per Challenge Level

## 🟢 Easy Level – Checklist

**Goal:** Basic 2-number calculator

### Features to Check:

- Prompt user for first number

- Prompt user for operation (+, -, \*, /)

- Prompt user for second number

- Perform correct calculation

- Print result

### Example Test Case:

```python
# Input: 2 + 3
# Output: 5
```

---

## 🟡 Medium Level – Checklist

### Adds on top of Easy

### Features to Check:

- Gracefully handle non-numeric inputs (e.g., letters)

- Prevent divide-by-zero

- Support chained operations using previous result

- Clear/reset functionality (optional but common)

### Example Tests:

```python
# Input: 5 \* 2 → then + 3
# Output: 10 → then 13

# Input: a + 2 → Error message
```

---

## 🔴 Hard Level – Checklist

### Adds on top of Medium

### Features to Check:

- Accept full math expressions as input (e.g., 3 + 4 \* 2)

- Parse and evaluate with correct order of operations

- Handle parentheses (5 + 2) \* 3

- Handle exponents: 2^3 or \*\*

- Support square root: √16 or sqrt(16)

### Example Tests:

```python
# Input: 2 \* (3 + 4)
# Output: 14

# Input: 3^2 + √16
# Output: 9 + 4 = 13
```

---

## 🟣 Leet Level – Checklist

### Adds on top of Hard

### Features to Check:

- Recognize trig functions: sin(30), cos(pi)

- Support scientific notation: 1e-3 + 2.5e2

- Implement basic command system:

- help, clear, exit, history

- Optional: Output rounding / fixed decimal format

### Example Tests:

```python
# Input: sin(0)
# Output: 0.0

# Input: 1e2 + 1e1
# Output: 110.0

# Input: clear
# Output: Previous result cleared.
```
