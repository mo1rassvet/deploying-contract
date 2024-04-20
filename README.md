# deploying-contract
Deploying contract on any chain via Atlas
for ex. **Function that allows for the transfer of tokens between two addresses**
This function takes three parameters:
- `_from`: The address of the token sender
- `_to`: The address of the token recipient
- `_amount`: The number of tokens to transfer
The function includes several `require` statements to ensure that:
1. The sender and recipient addresses are valid (not the zero address)
2. The transfer amount is greater than zero
3. The sender has sufficient balance to make the transfer
If all the requirements are met, the function updates the token balances of the sender and recipient addresses accordingly. It subtracts the `_amount` from the sender's balance and adds it to the recipient's balance.
Finally, the function emits a `Transfer` event to log the token transfer. The `Transfer` event should be defined in your contract with the appropriate parameters.
Note: Make sure to replace `balanceOf` with the actual mapping or variable name you use to store token balances in your contract.
