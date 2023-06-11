## Introduction

Solidity is the primary language for creating smart contracts on blockchain platforms like Celo. Decentralized Autonomous Organizations (DAOs) are one of the significant applications of these smart contracts, allowing a community to govern resources or make decisions collectively. This challenge involves building a simple DAO using Solidity.

## Problem Statement

Design a smart contract that simulates a basic DAO with the following requirements:

1. The contract should allow users to submit proposals.
2. The contract should enable DAO members to vote on proposals. A member's voting power should be proportional to the amount of DAO tokens they hold.
3. The contract should enforce a deadline for voting on each proposal.
4. After the deadline, the contract should automatically execute the proposal with the most votes.
5. The contract should prevent the same address from voting multiple times on the same proposal.

## Hints

- Use a `struct` to define a proposal with attributes such as proposal ID, content, vote count, and deadline.
- Use a `mapping` to link proposal IDs with their respective proposal data and to keep track of votes.
- Use `msg.sender` to identify the address that is interacting with the contract.
- Implement checks in the voting function to prevent multiple votes and ensure only valid DAO token holders can vote.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and fulfill all the requirements.
- **Readability**: The contract should be well-documented, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

Please note, this challenge is a simplified version of a DAO and doesn't cover aspects like security, efficiency, and upgradability, which are critical in a real-world DAO contract.

For a comprehensive understanding of Celo smart contracts and Solidity, please refer to the Celo and Solidity tutorials.

## Submission

Please reply with a link to your PR on GitHub, including your DAO contract. Also, include any notes or comments you think are necessary to understand your design and choices. Lastly, provide a brief explanation about how each function of the contract should be tested.
