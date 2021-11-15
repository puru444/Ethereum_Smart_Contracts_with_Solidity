# ETHEREUM SOLIDITY SMART CONTRACT

**For Hosting: Joint Savings Accounts**
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**BACKGROUND:** As Ethereum's Smart Contract Developer, I need to create a Solidity Smart Contract that accepts two user addresses. These addresses will be able to control a Joint Savings Account, this Smart Contract will use Ether Mgmt. Functions to implement a Financial Institution’s requirements for providing the features of the Joint Savings Account. These features will consist of the ability to Deposit & Withdraw funds from the Account.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**CONTENT**
- Project Description
- Technologies
- Ethereum Smart Contract - Features & Transactions
- Contributor
- License
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**PROJECT DESCRIPTION**

Following are the high-level details of this project:

Version Used: Pragma Solidity 0.5.0

1. Define a new contract named **`JointSavings`**
2. Inside the new contract 'JointSavings', following variables are defined:
    - Two variables of type `address payable` named `accountOne` and `accountTwo`
    - A variable of type `address public` named `lastToWithdraw`
    - Two variables of type `uint public` named `lastWithdrawAmount` and `contractBalance`.
3. Define a function named **'withdraw'** that will accept two arguments.
    - `uint` variable named `amount`
    - `payable address` named `recipient`
4. Define a `public payable` function named **`deposit`**
5. Define a `public` function named `setAccounts` that receive two `address payable` arguments named `account1` and `account2`.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**TECHNOLOGIES**

