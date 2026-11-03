# 🏦 Banking Management System (DBMS Project)

A comprehensive **Advanced Database Management System (ADBMS)** project implemented in **MySQL Workbench 8.0**. This system handles core banking operations including customer registration, account management, secure fund transfers, and transaction history tracking using procedural SQL features.

## 🚀 Features
* **Normalized Schema:** Manages `CUSTOMERS`, `ACCOUNTS`, and `TRANSACTIONS` with proper foreign key constraints.
* **Stored Procedures:** Automated procedures for:
  * Customer Registration (`ADD_CUSTOMER`)
  * Bank Account Generation with custom account numbering (`OPEN_ACCOUNT`)
  * Safe Money Deposits & Withdrawals with transaction rollbacks (`DEPOSIT_MONEY`, `WITHDRAW_MONEY`)
  * Inter-account Fund Transfers (`TRANSFER_MONEY`)
  * Transaction History Reporting (`SHOW_HISTORY`)
* **Triggers & Functions:** 
  * Prevents invalid or negative transactions using triggers (`CHECK_TRANSACTION`).
  * Instant balance checks via SQL functions (`CHECK_BALANCE`).
* **Cursors:** Utilizes SQL cursors to fetch and loop through detailed transaction histories.

## 🛠️ Tech Stack
* **Database:** MySQL / MySQL Workbench 8.0
* **Concepts Used:** DDL, DML, Transactions (`ACID` compliance with `START TRANSACTION`, `COMMIT`, `ROLLBACK`), Stored Procedures, Functions, Triggers, and Cursors.

## ⚙️ How to Run
1. Open **MySQL Workbench**.
2. Copy and run the code from `database_script.sql` or import the script directly.
3. The script will automatically create the `BANKING_DB` database, tables, routines, and execute test cases.