# Widgets and Classes Overview

## Widgets

### Expenses (`lib/widgets/expenses.dart`)
- **Type:** Stateful widget
- **Description:** Manages the list of expenses and displays the main UI.
- **Dependencies:** 
  - `ExpensesList`
  - `Chart`

### ExpensesList (`lib/widgets/expenses_list/expenses_list.dart`)
- **Type:** Stateless widget
- **Description:** Displays a list of expenses.
- **Dependencies:** 
  - `ExpenseItem` (for each expense item)

### NewExpense (`lib/widgets/expenses_list/new_expense.dart`)
- **Type:** Stateful widget
- **Description:** Provides a form to add a new expense.
- **Features:** 
  - Uses `TextEditingController` for input fields.
  - Handles form submission.

### Chart (`lib/widgets/charts/chart.dart`)
- **Type:** Stateless widget
- **Description:** Displays a chart of expenses.
- **Dependencies:**
  - `ChartBar` (for each category of expenses)

---

## Classes

### Expense (`lib/models/expense.dart`)
- **Description:** Represents an expense.
- **Properties:**
  - `title`
  - `amount`
  - `date`
  - `category`

### ExpenseBucket (`lib/models/expense_bucket.dart`)
- **Description:** Represents a bucket of expenses for a specific category.
