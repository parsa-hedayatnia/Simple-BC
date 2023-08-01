# Simple-BC
A blockchain is a time-stamped, decentralized set of fixed records that contain data of any size created by a large network of computers.
Those that are scattered around the world and do not belong to a single organization are controlled. Each block is secured using hash technology and to each other
It is connected, which protects it from being tampered with by unauthorized persons.
In this project, we will create a blockchain using Python, extract new blocks and display the entire blockchain.
This program implements a blockchain system using Python programming language. Running this program through a Flask web server
Takes. The commands related to the web server and the blockchain process are as follows:
First, the required modules for the program are imported, including datetime for timing, hashlib for hash calculation, and signature
digital, and json to store data in the blockchain. Also, Flask and jsonify modules to create a web server and display the blockchain
JSON format is used.
Then, a class called Blockchain is defined. In this class, operations related to the construction and management of blockchain have been implemented.
Some of the methods of this class are:
__init__: is the construction method that initializes the blockchain and creates the first block with zero hash.
block_create: adds a method to create a new block to the chain.
block_previous_print: returns a method to display the previous block.
work_of_proof: is a method that uses the Work of Proof algorithm to extract a new block by solving a computational problem.
takes action
Hash: A method is used to calculate the hash of a block.
valid_chain: A method that checks the validity of the blockchain.
Then, an instance of the Blockchain class named blockchain is created.
Then, using Flask decorators, three routes (endpoints) are defined for the web server:
block_mine:/ When this path is called, a new block is mined and its details are returned as JSON.
chain_get:/ When this path is called, the entire blockchain is returned as JSON.
valid:/ When this path is called, the validity of the blockchain is checked and the result is returned as JSON.
Finally, the Flask web server is run on the host 127.0.0.1 and port 5000 to enable communication with it and interaction with the blockchain.
By running the program and calling the mentioned paths, you can extract new blockchains, view the blockchain and check its validity.
