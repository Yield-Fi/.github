# .github
Platform Overview

Joinn is a Real World Asset (RWA) aggregation and tokenization platform designed to unify a fragmented market into a single, accessible hub. Through simple social logins, users can seamlessly create a non-custodial Joinn Smart Account and begin buying or selling on-chain RWAs from multiple issuers in one place. Users retain full ownership and control of their accounts and assets at all times, while our sponsored gas architecture enables gasless transactions—removing any need for blockchain expertise. Joinn is an on-chain RWA company committed to delivering seamless, global access to real-world asset investing for anyone with an internet connection. 

<img width="1285" height="719" alt="image" src="https://github.com/user-attachments/assets/eede294c-f333-4688-8ff0-ca3230e1e43a" />

Flow of Funds Explanation: 

1. Deposit Flow (User → Vault):

- User deposits funds from their non custodial Joinn Smart Account into the Joinn Stock Token Vault
- The Stock Token Vault has an automated strategy to buy and sell the relevant RWA in order to maintain a 90:10 ratio (RWA’s : USDC (reserves))
- Funds from the Stock Token Vault are used to purchase stock tokens from the vault
- The protocol then interacts with RWA Providers to acquire the necessary tokenized RWA’s
- These tokens are acquired and stored in the relevant Stock Token Vault vault maintaining the target ratio

2. Withdrawal Flow (Vault → User):  

a) Scenario 1 - Sufficient USDC Available in Stock Token Vault:
- User requests to exchange their stock tokens for USDC
- If there's enough USDC in the vault, the withdrawal processes immediately
- After withdrawal, the system rebalances the vault back to 90:10 ratio by:
    - Converting necessary RWA tokens through our RWA partner network to USDC
    - Maintaining the target reserve ratio 

b) Scenario 2 - Insufficient USDC Available to fulfill order:

- User requests withdrawal
- System detects insufficient USDC in vault
- User receives the total amount of USDC in Stock Token Vault to partially fill their order
- Order is placed with our RWA partner network to sell RWA Tokens from the Stock Token Vault in order to a) Top up USDC reserves in the Stock Token Vault to the desired ratio and b) Fulfill the residual balance of users order
- User automatically receives their USDC
- Vault rebalances to the 90:10 ratio

Key Components:

- Non Custodial Platform: Through simple social logins, users can seamlessly create a non-custodial Joinn Smart Account
- Non Discretionary Platform: User always has discretion over there investments and know exactly what they are investing in.
- Users go through KYC/AML checks in order to access Joinns RWA products.
- The first time a User connects to the platform they receive an Account Abstraction Account (smart contract wallet) unique to only them in order to provide a semaless user experience with gasless transactions and session tokens (User Account). 
- Only the User has access to their Joinn Smart Account
- Stock Token Vault: Maintains the 90:10 ratio of assets
- Smart Contracts: Manage the automated processes of the protocol by buying/selling and maintaining vault asset ratios.
- The system is designed to maintain liquidity while offering exposure to Tokenized RWA’s, with USDC serving as the liquid portion of the reserve structure.
