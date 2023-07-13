# Bank App

Write a bank application with python (preferably with `+3.10` version) that can accept incoming and outgoing money transactions.

## Requirements

* You can import a file of transactions into your bank application. Transaction at 
  minimum should consist of:
    * Date of the transaction
    * Description of transaction
    * Amount: positive amount is incoming transaction (money you receive) , negative is 
      outgoing transaction (money you spent on something)
* Imported data is computed to show balance of your account.
* Add an option to specify type of account for your bank app. It can be either Debit 
  (balance can't be negative) or Credit (balance can be negative up to specified amount)
* Should be possible to save imported data, so next time bank app is loaded, it will have 
  history of already imported data.
* When data is imported, it should print current balance of your account.
* You should be able to query your bank account to return balance at specific date or
  return transactions of specific period (e.g. we specify transactions date range and 
  we get all transactions for that range).
* There should be some basic tests that validate that app is working:
    * Import incoming and outgoing transactions. Get current balance of account.
    * Import transactions with different dates. Get balance of specific date (also can 
      write test when there are no transactions for wanted date).
    * Try to import transactions that would make a balance negative in Debit type of account.
    * Import transactions when it would make it negative balance in Credit type of Account (also when it would go over the credit limit as well).

### Bonus

Add multi currency support:

* Specify used currencies with their rates on specific dates (loaded by bank app).
* Transaction should now specify which currency it uses.
* Bank app uses one specific currency, where other currency rates are bases on that currency.
* When transactions are imported in bank app, amounts are converted to account currency.

### Extra Info

UI for bank APP does not matter, can even be simple prints.
App can work just like a simple program that accepts arguments and produces output and saves data somewhere.
