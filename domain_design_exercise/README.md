# Domain Design 

## Understanding Scenario (Bank Application)

- ***Customer*** can open an account.
- Two types of accounts:
  - ***Saving Account***: 
  - ***Current Account***: 

- An ***account*** can be opened with
    - **Single**
    - **Joint**:    

- A ***customer*** can have an unlimited number of ***accounts***.


- An ***account*** has a reference to its associated **account holder** (***customer record***).

- ***Customer*** can apply for ATM card (oprional)

- A customer record can
remain active even if the customer has terminated the ATM card service and returned the card to
the bank.

- An **account** is associated with a **branch**.

- A ***branch*** is associated with an unlimited number of
accounts.


## Idenifying Nouns 

- Customer
- Account
- Branch
- ATM Card
- Employment Details
- Savings Account
- Current Account

## Domain Model Classification Table

| Concept | Identity? | Lifecycle? | Business Logic? | Mutable? | Category |
|---------|-----------|------------|----------------|----------|----------|
| Customer | ✅ | ✅ | ✅ | ✅ | Entity |
| Account | ✅ | ✅ | ✅ | ✅ | Entity |
| ATM Card | ✅ | ✅ | ✅ | ✅ | Entity |
| Branch | ✅ | ✅ | Maybe | ✅ | Entity |
| Employment Details | ❌ | ❌ | ❌ | ❌ | Value Object |
| Address | ❌ | ❌ | ❌ | ❌ | Value Object |