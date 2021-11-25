# DS_Coin106
This is an independent cyptocurrency made using the cryptographic concepts like hash functions,digital signatures with underlying data structures like linked list, queues, trees, etc.
## Introduction
This is a course project of the course COL106(Data Structures and Algorithms) taken by our course instructors [Prof. Amitabha Bagchi](https://www.cse.iitd.ac.in/~bagchi/) and [Prof. Venkata Koppula](https://iitd.irins.org/profile/214118). It involves processes very similar to actual cryptocurrencies which are mentioned further.\
Some basic conventions/technologies used in the project: 
* Every coin is a six digit unique number.
* Every transaction has the following information:
  * the coin being transferred
  * the source (that is, the person spending this coin)
  * the destination (that is, the person receiving this coin)
  * some information to indicate when the source received this coin from someone (this will be described     in more detail later).\
   For simplicity, we assume every transaction consists of exactly one coin.
* A ***transaction-block*** consists of a set of transactions. Let ***tr-count*** denote the number of transactions per block. The transaction-block will also have additional attributes, which will be discussed below.
* A ***blockchain*** is an authenticated linked list of transaction-blocks.
* ***Pending transactions*** and ***transaction-queue***: All the transactions in the transaction-block are processed
transactions. Additionally, we have a transaction-queue which contains ***pending transactions***. Every
new transaction is first added to the transaction-queue, and later moved to a transaction-block (and
thus added to the blockchain).
