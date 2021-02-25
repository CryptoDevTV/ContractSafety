# ContractSafety

## Checklist

### 1. Contract:

#### 1.1 Is verified on Etherscan?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Smart contracts are stored on Ethereum blockchain in bytecode (mainly for optimization reasons) so to be sure that the source code of the contract stored on blockchain is the same as the one published on GitHub or on project page, project team should also verifiy it on Etherscan by providing the raw source code. Etherscan than compares the bytecode of this provided source code with bytecode stored on Ethereum blockchain.

#### 1.2 Is ERC-20 compatible?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > If the contract under reviewed is the token contract (not staking contract, dao etc.) it should be compatible with `ERC-20` standard to provide full functionality while using it.

#### 1.3 It is a proxy contract?
  * [ ] `YES`
  * [ ] `NO`
 
  ##### If yes, what is the address of the current main contract?
  
  ##### Why does it matter?
  > If the main contract is a proxy contract, its owner is able change contract functionality without changing contract address. While proxy contract is discovered during the review it is obligatory to also find the current contract behind this proxy.
  
#### 1.4 Allow for renounce ownership?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Renounce ownership is a good and common pattern for term called "burning keys". When contract owner is able to do this it is a good sign that he will do it in the future, after that no one will be able to interference with this how this smart contract works and no one will be able to call functions with `onlyOwner` modifier.
 
#### 1.5 Allow minting?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 1.6 Allow burning?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 1.7 Is pauseable?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 1.8 Is some kind of whitelist present?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 1.9 Is some kind of blacklist present?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 1.10 It is generated contract?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean
 
#### 1.11 How contract was funded (DEX, CEX, TornadoCash etc.)?
  * [ ] `DEX`
  * [ ] `CEX`
  * [ ] `TornadoCash`
  * [ ] `External address`
  * [ ] `Contract address`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

### 2. Owner:

#### 2.1 It is a contract or external address?
  * [ ] `contract`
  * [ ] `external address (multisig, dao)`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 2.2 Is deployer of this contract?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 2.3 Are management keys burnt?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

### 3. Liquidity:

#### 3.1 Available on Uniswap?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 3.2 Is locked (TeamFinance, UniCrypt)?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

### 4. Holders:

#### 4.1 Is Uniswap first?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean

#### 4.2 Is owner a main holder?
  * [ ] `YES`
  * [ ] `NO`
  ##### Why does it matter?
  > Short explenation why it is important and what does it mean
