
# Rest API

## Accounts

| Method | Path                   | Description             |
|:-------|:-----------------------|:------------------------|
| POST   | `/accounts`            | Create Account       |
| PUT    | `/accounts/{accountID}` | Update Account       |
| DELETE | `/accounts/{accountID}` | Delete Account       |
| PUT    | `/accounts/{password}`  | Reset Password       |



## Categories
| Method | Path                   | Description             |
|:-------|:-----------------------|:------------------------|
| POST   | `/accounts/{accountID}/categories`          | Create Category       |
| PUT    | `/categories/{categoryID}`| Update Category       |
| DELETE | `/categories/{categoryID}` | Delete Category       |
| DELETE | `/categories` | Delete All Categories       |
| GET    | `/categories`  | List All Categories       |
| GET    | `/categories/{categoryID}`  | List a Specific Category       |

## Transactions
| Method | Path                   | Description             |
|:-------|:-----------------------|:------------------------|
| POST   | `/categories/{categoryID}/transactions/`          | Create Transaction       |
| PUT    | `/transactions/{transactionID}`| Update Transaction       |
| DELETE | `/transactions/{transactionID}` | Delete Transaction       |
| DELETE | `/transactions` | Delete All Transaction       |
| GET    | `/transactions`  | List All Transactions       |
| GET    | `/transactions/{transactionID}`  | List a Specific Transactions       |
