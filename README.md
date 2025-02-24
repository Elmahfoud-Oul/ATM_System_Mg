# ATM System (C Programming)

This repository contains a C program for a basic ATM system. The program simulates typical ATM functions, including checking balances, withdrawing money, depositing money, transferring money, and viewing transaction slips. The application is structured to interact with the user through a text-based interface (Console).

---

## Features:

1. **Welcome Screen**: 
   - Displays a welcoming message to the user.
   
2. **PIN Authentication**: 
   - The user must enter the correct 4-digit PIN (00000 in this case) to access the ATM system.

3. **Core ATM Services**:
   - **Check Balance**: 
     - The user can check the current balance.
   - **Withdraw Cash**: 
     - The user can withdraw money (subject to available balance).
   - **Deposit Cash**: 
     - The user can deposit money into their account.
   - **Transfer Money**: 
     - The user can transfer money to another account after PIN authentication.
   - **Mini Statement**: 
     - The user can view a mini statement of recent transactions (Withdrawals, Deposits, and Transfers).
     
4. **Transaction Slip**: 
   - The user can opt to generate and save a transaction slip, detailing the transaction history and current balance.

5. **Date & Time**: 
   - The program tracks and displays the current date and time for each transaction.

---

## File Operations:
- The transaction slip can be saved to a specific file on your computer. It is written to the file using the `fprintf` function.

---

## Code Explanation:

### 1. `welcome()`:
   - Displays the welcome message when the ATM system is started.

### 2. `withdraw()`:
   - Prompts the user to enter the amount they wish to withdraw.
   - Checks if the balance is sufficient for the withdrawal.
   - If sufficient, updates the balance and logs the transaction.

### 3. `transfer()`:
   - Prompts the user to enter the recipient account number and PIN.
   - Allows the user to transfer money after verifying the PIN.
   - If the balance is sufficient, updates the balance and logs the transaction.

### 4. `deposit()`:
   - Allows the user to deposit money into their account.
   - Updates the balance and logs the transaction.

### 5. `date_time()`:
   - Fetches the current date and time from the system and prints it in a specific format.

### 6. `slip()`:
   - Prints the transaction slip on the console, listing all recent transactions.
   - The slip contains the current balance and transaction details.

### 7. `printout()`:
   - Prompts the user if they want to save a transaction slip to their computer.
   - If the user agrees, the slip is saved to a file.

---

## Console View

The following image shows the console interface of the ATM system:

![ATM Console View](https://raw.githubusercontent.com/Elmahfoud-Oul/ATM_System_Mg/refs/heads/main/Console_View.png)

---

## How to Run:

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/Elmahfoud-Oul/ATM_System_Mg.git
