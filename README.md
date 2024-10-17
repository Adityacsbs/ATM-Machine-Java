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

   Database Configuration:

2. Set up a MySQL database named atm_machine.
   Run the following SQL commands to create the required tables:

     CREATE DATABASE atm_machine;

USE atm_machine;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    password VARCHAR(50) NOT NULL,
    balance DECIMAL(10, 2) DEFAULT 0.00
);

CREATE TABLE transactions (
    id INT AUTO_INCREMENT PRIMARY KEY,
    user_id INT,
    type ENUM('deposit', 'withdrawal', 'transfer'),
    amount DECIMAL(10, 2),
    date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
3.  Configure Database Connection:

   Open Conn.java.
   Update the database connection details with your local setup:

   Connection con = DriverManager.getConnection("jdbc:mysql://localhost:3306/atm_machine", "root", "your_password");

4.  Run the Project:

   Open the project in your IDE (NetBeans or any other Java IDE).
   Compile and run the Login.java (or ATM.java) class.
   Use the console interface to simulate ATM transactions (create an account, login, and perform transactions).  
   


