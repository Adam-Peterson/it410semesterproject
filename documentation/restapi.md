
# Rest API

## Accounts

| Method | Path                   | Description             |
|:-------|:-----------------------|:------------------------|
| POST   | `/accounts`            | Create Account       |
| PUT    | `/accounts/{accountID}` | Update Account       |
| PUT    | `/accounts/{accountID}` | Deactivate Account       |
| DELETE | `/accounts/{accountID}` | Delete Account       |
| PUT    | `/accounts/{password}`  | Reset Password       |

## Sessions
| Method | Path                   | Description             |
|:-------|:-----------------------|:------------------------|
| POST   | `/sessions`            | Create Session       |
| PUT   | `/sessions/{sessionID}` | Renew Session       |
| DELETE    | `/sessions/{sessionID}` | Delete Session       |


## Budget Categories
| Method | Path                   | Description             |
|:-------|:-----------------------|:------------------------|
| POST   | `/accounts/{accountID}/categories/{categoryTitle}/{categoryBudgetGoal}`          | Create Category       |
| PUT    | `/categories/{categoryID}/{categoryTitle}`| Update Category Title      |
| PUT    | `/categories/{categoryID}/{categoryBudgetGoal}`| Update Category Budget Goal      |
| DELETE | `/categories/{categoryID}` | Delete Category       |
| DELETE | `/categories` | Delete All Categories       |
| GET    | `/categories`  | List All Categories       |
| GET    | `/categories/{categoryID}`  | List a Specific Category       |

## Transactions
| Method | Path                   | Description             |
|:-------|:-----------------------|:------------------------|
| POST   | `/categories/{categoryID}/transactions/{transactionTitle}/{transactionAmount}`          | Create Transaction       |
| PUT    | `/transactions/{transactionID}`| Update Transaction       |
| DELETE | `/transactions/{transactionID}` | Delete Transaction       |
| DELETE | `/transactions` | Delete All Transactions       |
| GET    | `/transactions`  | List All Transactions       |
| GET    | `/transactions/{transactionID}`  | List a Specific Transactions       |
