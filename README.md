# Create-a-Blockchain
A Blockchain transaction created with Python

This is a simple implementation of a blockchain in Python using Flask. It consists of two parts.

Part 1: Building a Blockchain
The first part is the creation of a Blockchain class. It has an initialization method which creates an empty list called chain and creates the first block with a proof of work and a previous hash of 0. It also contains methods to create a new block, get the previous block, calculate the proof of work, create a hash for a block, and check if a chain is valid.

Part 2: Mining our Blockchain
The second part is to create a web application to interact with the blockchain. It creates an instance of the Blockchain class and provides three endpoints. The /mine_block endpoint is used to mine a new block. The /get_chain endpoint returns the current blockchain. The /is_valid endpoint checks if the blockchain is valid.

When the /mine_block endpoint is called, it first retrieves the previous block from the blockchain, calculates the proof of work, creates a new block, and returns the block information with a message. The /get_chain endpoint returns the current blockchain and the length of the chain. The /is_valid endpoint checks if the blockchain is valid by iterating through the chain and checking if the hash of each block matches the previous hash, and if the proof of work is valid.

The app is run on the host 0.0.0.0 and port 5000.
