![Views Counter](https://views-counter.vercel.app/badge?pageId=https%3A%2F%2Fgithub%2Ecom%2Fmesbahulalam%2Fnotepad-calculator&leftColor=000000&rightColor=0adb3f&type=total&label=Views&style=none)

# notepad-calculator
A fork of https://nekocalc.com/notepad-calculator

# Deployed Page
https://mesbahulalam.github.io/notepad-calculator/

# Notepad Calculator Dashboard
A dynamic, web-based notepad that doubles as a powerful real-time calculator. This tool allows you to write down notes, perform calculations, assign variables, and track totals seamlessly. All your notes are automatically saved to your browser's local storage, so you can pick up right where you left off.
# Features
 - Real-time Calculations: Performs calculations as you type.
 - Variable Assignment: Define variables and use them in subsequent calculations.
 - Smart Summation: Use keywords like total and subtotal to quickly calculate sums.
 - Note Management: Create, save, rename, and delete multiple notes.
 - Persistent Storage: Notes are saved in the browser's localStorage.
 - Responsive Design: A clean, modern interface that works on both desktop and mobile devices.
 - Copy to Clipboard: Easily copy the entire content of your notepad.
 - 
# Documentation
## Arithmetic Operators
The following operators are supported:
|**Operator**|**Description**|**Example**|
| :--------- | :-----------: | --------: |
| + | Addition          | 10 + 5 |
| - | Subtraction       | 10 - 5 |
| * | Multiplication    | 10 * 5 |
| / | Division          | 10 / 5 |
| ^ | Exponentiation    | 10 ^ 2 |
| of | Percentage of    | 10% of 50 |

# Usage Example
The example below demonstrates how to use variables, comments, and keywords to create a monthly budget.

```
# General Purpose Calculations

# '#' creates a comment, which is ignored by the calculator.
# Variables are defined with '='.
price = 150
quantity = 3
cost = price * quantity

# --- Using 'subtotal' ---
# 'subtotal' sums up all previous results and variable definitions
# since the last 'subtotal'. Here, it sums price(150), quantity(3), and cost(450).
first_subtotal = subtotal

# Using 'subtotal' on a line by itself resets the counter for the next section.
subtotal

# --- Continuing Calculations ---
discount_percent = 10%
discount_amount = cost * discount_percent
final_cost = cost - discount_amount

# This subtotal only includes the values since the last reset.
# It sums discount_percent, discount_amount, and final_cost.
second_subtotal = subtotal

# --- Using 'total' and 'totalvars' ---
# 'total' sums *all* results and definitions in the entire note.
grand_total = total

# 'totalvars' sums the current value of *all* defined variables.
# (price, quantity, cost, first_subtotal, discount_percent, etc.)
all_vars_total = totalvars
```

# Technical Stack
- **Frontend**: HTML, CSS, Vanilla JavaScript
- **Styling**: Tailwind CSS
- **Icons**: Feather Icons
- **Storage**: Browser Local Storage
- 
This project is self-contained in a single index.html file and requires no backend or build process to run.
