# ATM Simulator System

This is a desktop-based ATM simulator developed in **Java** using **Swing** for the Graphical User Interface (GUI) and **JDBC** for database connectivity. It provides a user-friendly interface for simulating standard ATM operations, including balance inquiry, deposits, and withdrawals.


---

## ✨ Key Features

- **User Authentication**: Secure login using a PIN.
- **Account Management**: Users can check their balance, deposit funds, and withdraw cash.
- **Transaction History**: A log of all transactions is maintained for each user.
- **File-Based Storage**: Account data and transaction history are saved to a file, so they are not lost when the program exits.
- **GUI Interface**: A desktop application built with Java Swing for a user-friendly experience.
- **Database Integration**: Uses JDBC to connect to a relational database (like MySQL or PostgreSQL) to manage user accounts and transactions.
- **Secure Authentication**: Users log in with a unique account number and PIN.
- **Transaction Processing**: Supports real-time deposits and withdrawals with validation checks.
- **Transaction History**: Keeps a record of all transactions for each user.

---


## 🚀 How to Run

### Prerequisites

- **Java Development Kit (JDK) 8 or later**
- An **SQL database** (e.g., MySQL)
- The **JDBC driver** for your specific database (e.g., `mysql-connector-java.jar`).

### Instructions

1.  **Set up the Database**:
    - Create a database and tables for `accounts` and `transactions`.
    - Example SQL for an `accounts` table:
      ```sql
      CREATE TABLE accounts (
          account_number VARCHAR(20) PRIMARY KEY,
          pin_number VARCHAR(4) NOT NULL,
          balance DECIMAL(10, 2) NOT NULL
      );
      ```

2.  **Configure the Project**:
    - Add the **JDBC driver JAR file** to your project's build path.
    - Update the **database connection details** (URL, username, password) in your database connection class.

3.  **Run the Application**:
    - Compile and run the main class from your IDE (e.g., `Main.java` or `ATMApp.java`).
---

## 📖 Usage

Follow the prompts in the command line to use the ATM.

1.  Enter your **PIN** to log in.
2.  Select an option from the menu:
    - `1` to **Check Balance**
    - `2` to **Deposit**
    - `3` to **Withdraw**
    - `4` to **View Transaction History**
    - `5` to **Exit**

---

## 🤝 Contributing

Contributions are welcome! If you find a bug or have an idea for a new feature, feel free to open an issue or submit a pull request.

1.  Fork the repository.
2.  Create your feature branch (`git checkout -b feature/NewFeature`).
3.  Commit your changes (`git commit -m 'Add a new feature'`).
4.  Push to the branch (`git push origin feature/NewFeature`).
5.  Open a **Pull Request**.

---
