# Bitcoin

It is a protocol that for the first time solved the problem of double spending in a digital currency.

The genesis block of Bitcoin, which is the first block in the Bitcoin blockchain, contains a notable comment or message left by its creator, Satoshi Nakamoto. The message is:
> "The Times 03/Jan/2009 Chancellor on brink of second bailout for banks."
This message is embedded in the coinbase parameter of the input of the first transaction. It serves not only as a proof that the block was created on or after January 3, 2009, but also as a politically charged statement. The message refers to a headline in The Times newspaper on that day, highlighting the instability of the traditional banking system and possibly providing an insight into one of the motivations behind the creation of Bitcoin, which offers a decentralized alternative to conventional banking.

## Miners
1. Process and confirm transactions
1. Create new blocks
1. Secure the network

## Hash functions
Bitcoin uses sha256 hash which generates unique hashes depending on the content of the block. Sha stands for Secure Hash Algorhythm, Hashes are one way funcitons, you cannot derive the original content of the file by it's hash with the current computation setup.

## Nonce
The number which combined with the block content and the hash function gives a hash signature with n amount of zeros at the beginning. Finding this number through computation resources and brute force is what it is known as Proof of Work mining. The word "nonce" stands for "number used once." It is a unique, often random or semi-random value that is used in cryptographic communication to prevent certain types of security attacks.
In mining, the goal is to find a nonce that, when used in combination with the block data, produces a hash that meets the network's **difficulty target**.

## Block structure:
* block number
* Nonce
* Data/transactions
* Previous block hash
* Current block hash

Expanding on the notes provided, let's delve deeper into the four key components of Bitcoin:

## Components of Bitcoin

### 1. Code
- **Foundation**: Bitcoin's codebase is the foundation of its existence. This open-source software defines the rules of the network and how the blockchain operates. 
- **Consensus Protocol**: A crucial part of the code is the consensus protocol, particularly Proof of Work (PoW), which governs how transactions are verified and blocks are added to the blockchain.
- **Updates and Governance**: The decentralized nature of Bitcoin means changes to the code require broad consensus among network participants, typically miners and node operators.

### 2. Cryptography
- **Securing Transactions**: Bitcoin uses cryptographic algorithms to secure transactions. Public key cryptography allows users to generate a cryptographic pair of keys: a public key (wallet address) and a private key (used to sign transactions).
- **Hashing**: Cryptographic hashing is integral to the blockchain's structure. Each block contains the hash of the previous block, creating a secure and unchangeable chain.
- **Ensuring Integrity**: Cryptography ensures the integrity and irreversibility of transactions, making Bitcoin resistant to fraud and hacking.

### 3. Hardware (Miners)
- **Mining Process**: Miners use specialized hardware to solve complex mathematical problems (hashing) that validate and secure transactions. This process is known as mining.
- **ASICs**: The most effective mining hardware are Application-Specific Integrated Circuits (ASICs), designed specifically for Bitcoin mining.
- **Energy Consumption**: Mining is a resource-intensive process, requiring substantial electrical energy, which has raised environmental concerns.

### 4. Game Theory to Give It Value
- **Incentives for Miners**: Miners are incentivized to maintain the network's integrity through block rewards (newly minted bitcoins) and transaction fees. This ensures a trustworthy system where miners are rewarded for following the rules.
- **Supply Limit**: Bitcoin's code limits its total supply to 21 million coins, creating scarcity and potential value appreciation over time.
- **Network Effects**: The value of Bitcoin is also driven by network effects; as more people use and trust the system, its value increases.
- **Speculative Investment**: Besides being a digital currency, Bitcoin is also seen as a speculative investment. Its value is influenced by investor sentiment, market trends, and macroeconomic factors.

## The Coinbase
The coinbase transaction is a unique type of transaction in the world of Bitcoin and other cryptocurrencies. It has several key characteristics that distinguish it from regular transactions:

1. **Creation of New Bitcoins**: The coinbase transaction is the first transaction in a new block. It is used by miners to introduce new bitcoins into circulation. This is the only way new bitcoins are created; they are "minted" as a reward for miners who successfully validate and add a new block to the blockchain.

2. **Block Reward**: The coinbase transaction includes the block reward, which is a specific amount of bitcoins given to the miner as an incentive for their computational work in verifying transactions and adding them to the blockchain. The block reward halves approximately every four years in an event known as the "halving." This process is designed to control the supply of new bitcoins, mimicking the scarcity and gradual release of precious metals like gold.

3. **Transaction Fees**: In addition to the block reward, the coinbase transaction also includes the transaction fees from all other transactions included in the block. Miners receive these fees as additional compensation, which becomes more important as the block reward decreases over time.

4. **Special Format**: The coinbase transaction has a special format. It does not require any inputs like regular transactions. Instead, it creates bitcoins from nothing. The input section of a coinbase transaction typically contains a block's height to ensure that each coinbase transaction is unique and to prevent potential double-spending issues.

5. **Message or Extra Nonce**: Miners often use the coinbase transaction to include a message or extra nonce value. For example, the very first block in the Bitcoin blockchain, known as the Genesis Block, contains a famous message left by its creator, Satoshi Nakamoto.

6. **Maturity Period**: Newly created bitcoins in a coinbase transaction have a maturity period of 100 blocks. This means that the miner has to wait until 100 additional blocks are added to the blockchain after their block before they can spend the newly minted bitcoins. This rule is in place to prevent various forms of fraud and attacks on the network.
