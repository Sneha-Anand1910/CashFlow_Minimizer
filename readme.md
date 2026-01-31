# CashFlow Minimizer (C | DSA Project)

## Project Overview
CashFlow Minimizer is a C-based program that minimizes the number of transactions required to settle debts among a group of people.

The project models transactions as a graph using an adjacency matrix and applies a greedy cashflow minimization algorithm to compute simplified settlements. It also includes strict input validation and an optional fixed-budget constraint.

-------------------------------------------------------------------------------------------------------------------

## Problem Statement
In group expense scenarios (trips, events, shared spending), multiple transactions between people make settlement complex.

This project simplifies the settlement process by:
- Calculating net balances for each person
- Reducing multiple transactions into the minimum required transfers
- Ensuring correctness and fairness

-------------------------------------------------------------------------------------------------------------------

## Key Features
- Unique name and Gmail ID validation
- Case-insensitive input handling
- Transaction graph representation using adjacency matrix and adjacency list
- Net balance computation for each participant
- Greedy algorithm for minimizing cashflow transactions
- Floating-point precision handling
- Fixed-budget validation (total spending = 1000 units)

-------------------------------------------------------------------------------------------------------------------

## Validation Rules
- Names must be unique (case-insensitive)
- Only Gmail IDs ending with '@gmail.com' are accepted
- Sender and receiver cannot be the same person
- Transaction amount must be positive
- Total spending must equal exactly 1000 units
- No single person can spend the entire budget alone

-------------------------------------------------------------------------------------------------------------------

## Algorithm Used
1. Store transactions in an adjacency matrix
2. Compute net balance for each person: - Incoming money − Outgoing money
3. Identify the maximum creditor and maximum debtor
4. Settle the minimum possible amount between them
5. Repeat until all balances become zero

This greedy approach minimizes the total number of transactions.

-------------------------------------------------------------------------------------------------------------------

## Data Structures Used
- Adjacency Matrix
- Adjacency List
- Arrays
- Structures

-------------------------------------------------------------------------------------------------------------------

## Project Structure
CashFlow_Minimizer/
├── main.c # Program entry point
├── cashflow.c # Core cashflow minimization logic
├── cashflow.h # Function declarations and constants
└── README.md # Project documentation