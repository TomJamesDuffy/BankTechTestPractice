# Week 10 Makers Academy
This is the first practice tech test set during the tenth week of Makers Academy.

## Specification

### Model

![Program Structure](https://image.ibb.co/cp5xtc/Bank_Tech_Test_Diagram.jpg)

### Setup

1.) Run bundle install  
2.) Run RSpec to confirm tests are working

### Approach

The first step I took was to try and frame the problem as a diagram (see above). I then tried to tackle the aspects of the program that were most important from the users point of view. That is, having the ability to withdraw and deposit from their bank. Followed by the ability to view the balance. These segments were test driven.

### How to use

The two main classes are the bank class and the statement class.

The BankAccount class enables you to `withdraw`, `deposit` and see your `balance`.    
You can also call your transaction history in the form of an array using `bank.transaction_history`  
The statement class enables you to print a given transaction history.   

`Statement.print(bank.transaction_history)`

### Requirements

* You should be able to interact with your code via a REPL like IRB or the JavaScript console.  (You don't need to implement a command line interface that takes input from STDIN.)
* Deposits, withdrawal.
* Account statement (date, amount, balance) printing.
* Data can be kept in memory (it doesn't need to be stored to a database or anything).

### Acceptance criteria

**Given** a client makes a deposit of 1000 on 10-01-2012  
**And** a deposit of 2000 on 13-01-2012  
**And** a withdrawal of 500 on 14-01-2012  
**When** she prints her bank statement  
**Then** she would see

```
date || credit || debit || balance
14/01/2012 || || 500.00 || 2500.00
13/01/2012 || 2000.00 || || 3000.00
10/01/2012 || 1000.00 || || 1000.00
```
