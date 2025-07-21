# 🧱 Challenge 3 – Scoring Structure (Finalized)

## 🟢 Easy Level – Built-in JSON Parser + Unit Tests
 - ✅ Use language’s built-in JSON parser (json in Python, JSON.parse in JS, etc.)

- ✅ Implement unit tests that run against all steps (step0 to step4)

- 🎯 Goal: Understand I/O flow, test harnesses, and CLI usage

- 🧪 Tests must check both valid and invalid cases

- ✅ Exit codes: 0 for valid JSON, 1 for invalid

- 💯 Scoring: Full points if:

    - Runs all steps with correct output

    - Uses built-in parser

    - Has a working unit test suite

🔢 Score: 25 pts


## 🟡 Medium Level – First Principles Parsing
- ❌ No use of built-in JSON parsers (must write parser from scratch)

- ✅ Still implement unit tests against step 0 to step 4

- 🧠 Focus on building lexer/parser using string processing and logic

- 👨‍🏫 Teaches parsing fundamentals and data validation

- 💯 Scoring: Full points if:

    - Implements correct logic without JSON libraries

    - Unit tests pass most of step 0 to step 4 files

🔢 Score: 25 pts

## 🔴 Hard Level – Parser Coverage > 50%
- ✅ Must correctly parse 50% or more of all test cases

- ✅ From any level (step 0 to step 5)

- ✅ Uses first-principles parser (from Medium level)

- 💯 Scoring: Full points if:

    - Custom parser runs through automated test harness

    - 50%+ pass rate (based on exit codes)

🔢 Score: 25 pts

## 🟣 Leet Level – 100% Test Coverage
- 🎯 Full pass of all tests (valid/invalid, edge cases)

- ✅ Handles nesting, arrays, mixed types, formatting issues

- ✅ Must be entirely first-principles implementation

- 💯 Scoring: Full points if:

    - All test files return the correct status code

    - Parser has zero false positives/negatives

🔢 Score: 25 pts

### 📊 Total Points: 100
|Level	|Description	|Points|
|-------|---------------|------|
|Easy	|Built-in parser + unit test for all steps	|25|
|Medium	|No JSON libs, unit-tested parser	|25|
|Hard	|50%+ test case accuracy	|25|
|Leet	|100% test case accuracy	|25|