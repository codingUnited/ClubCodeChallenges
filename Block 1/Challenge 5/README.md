# Coding Challenge: “Port & Fix” — Rescue an Old C++11 App

## Overview

You’re given a small, buggy C++11 console application with little to no documentation. Your job is to:

1. Reverse-engineer what it does,
2. Fix the bugs, and
3. Rewrite the app in another language of your choice: Java / JavaScript / PHP / C# / Go / Python.

Keep the original functionality (feature parity), but produce a modern, maintainable implementation.

---

## Learning Goals

- Reading/understanding legacy code with minimal docs
- Debugging and writing tests to pin down behavior
- Designing a clean architecture in a new language
- Shipping a small, production-ready CLI or web-miniapp

---

## Starter Assets

- Legacy repo (C++11) with:
  - Source files (buggy)

Note: Building/running the C++11 version may be annoying—by design. That’s part of the challenge.

---

## Requirements

### Functional

- Maintain feature parity with the legacy behavior (as discovered by tests you write and by exploring the app).
- For CLI apps: expose the same core commands/flags.
- Correct the observable wrong behaviors (logic errors, edge cases).

### Non-Functional

- Clear README with: problem summary, how to run, assumptions, and decisions.
- Automated tests covering core logic + at least 3 edge cases you discovered.
- Error handling and helpful messages for bad inputs.
- Basic logging at useful points (debug/info or equivalent).
