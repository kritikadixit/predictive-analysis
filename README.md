# TrendPredictor Smart Contract

## Description
TrendPredictor is a simple Solidity smart contract designed to store and retrieve AI-generated trend predictions on the blockchain. Users can submit trend predictions, which are stored in a public ledger, ensuring transparency and immutability. The contract allows users to retrieve specific predictions and check the total number of predictions made.

## Features
- Submit AI-generated trend predictions.
- Store predictions permanently on the blockchain.
- Retrieve predictions by index.
- View the total number of predictions submitted.

## How It Works
1. A user submits a trend prediction using the `submitPrediction` function.
2. The prediction, along with the sender's address and timestamp, is stored on-chain.
3. The contract emits an event `NewPrediction` to notify listeners of a new prediction.
4. Users can retrieve predictions using the `getPrediction` function.
5. The `getTotalPredictions` function returns the number of predictions stored.

## Deployment
To deploy the contract:
1. Compile the contract using Solidity version 0.8.0 or later.
2. Deploy it on Ethereum or any compatible EVM blockchain.
3. Use a frontend or scripts to interact with the contract.

## Example Usage
- **Submit a prediction:**
  ```solidity
  trendPredictor.submitPrediction("AI will revolutionize education");
  ```
- **Retrieve a prediction:**
  ```solidity
  (string memory trend, uint256 timestamp, address predictor) = trendPredictor.getPrediction(0);
  ```
- **Check total predictions:**
  ```solidity
  uint256 total = trendPredictor.getTotalPredictions();


DEPLOYED CONTRACT ADDRESS- 0x02A614883Df4732809Fa7DdE4c2A674De5b4041b
