# Upgradeable_Voting_smart_contract

Lab lesson 2: upgradabiliy
Making an upgradeable voting smart contract

Create a smart contract( which can be upgraded) where people can submit proposals and vote on them.
The owner can upgrade the smart contract to add functionality and fix bugs

Adding a proposal is free(apart from the gas cost of course). 
A proposal only contains the id(uint) of the proposal, you can assume that the additional information about the proposal can be found online.

Voting on a proposal costs 0.5 Ether, this is configurable by the owner of the smart contract.
The person who submitted the winning proposal gets the money from all the votes as a reward.

A proposal wins if it has  the most votes, the owner can customize the "win schedule".
For example: a proposal must get at least half of the votes)
You do not need to implement  an additional "win schedule", you may assume that the owner will implement any new win schedule if required.
The win scheme should get the list of proposals with votes and return only the id of the winning proposal.

After 1000 blocks, no more voting is possible. Only the function that calculates the winner can still be executed.

Once the winner has been calculated, the winner can receive his Ether(don't forget to use the design patterns from the first lesson!).

This is an individual task that counts for daily work. You only need to create the Solidity code, no website needs to be created. You may put multiple contracts in a zip.
Only .sol  and .zip are valid.
