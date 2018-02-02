# currency-data
## the task
You need to fetch current currency rates for EUR to USD and EUR to CHF from the currencylayer API and store them into a MySQL database table.

https://currencylayer.com (you'll have to sign up for a free account)

### goals
* Define the table structure
* Provide a CLI PHP script which when executed fetches the data and stores it into the table

### constraints
* Use the oceanapplications/currencylayer-php-client SDK

### hints 
* You can use whatever frameworks & libraries you want (except the aforementioned API SDK which you are required to use)
* You can use any PHP7.1 features you want
* You can use any MySQL 5.7 features you want

## discussion

| Task Component | Possible Questions |
|------|--------------------|
|Add currencylayer API SDK via composer| What is semver?
||Should composer.lock be committed or not?|
|Use the SDK to fetch current currency rates for EUR → USD and EUR → CHF||
|Define a MySQL table to store the rates|How do you set the PK and why?|
||Currencies as string, Enum or create an String → Id mapping? |
||When using Enum, what are the advantages and disadvantages of each type?|
||What MySQL data type do you use for money? Float or Decimal? Why?|
|Store rates into this table|mysqli or PDO|
||What are the advantages of prepared statements?|
||SQL injection: What is the conceptual difference between using prepared statements and escaping the data using the quote/escape function|
|Bonus: Add a simple unit test|If not already happened: What would you abstract to make your code unit testable (dependency injection) and how would you do it?|




