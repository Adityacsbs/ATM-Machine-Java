# ATM Machine Project (Java)

## Overview
This project simulates an **ATM Machine** system developed in **Java**. It provides core functionalities of an ATM system including account creation, balance inquiry, withdrawals, deposits, mini-statement viewing, and fund transfers.

The project utilizes **JDBC** to connect to a **MySQL** database for storing user details and transactions.

## Features
- **Account Creation**: Allows users to create a new account with a unique ID.
- **Balance Inquiry**: Allows users to view their account balance.
- **Deposit**: Enables users to deposit money into their accounts.
- **Withdrawal**: Allows users to withdraw funds from their accounts.
- **Mini Statement**: Provides a summary of recent transactions.
- **Fund Transfer**: Allows users to transfer money from one account to another.
- **Account Management**: Includes signup, login, and account deletion functionalities.

## Technologies Used
- **Java**: Core programming language used for the backend logic.
- **JDBC**: Java Database Connectivity for interacting with the database.
- **MySQL**: Database used to store account details and transactions.
- **NetBeans**: IDE used for developing the project (or any other Java IDE).
- **Git**: Version control to track changes and collaborate on the project.

## Project Structure
### Core Classes:
- **Conn.java**: Establishes the connection to the MySQL database.
- **BalanceEquiry.java**: Displays the balance of the user.
- **Deposit.java**: Manages the deposit transactions.
- **Withdrawl.java**: Handles the withdrawal process.
- **Transactions.java**: Manages fund transfers and records transactions.
- **Login.java**: Handles user authentication and login.
- **Signup.java**: Manages the signup process for new accounts.
- **MiniStatement.java**: Provides recent transaction details to the user.

## Setup Instructions

### Prerequisites:
1. **Java JDK** (Version 8 or higher) installed on your machine.
2. **MySQL** database setup.
3. **NetBeans IDE** (or any IDE of your choice) to run the project.
4. **Git** installed for version control and collaboration.

### Steps to Run the Project:
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Adityacsbs/ATM-Machine-Java.git
