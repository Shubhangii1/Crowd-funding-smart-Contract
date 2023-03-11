CrowdFunding Smart Contract
This smart contract is designed to implement a crowdfunding platform using the Ethereum blockchain. It is written in the Solidity programming language and uses the Ethereum Virtual Machine (EVM) to execute the code.

How it works
The contract allows people to contribute ether to the contract, and if the total contributions reach a predetermined target amount before a deadline, the funds will be released to the project owner or recipient. If the target is not reached by the deadline, the contributors can withdraw their contributions.

The contract has several features, including:

minimumContribution: The minimum amount of ether that a contributor can contribute to the contract.
deadline: The deadline by which the target amount must be reached.
target: The target amount of ether that must be raised for the project to be funded.
raisedAmount: The total amount of ether raised by the contributors.
noOfContributors: The number of contributors who have contributed to the contract.
Request: A struct that contains information about a payment request made by the project owner or recipient.
requests: A mapping that stores all the payment requests made by the project owner or recipient.
The contract owner or manager can create a payment request by calling createRequests. Contributors can then vote on the request by calling voteRequest. Once a request has received a majority of votes from the contributors, the manager can call makePayment to release the funds to the recipient.

Usage
To use this smart contract, you will need to deploy it on the Ethereum blockchain using a tool such as Remix or Truffle. Once deployed, contributors can send ether to the contract by calling sendEth. The contract owner or manager can create payment requests using createRequests, and contributors can vote on them using voteRequest. When the target amount is reached, the manager can call makePayment to release the funds to the recipient. If the target is not reached by the deadline, contributors can withdraw their contributions using refund.
