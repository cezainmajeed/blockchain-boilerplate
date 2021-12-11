# blockchain-boilerplate

## Contracts

A Contract is an abstraction of an executable program on the Ethereum Blockchain. A Contract has code (called byte code) as well as allocated long-term memory (called storage). Every deployed Contract has an address, which is used to connect to it so that it may be sent messages to call its methods.

A Contract can emit Events, which can be efficiently observed by applications to be notified when a contract has performed specific operation. Events cannot be read by a Contract.

There are two types of methods that can be called on a Contract:

A Constant method may not add, remove or change any data in the storage, nor log any events, and may only call Constant methods on other contracts. These methods are free (no Ether is required) to call. The result from them may also be returned to the caller.

A Non-Constant method requires a fee (in Ether) to be paid, but may perform any state-changing operation desired, log events, send ether and call Non-Constant methods on other Contracts. These methods cannot return their result to the caller. These methods must be triggered by a transaction, sent by an Externally Owned Account (EOA) either directly or indirectly (i.e. called from another contract), and are required to be mined before the effects are present. Therefore, the duration required for these operations can vary widely, and depend on the transaction gas price, network congestion and miner priority heuristics.
