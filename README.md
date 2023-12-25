# Health Insurance 

## Overview

This smart contract, written in Solidity, implements a basic health insurance system on the Ethereum blockchain. The contract allows individuals to apply for health insurance by providing their age and paying a premium. Once approved, the policyholder is marked as insured, and the contract keeps track of relevant details such as the policyholder's address, age, premium amount, and insurance status.

## Features

1. **Policyholder Information**: The contract stores information about the policyholder, including their Ethereum address, age, premium amount, and insurance status.

2. **One-Time Application**: The contract ensures that an individual can apply for insurance only once. Subsequent attempts to apply will result in a revert.

3. **Age Verification**: The applicant must be at least 35 years old to be eligible for insurance. This is enforced using a `require` statement.

4. **Age Range Check**: The contract includes an `assert` statement to check that the provided age is within a reasonable range (between 35 and 150 years).

5. **Premium Amount Check**: The applicant must pay a specific premium amount (500 Wei) for the insurance. If the provided premium is not exactly 500 Wei, the transaction will be reverted.

6. **Initialization**: The contract is initialized with default values, setting the policyholder to address 0 and marking the insurance status as false.

## Smart Contract Deployment

To deploy this smart contract, follow these steps:

1. Ensure you have the necessary tools to interact with the Ethereum blockchain (e.g., Remix, Truffle, or other development environments).

2. Set the appropriate Solidity compiler version (greater than or equal to 0.8.0) for deployment.

3. Deploy the contract to the Ethereum blockchain.

## How to Apply for Insurance

1. Call the `applyForInsurance` function, providing the desired age and the correct premium amount (500 Wei).

2. Ensure that the applicant's age is at least 35, or the transaction will be reverted.

3. Verify that the premium amount is exactly 500 Wei; otherwise, the transaction will be reverted.

4. The policyholder's address, age, premium amount, and insurance status will be updated upon successful application.

## Author

Gagana Deepika


