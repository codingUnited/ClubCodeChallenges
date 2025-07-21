# 🧩 Build Your Own JSON Parser

Welcome to Challenge 3 of the Coding Club Challenge Series: **Build Your Own JSON Parser**.

Building a JSON parser is a great way to learn about parsing techniques, which are foundational in everything from reading structured data formats to writing full programming language compilers.

---

## 📚 Why This Challenge?

Parsing is typically broken down into two main phases:

1. **Lexical Analysis** – Breaking raw text into meaningful chunks called _tokens_.
2. **Syntactic Analysis** – Matching those tokens to a grammar to build meaning.

If you want to go deeper, consider reading the [Dragon Book](https://en.wikipedia.org/wiki/Compilers:_Principles,_Techniques,_and_Tools) — the definitive guide to compiler construction.

---

## 🧠 What is JSON?

[JSON (JavaScript Object Notation)](https://www.json.org/json-en.html) is a lightweight data-interchange format. It’s used everywhere — from APIs to configuration files.

- Formal Spec: [IETF JSON Standard](https://tools.ietf.org/html/std90)
- Visual Guide: [JSON.org](https://www.json.org/json-en.html)

---

## 🛠 Challenge Overview

You will build a JSON parser that evaluates JSON strings from the command line and reports whether they are valid or not.

Your parser will evolve in **steps**, increasing in complexity.

### ✅ Step 0 — Environment Setup

- Choose your programming language and IDE.
- Set up your environment.
- Download the test data (for Steps 1–4) from:  
  📦 [tests.zip (DropBox)](https://www.dropbox.com/scl/fi/9vdw9wd9r5gw0azzehnzy/tests.zip?rlkey=mlp42ah3wmdav9w9kvekgk2fp&dl=0)

### 🟢 Step 1 — Empty Objects & Invalid Input

Your goal is to:
- Accept a valid empty JSON object (`{}`)
- Reject invalid JSON
- Return `0` for valid, `1` for invalid

📂 Test cases: `tests/step1/`

---

### 🟡 Step 2 — Key/Value Pairs (Strings Only)

Your parser should now handle:
```json
{ "key": "value" }
```
📂 Test cases: tests/step2/

### 🔴 Step 3 — Basic Types
Support additional JSON values:

- true, false, null

- numbers (integers, floats)

Example:
```json
{
  "key1": true,
  "key2": false,
  "key3": null,
  "key4": "value",
  "key5": 101
}
```
📂 Test cases: tests/step3/

### 🟣 Step 4 — Objects & Arrays

Support nesting and array values:
```json
{
  "key": "value",
  "key-n": 101,
  "key-o": {},
  "key-l": []
}
```
📂 Test cases: tests/step4/

### 🧠 Step 5 (Hard/Leet Only) — Advanced Structures
These test cases are only for participants attempting Hard or Leet levels. They include:

- Deeply nested objects/arrays

- Edge-case formatting

- Complex combinations

📂 Step 5 tests provided in your earlier upload or shared via internal drop.