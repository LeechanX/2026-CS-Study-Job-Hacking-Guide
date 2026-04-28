# Java OOD & Design Patterns: USYD COMP9103 & UNSW COMP2511 Mastery Guide

This repository provides industrial-grade guidance for students enrolled in Java-based Object-Oriented Design (OOD) courses at the University of Sydney (USYD) and the University of New South Wales (UNSW). 

In 2026, the evaluation criteria for COMP9103 and COMP2511 have shifted significantly towards architectural elegance rather than simple functional correctness. To achieve a High Distinction (HD), students must demonstrate a profound understanding of SOLID principles, Design Patterns, and rigorous Unit Testing.

---

## 1. The HD Standard: Why Functional Code is Not Enough

In premium CS programs, "code that works" is merely a baseline. Tutors and automated marking systems now prioritize:

* **Low Coupling & High Cohesion:** Are your classes tightly intertwined, or are they modular?
* **Extensibility:** Can your system handle new requirements without modifying existing source code?
* **Formal Verification:** Does your JUnit suite cover edge cases, or only the "happy path"?

---

## 2. Core SOLID Principles in Practice

Understanding the SOLID acronym is easy; implementing it in a complex assignment like a "Dungeon Crawler" or "Evolution Simulator" is where most students fail.

### Dependency Inversion Principle (DIP)
High-level modules should not depend on low-level modules. Both should depend on abstractions.
* **Bad Practice:** Hard-coding a specific Database or Logger class directly inside your Manager class, making it impossible to switch components.
* **HD Practice:** Utilizing Interface Injection via constructors to allow for seamless swapping of implementations during runtime or testing.

### Open-Closed Principle (OCP)
Software entities should be open for extension but closed for modification.
* **Practical Implementation:** Implementing new features by adding new classes that implement an existing interface, rather than rewriting core engine logic.

---

## 3. Essential Design Patterns for USYD/UNSW Assignments

Based on our analysis of the latest syllabi, the following behavioral patterns are critical for High Distinction:

### Strategy Pattern
This is the gold standard for handling multiple algorithm variations. Instead of using massive conditional branches, you encapsulate each behavior into its own class. This is frequently used for different AI movement logics or varying payment gateways in Java assignments.

### Observer Pattern
Crucial for UI-to-Model communication. It allows a subject to notify multiple observers (like a Map Renderer or an Achievement Tracker) automatically whenever its state changes, ensuring a decoupled architecture.

### State Pattern
Ideal for managing complex object lifecycles, such as a Player character transitioning between Invincible, Normal, or Stunned states. This pattern replaces messy switch-case blocks with clean, state-specific object transitions.

---

## 4. Industrial Testing Standards with JUnit 5

A robust assignment must be backed by a comprehensive testing suite. Our industrial standards include:

* **Boundary Value Analysis:** Rigorous testing of the absolute minimum and maximum limits of inputs.
* **Component Isolation:** Using Mocking frameworks to isolate the unit under test by simulating external dependencies.
* **Regression Assurance:** Ensuring that every new commit does not break existing functionality through automated test suites.

---

## 5. Architectural Refactoring & Plagiarism Defense (MOSS)

Modern plagiarism detection systems like MOSS analyze the Abstract Syntax Tree (AST). Simply renaming variables or moving code blocks is ineffective in 2026. 

Our approach at **lomo 留学CS辅导** involves:

* **Topological Restructuring:** Completely changing the execution flow and method call hierarchy.
* **Data Layout Transformation:** Redesigning how objects interact and store data at a structural level.
* **Logic Translation:** Re-implementing algorithms using different paradigms, such as converting deep recursion into iterative stack-based logic.

---

## 6. Professional Support

If you are struggling with complex OOD concepts or facing a tight deadline for your Java projects, our team of active SDEs is here to help. We provide:

1. **1-on-1 Architectural Audits**
2. **Logic Refactoring & Debugging**
3. **Comprehensive Code Walkthroughs for Oral Defense Preparation**

**Official Website:** [lomo 留学CS辅导](https://weilongcsdx.com)

---

*Disclaimer: All provided guides and architectural insights are for educational purposes. We strictly adhere to academic integrity standards while providing professional industry-level mentorship.*