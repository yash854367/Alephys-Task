# Expense Tracker

A simple Java console application for tracking your incomes and expenses. Easily add, view, save, and load your financial transactions, and get a clear monthly summary of your finances.

---

## Features

- **Add Transactions:**  
  Log income or expense transactions with category, amount, date, and optional description.

- **View Monthly Summary:**  
  See your total income, expenses, category breakdowns, and net savings for any month.

- **Save Data to File:**  
  Export all transactions to a CSV file for backup or sharing.

- **Load Data from File:**  
  Import transactions from a CSV file into the application.

---

## How to Use

1. **Compile the App**

    ```bash
    javac ExpenseTracker.java
    ```

2. **Run the App**

    ```bash
    java expense.ExpenseTracker
    ```

3. **Menu Options**

    ```
    1. Add Transaction
    2. View Monthly Summary
    3. Save Data to File
    4. Load Data from File
    5. Exit
    ```

    - **Add Transaction:**  
      Enter 'I' for income or 'E' for expense, specify category, amount, date (YYYY-MM-DD), and an optional description.

    - **View Monthly Summary:**  
      Enter a month (YYYY-MM) to see the breakdown and net savings.

    - **Save Data to File:**  
      Provide a filename (like `transactions.csv`) to export all current transactions.

    - **Load Data from File:**  
      Provide a CSV file to import transactions (existing data will be kept in addition).

    - **Exit:**  
      Close the application.

---

## CSV File Format

Each transaction is stored as a line in CSV with these fields:

```
Type,Category,Amount,Date,Description
```

- `Type`: `I` for Income, `E` for Expense
- `Category`: e.g., Salary, Food, Rent, Business, Travel, etc.
- `Amount`: Numeric value
- `Date`: In format `YYYY-MM-DD`
- `Description`: Optional text

**Example:**

```
I,Salary,50000,2025-05-01,Monthly salary
E,Food,800,2025-05-02,Lunch
E,Rent,12000,2025-05-03,May rent
I,Business,2500,2025-05-10,Freelance
E,Travel,1500,2025-05-11,Taxi
```

---

## Notes

- When saving to a file, make sure the file is **not open** in another program (like Excel).
- When loading from a file, ensure the format matches the example above.
- You can open the CSV file in Excel, Notepad, or any spreadsheet/text editor for review or manual editing.

---

## Requirements

- Java 8 or newer