- Remix IDE - (https://remix.ethereum.org/#optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.7+commit.e28d00a7.js)
- Code Compiler Version: 0.5.0
- Contract Deployment Environment: Javascript VM
- Language: Solidity
- Crypto Currency: Ether
- Keys Generator: Ganache
- Wallet: Metamask

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**ETHEREUM SMART CONTRACT (Environment: Remix IDE)**
----------------------------------------------------

**A. Following basic functionalities are defined in Smart Contract:**

**1. Defined: Contract Name:** 

Under Version Pragma Solidity 0.5.0, the Contract defined as "JointSavings" with few variables:

![Code_1](https://user-images.githubusercontent.com/86034323/141752416-4c58d85b-5a13-4781-812f-23d98d0aefc6.png)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**2. Defined Function: Withdraw:**

- In order to implement the capability to Withdraw, few "require" functions are defined to manage the "error handling" capability with warning messages with public view privileges. 
- Defined other logics: lastwithdraw amount with balances.

![Code_2](https://user-images.githubusercontent.com/86034323/141753119-4fa0a974-7f59-497e-873f-bb8c6a34468b.png)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**3. Defined Function: Deposit:**

- In order to implement the capability to Deposit, the function "deposit" is defined with public view privileges.
- Defined contractBalanace to get the current balance amount of Contract. 

![Code_3](https://user-images.githubusercontent.com/86034323/141754409-364454cc-10a7-4cf2-b6ca-1b34e63ae228.png)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**4. Defined Function: setAccounts:**

- In order to define the basic 2 Joint Accounts, "setAccounts" function has been used with public view privileges.
- Where, the values are defined for Joint Accounts (accountOne & accountTwo).

![Code_4](https://user-images.githubusercontent.com/86034323/141755766-d6aead44-e7d8-41c0-bf41-bdaedc769d7b.png)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**5. Defined Function: Default Fallback Function:**

- In order to store the Ether sent from outside the deposit function, this fallback function needs to be defined:

![Code_5](https://user-images.githubusercontent.com/86034323/141757257-968fd96f-c3be-41be-b238-3a4154cc2609.png)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**B. Following features of Smart Contract are highlighted below:**

**1. COMPILE: Smart Contract:**

Once the Smart Contract's basic functionalities are defined, then the next step is: To Compile the Smart Contract: 

![compiled](https://user-images.githubusercontent.com/86034323/141758389-7ccdb1ad-594f-4f6a-b7cb-f44c237aef3b.png)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**2. DEPLOY: Smart Contract:**

Next step is: To deploy the Smart Contract in JavaScript VM Environment:

![Deploy](https://user-images.githubusercontent.com/86034323/141759623-8d5e0df2-5780-4fdb-8ef8-f77089ba04a4.png)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**3. DEPLOYMENT VERIFIED: Smart Contract:**

Once the contract is deployed, it can be verified with complete details like Gas Fees, TRX Hash, TRX Cost, Execution Cost etc. 

![Deployed_Contract](https://user-images.githubusercontent.com/86034323/141760514-12c0084e-12d9-4822-a523-04f518801753.png)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**C. Following are the transactions occured after deploying the Smart Contract:**

**1. Set Accounts:**

- Set up two accounts using the "setAccounts" function. Following two accounts are setup as account1 and account2 for the Deployed Contract:

1. account1 address: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb
2. account2 address: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0

- After mentioning the accounts' hash keys, we click on “transact button” to set up these two accounts.

![setAccount_Function](https://user-images.githubusercontent.com/86034323/141761499-71e16a6c-577d-4640-86f9-429749ae6afa.png)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**D. Transactions: 3 Deposits & 2 Withdrawals:**

**1. DEPOSIT 1 ETHER IN WEI:** 

- TRX_1: Deposit of 1 Ether on scale of Wei i.e. 1000000000000000000 (1 Quintillion Wei) in Deployed Contract:

![deposit_1ether](https://user-images.githubusercontent.com/86034323/141764823-6d58a39e-7c27-43c2-aa84-a01449ec2dc8.png)

- TRX_1 Details:

![deposit_1ether_trx](https://user-images.githubusercontent.com/86034323/141765505-ebf7fdcf-a397-4eb4-afd1-699ce6765d08.png)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**2. DEPOSIT 10 ETHERS IN WEI:** 

- TRX_2: Deposit of 10 Ether on scale of Wei i.e. 10000000000000000000 (10 Quintillion Wei) in Deployed Contract:

![deposit_10ether](https://user-images.githubusercontent.com/86034323/141766059-381e608a-1e08-4ac8-a7b0-7b901744fc96.png)

- TRX_2 Details:

![deposit_10ether_trx](https://user-images.githubusercontent.com/86034323/141766379-881f5b94-04cd-4a2e-b59f-27ea34dcdbee.png)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**3. DEPOSIT 5 ETHERS:**

- TRX_3: Deposit of 5 Ether in Deployed Contract:

![deposit_5ether](https://user-images.githubusercontent.com/86034323/141766721-db64e629-c088-485f-9c7c-b8ddf09baaf9.png)

- TRX_3 Details:

![deposit_5ether_trx](https://user-images.githubusercontent.com/86034323/141766934-b589f198-7eff-4cb6-a337-42e1629438d9.png)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**4. WITHDRAWAL 5 ETHERS IN WEI:**

- TRX_4: Withdrawal of 5 Ether on scale of Wei i.e. 5000000000000000000 (5 Quintillion Wei) for account1 (0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb) with Contract Balance of 16 Ethers:

![withdrawal_5ether](https://user-images.githubusercontent.com/86034323/141767601-5d4f2d7b-ad80-43fa-a2b6-85c4f85c71df.png)

- Contract Balance has been reduced by 5 Quintillion Wei, updated amount is: 11 Quintillion Wei

![withdrawal_5ether_contractbalance](https://user-images.githubusercontent.com/86034323/141768221-c3d7e275-36ac-4d06-a175-ba8524e84577.png)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**5. WITHDRAWAL 10 ETHERS IN WEI:**

- TRX_5: Withdrawal of 10 Ethers on scale of Wei i.e. 10000000000000000000 (10 Quintillion Wei) for account2 (0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0) with Contract Balance of 11 Ethers:

![withdrawal_10ether](https://user-images.githubusercontent.com/86034323/141768789-6c1b7650-c884-496c-83b3-e3e998b78470.png)

- Contract Balance has been reduced by 10 Quintillion Wei, updated amount is: 1 Quintillion Wei (1 Ether)

![withdrawal_10ether_contractbalance](https://user-images.githubusercontent.com/86034323/141769031-7a81929b-9886-4079-9436-16f4e0215d2c.png)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**CONTRIBUTOR**

- PRATEEK SHARMA

www.linkedin.com/in/prateek-sharma-21a081180

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**LICENSE**

GNU General Public License v3.0
