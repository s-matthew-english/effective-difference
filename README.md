### The Quorum Node includes the following modifications to geth:

## ‘Proof of work’ consensus algorithm has been replaced with ‘QuorumChain’ consensus, a vote-based consensus mechanism.

This constitutes one of the most salient differences, additional information
can be found in the Quorum codebase at: 

https://github.com/jpmorganchase/quorum/blob/master/raft/doc.md

## The P2P layer has been modified to only allow connections to/from permissioned nodes.


## The block generation logic has been modified to replace the ‘global state root’ check with a new ‘global public state root’.


## The block validation logic has been modified to replace the ‘global state root’ in the block header with the ‘global public state root’


## The State Patricia trie has been split into two: a public state trie and a private state trie.


## Block validation logic has been modified to handle ‘Private Transactions’


## Transaction creation has been modified to allow for Transaction data to be replaced by encrypted hashes in order to preserve private data where required


## The pricing of Gas has been removed, although Gas itself remains
