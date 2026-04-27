# 🚦 Lab Experiment 2 — Traffic Light Simulation
### Subject: Web Engineering & Browser Languages (WEBL)
### Aim: Create a functional traffic light simulator using HTML, CSS, and JavaScript.

---

## 📁 Project Overview
This project simulates a traffic light system where a single button click triggers the transition between lights. It focuses on the use of JavaScript variables, control flow (if-else/switch), and event handling.

---

## ▶️ How to Run

1. **Locate the Folder:** Open the `Traffic-Light-Simulator` folder on your computer.
2. **Open index.html:** Right-click the `index.html` file and select **Open with** → **Chrome** (or any modern browser).
3. **Interact:** Click the **"Change Light"** button at the bottom of the traffic light to see the sequence in action.

---

# 📚 TERMINOLOGY & DEFINITIONS

---

## 🏗️ JavaScript Variables (`var`, `let`, `const`)

### 1. `var`
- **Scope:** Function-scoped.
- **Redeclaration:** Can be redeclared and updated within the same scope.
- **Hoisting:** Variables are hoisted to the top of their scope and initialized with `undefined`.
- **Usage:** Mostly used in legacy (older) code; now largely replaced by `let`.

### 2. `let`
- **Scope:** Block-scoped (only exists within `{ }`).
- **Redeclaration:** Cannot be redeclared in the same scope, but can be updated.
- **Usage:** Preferred for variables that need to change value during the program.

### 3. `const`
- **Scope:** Block-scoped.
- **Redeclaration:** Cannot be updated or redeclared once assigned.
- **Usage:** Used for values that should remain constant throughout the program (like references to HTML elements).

---

## 🔄 Control Loops (`for`, `while`, `do-while`)

### 1. `for` Loop
- **Best Use:** When you know the exact number of times you want to run the code.
- **Structure:** `initialization; condition; increment/decrement` are all in one line.

### 2. `while` Loop
- **Best Use:** When the number of iterations depends on a condition being true.
- **Structure:** Checks the condition **before** running the code inside.

### 3. `do-while` Loop
- **Best Use:** Similar to `while`, but guarantees the code runs **at least once** even if the condition is false.
- **Structure:** Checks the condition **after** executing the code block.

---

## ⚡ Events & Event Handling

### What is an Event?
An **event** is a signal that something has happened in the browser. Examples:
- A user clicking a button (`click`).
- A page finishing loading (`load`).
- A user typing in a text field (`input`).

### 1. Inline Event Handling
- Written directly inside the HTML tag: `<button onclick="changeLight()">`.
- **Pros:** Simple for tiny scripts.
- **Cons:** Hard to maintain, makes HTML messy, and separates logic poorly.

### 2. External Event Handling
- Written in a separate JavaScript file using `element.addEventListener('click', ...)` or by assigning to the property `element.onclick = ...`.
- **Pros:** Keeps HTML clean, allows multiple listeners on one element, and is the **professional standard**.

---

# ❓ VIVA QUESTIONS & ANSWERS

**Q1. What is the execution order of your traffic light?**
> The transition sequence is **Red → Green → Yellow → Red**.

**Q2. Why is `let` better than `var`?**
> `let` provides block scoping, which prevents variables from "leaking" outside of loops or if-statements, making the code safer and easier to debug.

**Q3. How did you change the color of the lights in JavaScript?**
> By manipulating the CSS properties of the elements. Usually, this is done by adding/removing a CSS class or changing the `style.backgroundColor` property based on the current state.

**Q4. What event is triggered when the button is clicked?**
> The `click` event is triggered.

**Q5. Can you reassign a value to a `const` variable?**
> No, trying to reassign a `const` variable will throw a `TypeError`.

---

## ✅ Conclusion
This experiment successfully demonstrated the integration of HTML structure, CSS styling, and JavaScript logic. By using variables to track states and event listeners to trigger transitions, we created an interactive simulation that follows standard programming patterns for state management.

---

*Lab Experiment 2 · WEBL Practical · Academic Year 2025–26*
