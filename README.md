# Simple Financial Transactions API using Node

This project implements a boilerplate financial transactions API, in which the user can GET and POST transactions, saving and loading them from their chosen database (currently in memory). Withdrawal transactions will respect the user's balance.

## Install

`yarn install` on the root folder

## How to use

- run `yarn dev:server` and access http://localhost:3333/transactions to get the list of transactions
- `POST` to the above path to create a new transaction, using the parameters as the following example:

```json
{
  "title": "Created a website",
  "value": 10000,
  "type": "income"
}
```

`type` can be either `income` or `outcome`

## Extending the project

Currently, you can only `GET` or `POST` new transactions, they can not be updated and removed, and it saves the data to memory. Making this useful would require you to add a real database and implement the full transactions CRUD.
