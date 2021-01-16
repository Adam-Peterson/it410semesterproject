# Define Events
<ul>
  <li>account created</li>
  <li>account updated</li>
  <li>account deactivated</li>
  <li>account deleted</li>
  <li>account password reset</li>
  <li>session created</li>
  <li>session deleted</li>
  <li>budget category created</li>
  <li>budget category updated</li>
  <li>budget category deleted</li>
  <li>transaction item created</li>
  <li>transaction item updated</li>
  <li>transaction item deleted</li>
</ul>

# Define Commands
<ul>
  <li>Create an account</li>
  <li>Delete an account</li>
  <li>Update account password</li>
  <li>Validate password</li>
  <li>Create budget category</li>
  <li>Set budget category dollar goal</li>
  <li>Rename budget category</li>
  <li>Update budget category dollar goal</li>
  <li>Create transaction</li>
  <li>Assign transaction to cateory</li>
  <li>Reassign transaction to different cateogry</li>
  <li>Delete transaction</li>
  <li>Delete category
    <ul>
      <li>Deleting a category will trigger delete transaction for all transactions in the category</li>
    </ul>
   </li>
  <li>Check balance remaining</li>
  <li>View Transactions</li>
  <li>View Category</li>
</ul>


# Define Entities
<ul>
<table><thead><tr><th>Property</th><th>Type</th><th>Description</th></tr></thead><tbody><tr><td>id</td><td>UUID</td><td>Automatically generated, immutable, unique identifier.</td></tr><tr><td>username</td><td>text</td><td>The user's chosen display name.</td></tr><tr><td>password</td><td>encrypted text</td><td>The user's password.</td></tr></tbody></table>  <li>Category</li>
  <li>Transaction</li>
</ul>

# Define Value Objects
<ul>
  <li>File (Reciept image upload)
      <ul>
      <li>This is a potential feature that may or may not exist in the final product</li>
    </ul>
  </li>
</ul>


