# Define Events

<ul>
  
  ## Account Events
  <li>account created</li>
  <li>account updated</li>
  <li>account deactivated</li>
  <li>account deleted</li>
  <li>account password reset</li>
  
  ## Session Events
  <li>session created</li>
  <li>session deleted</li>
  
  ## Budget Events
  <li>budget category created</li>
  <li>budget category updated</li>
  <li>budget category deleted</li>
  
  ## Transaction Events
  <li>transaction item created</li>
  <li>transaction item updated</li>
  <li>transaction item deleted</li>
</ul>

# Define Commands

<ul>
  
   ## Account Commands
  <li>Create an account</li>
  <li>Delete an account</li>
  <li>Update account password</li>
  <li>Validate password</li>
  
  ## Category Commands
  <li>Create budget category</li>
  <li>Set budget category dollar goal</li>
  <li>Rename budget category</li>
  <li>Update budget category dollar goal</li>
  <li>Delete category
    <ul>
      <li>Deleting a category will trigger delete transaction for all transactions in the category</li>
    </ul>
  </li>
  <li>View Category</li>

  
  ## Transaction Commands
  <li>Create transaction</li>
  <li>Assign transaction to cateory</li>
  <li>Reassign transaction to different cateogry</li>
  <li>Delete transaction</li>
    <li>View Transactions</li>
    
  ## Miscellaneous Commands

  <li>Check balance remaining</li>
</ul>


# Define Entities

## User Account
<table>
  <thead>
    <tr>
      <th>Property</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>UUID</td>
      <td>Automatically generated, immutable, unique identifier.</td>
    </tr>
    <tr>
      <td>username</td>
      <td>text</td>
      <td>User's chosen display name.</td>
    </tr>
    <tr>
      <td>password</td>
      <td>encrypted text</td>
      <td>The user's password, stored in a hashed format.</td>
    </tr>
  </tbody>
  </table>
  
  ## Category
  <table>
  <thead>
    <tr>
      <th>Property</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>UUID</td>
      <td>Automatically generated, immutable, unique identifier.</td>
    </tr>
    <tr>
      <td>account id</td>
      <td>UUID</td>
      <td>Account ID that category belongs to</td>
    </tr>
    <tr>
      <td>name</td>
      <td>text</td>
      <td>Name of the category (ex. Groceries)</td>
    </tr>
    <tr>
      <td>amount</td>
      <td>decimal</td>
      <td>Goal for money to be spent in this category per month</td>
    </tr>
  </tbody>
  </table>
  
  ## Transaction
  <table>
  <thead>
    <tr>
      <th>Property</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>UUID</td>
      <td>Automatically generated, immutable, unique identifier.</td>
    </tr>
    <tr>
      <td>task id</td>
      <td>UUID</td>
      <td>Task ID that this belongs to</td>
    </tr>
    <tr>
      <td>name</td>
      <td>text</td>
      <td>Name of the transaction</td>
    </tr>
    <tr>
      <td>Date</td>
      <td>Date</td>
      <td>Date of the transaction</td>
    </tr>
    <tr>
      <td>amount</td>
      <td>decimal</td>
      <td>Dollar amount of the transaction</td>
    </tr>
  </tbody>
  </table>

# Define Value Objects
<ul>
  <li>File (Reciept image upload)
      <ul>
      <li>This is a potential feature that may or may not exist in the final product</li>
    </ul>
  </li>
</ul>


