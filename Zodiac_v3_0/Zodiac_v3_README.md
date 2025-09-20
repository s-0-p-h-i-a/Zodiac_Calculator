# Zodiac Sign Calculator

**Version:** v3.0  
**Date:** 2025-08-26

This version introduces **functions** for calculation and string mapping, plus **loop-based input validation**. It represents the program’s transition from a single-block `main()` into a modular structure.

---

## 🔍 Overview

The user inputs their **birth day and month**, and the program returns:

- Their **zodiac sign**
- Its **element** (Fire, Earth, Air, Water)
- Its **modality** (Cardinal, Fixed, Mutable)

The program now uses functions for both numeric calculations and string conversions, making the main logic easier to follow/maintain and reducing repeated logic.

---

## 🧱 Features

- Input validation with **do/while loops** until valid values are entered
    
- Functions for:
    
    - `defineMonthEnd()` → last day of each month
    - `defineSignStart()` + `defineSign()` → zodiac sign calculation
    - `defineElement()` + `defineModality()` → numeric classification
    - `defineSignName()`, `defineElementName()`, `defineModalityName()` → string output mapping

- Uses **switch** and **if/else** branches inside functions to handle conditions
    
- Decorative console output
    

------

## 🔁 v2.1 → v3.0 Trajectory

This version is about **refactoring into functions** and improving input handling.

| Area             | v2.1 Approach                | v3.0 Improvements                                    |
| ---------------- | ---------------------------- | ---------------------------------------------------- |
| Input validation | Single checks, limited retry | `do…while` loops for continuous prompting            |
| Sign calculation | Month-specific hardcoding    | Generalised offset logic with function encapsulation |
| Structure        | All logic in `main()`        | Modular functions for calc + string mapping          |
| Readability      | Inline branching             | Streamlined top-down main flow                       |

---
## 🧠 Learning Goals

This version focused on:

- Practicing **function creation and use**
    
- Recognising natural module boundaries in existing code
    
- Understanding how to reduce complexity in `main()`
    
- Building confidence in structuring C++ programs beyond a single block

---

## 🚧 Limitations & Future Work

- Still no leap year validation
    
- Input still limited to integer values (`cin.fail()` handling not yet applied)
    
- Switches and if/else remain verbose — arrays will be a better fit in future
    
- Sign calculation logic works but could be simplified further with data structures

---
## Next steps:

- Introduce **`cin.fail()` handling** for invalid inputs
- Experiment with **arrays** or **structs** to reduce repetition
- Continue testing new sign calculation logic against edge cases

---

## 🗃️ Files

- `zodiac_v3.cc`: Source code for version 3.0
    
- `devlog_v3.md`: Development log for function refactor and validation changes

---