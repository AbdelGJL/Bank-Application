# Bank-Application
Below are the function names and their purposes in the provided code:

sys module: Imports the sys module, which provides access to variables and functions that interact with the interpreter.

os module: Imports the os module, which allows the use of operating system-dependent functionality, such as file system interaction.

datetime module: Imports the datetime module, which provides classes for working with dates and times.

Employee class: Defines a class called "Employee" that represents a bank employee.

init(self, pin): Initializes an Employee object with a provided PIN.

login_menu(self): Displays the login menu for employees, allowing them to choose between employee, customer, or program exit. Calls the corresponding login function based on the choice.

login_as_employee(self): Prompts the employee to enter their PIN. If the entered PIN matches the employee's PIN, it displays the employee menu; otherwise, it prompts for the PIN again.

login_as_customer(self): Calls the login_as_customer function of the bank object.

employee_menu(self): Displays menu options available to the employee, prompts for a choice, and calls the corresponding function based on the choice.

Customer class: Defines a class called "Customer" that represents a bank customer.

init(self, first_name, last_name, email, pin): Initializes a Customer object with the provided first name, last name, email, and PIN. Sets initial values for the account number, savings balance, and current balance.

customer_menu(self, bank): Displays menu options available to the customer, prompts for a choice, and calls the corresponding function based on the choice.

perform_transaction_menu(self, bank): Displays account type options for performing a transaction, prompts for a choice, and calls the corresponding function based on the choice.

Bank class: Defines a class called "Bank" that represents the bank itself.

init(self): Initializes a Bank object. Sets the employee's PIN, initializes empty dictionaries for customers and transactions, and creates the necessary directories and files.

load_customer_accounts(self): Loads existing customer accounts from a file into the customers dictionary.

update_customer_file(self): Updates the customer file with the current customer data.

create_transaction_file(self, account): Creates a transaction file for the specified account.

save_transaction(self, account_number, account_type, transaction_type, amount, new_balance): Saves a transaction record in the corresponding transaction file.

login_menu(self): Calls the login_menu function of an Employee object to display the initial login menu.

login_as_customer(self): Prompts the customer for their details, validates them, logs the customer in if the details are valid, and displays the customer menu.

create_customer_account(self): Prompts an employee to enter customer details, generates an account number and PIN, creates a new customer account, and updates the customer file.

delete_customer_account(self): Prompts an employee to enter a customer's account number, checks if the account exists, and deletes the customer account if it has a zero balance.

create_transaction(self, account_number, account_type): Prompts an employee to enter transaction details, performs the transaction if the account exists and has sufficient balance, and updates the customer account and transaction records.

display_customer_account(self, account_number): Displays the customer account details for the specified account number.

display_transaction_history(self, account_number, account_type): Displays the transaction history for the specified account number and account type.

display_all_accounts(self): Displays the account details for all customers.

bank = Bank(): Creates an instance of the Bank class, representing the bank object.

bank.login_menu(): Calls the login_menu function of the bank object to start the banking system by displaying the initial login menu.

The customers.txt contains a list of customers of the bank.

The transactions folder contains the files of savings and currents balances of all accounts of the bank.

In summary, the provided code implements a basic banking system where employees can log in and perform various operations such as creating customer accounts, deleting customer accounts, and conducting transactions. Customers can also log in and perform transactions on their accounts. The system maintains customer account details and transaction history using files.
