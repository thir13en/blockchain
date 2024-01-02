# Bitcoin

It is a protocol that for the first time solved the problem of double spending in a digital currency.

## Miners
1. Process and confirm transactions
1. Create new blocks
1. Secure the network

## Hash functions
Bitcoin uses sha256 hash which generates unique hashes depending on the content of the block. Sha stands for Secure Hash Algorhythm, Hashes are one way funcitons, you cannot derive the original content of the file by it's hash with the current computation setup.

## Nonce
The number which combined with the block content and the hash function gives a hash signature with n amount of zeros at the beginning. Finding this number through computation resources and brute force is what it is known as Proof of Work mining.

## Block structure:
* block number
* Nonce
* Data/transactions
* Previous block hash
* Current block hash