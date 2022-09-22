# Bank tech test

## Specification

### Requirements

You should be able to interact with your code via a REPL like IRB or Node. (You don't need to implement a command line interface that takes input from STDIN.)
Deposits, withdrawal.
Account statement (date, amount, balance) printing.
Data can be kept in memory (it doesn't need to be stored to a database or anything).

### Acceptance criteria

Given a client makes a deposit of 1000 on 10-01-2023
And a deposit of 2000 on 13-01-2023
And a withdrawal of 500 on 14-01-2023
When she prints her bank statement
Then she would see

date || credit || debit || balance
14/01/2023 || || 500.00 || 2500.00
13/01/2023 || 2000.00 || || 3000.00
10/01/2023 || 1000.00 || || 1000.00

### User stories

```
As a customer
So I can make financial transactions
I would like to open a bank account
```

```
As a customer
So I can make purchases
I would like to withdraw money from the bank 
```

```
As a customer
So I can grow my savings
I would like to deposit money into the bank
```

```
As a customer
So I can keep track of my financial transactions and account balance
I would like to be able to print out a statement
```

### Quick start

* clone this repository
*  `bundle install` inside the terminal


## Dependencies

This projects uses `rspec` for testing.

Gemfile
```ruby
# frozen_string_literal: true

source "https://rubygems.org"

# gem "rails"

gem "rspec", "~> 3.11"

```