# Bank Management System

## Description
This is a simple console-based **Bank Management System** written in C++. It allows users to manage accounts, including creating new accounts, depositing and withdrawing money, modifying accounts, and deleting them. The data is stored in a binary file and operations are performed using file handling techniques.

## Features
- **Create a New Account**: Allows the user to create a new account by providing details such as account number, account holder's name, account type (C/S), and initial deposit.
- **Deposit Amount**: Deposits an amount to an existing account.
- **Withdraw Amount**: Withdraws an amount from an existing account, ensuring that the balance doesn't go negative.
- **Balance Enquiry**: Displays the details of a particular account based on the account number.
- **Display All Accounts**: Displays a list of all account holders with their account details.
- **Close an Account**: Deletes an account by removing it from the file.
- **Modify Account**: Allows the user to update the details of an existing account.

## How It Works
The program uses C++ classes to manage the account details and file handling to store account information in a binary file (`account.dat`). Here's a brief explanation of how each feature works:
- When an account is created, it's written to the binary file.
- For deposit, withdrawal, and modifications, the program reads from the file, modifies the data in memory, and then writes the updated data back to the file.
- Each account is stored with an account number, name, account type (C for Current, S for Savings), and balance.
  
## Class and Methods

### `account` Class
- `create_account()`: Gathers input for account number, name, account type, and initial deposit to create a new account.
- `show_account()`: Displays the details of a specific account.
- `modify()`: Allows the modification of account holder's name, account type, and balance.
- `dep(int)`: Adds the specified amount to the account balance.
- `draw(int)`: Deducts the specified amount from the account balance (if there are sufficient funds).
- `report()`: Displays a summarized account report.
- `retacno()`: Returns the account number.
- `retdeposit()`: Returns the current balance of the account.
- `rettype()`: Returns the type of account.

### Main Functions
- `write_account()`: Creates a new account and writes it to the binary file.
- `display_sp(int)`: Displays the details of a specific account.
- `modify_account(int)`: Allows the modification of an existing account.
- `delete_account(int)`: Deletes an account by removing it from the binary file.
- `display_all()`: Displays all account holders' details.
- `deposit_withdraw(int, int)`: Handles deposits and withdrawals by modifying the account balance.

## Setup and Compilation

### Requirements
- A C++ compiler (like GCC or any IDE that supports C++ programming).
  
### Compilation Steps
1. Copy the code into a file named `bank_management_system.cpp`.
2. Open the terminal and navigate to the folder where the file is located.
3. Compile the program using the following command:
   ```bash
   g++ -o bank_management_system bank_management_system.cpp
4. Run the compiled program
   ```bash
   ./bank_management_system
## Usage
1. After running the program, you will be presented with a menu.
2. Select the option you want to perform by entering the corresponding number.
3. Follow the instructions to complete operations like creating a new account, depositing/withdrawing money, and more.
