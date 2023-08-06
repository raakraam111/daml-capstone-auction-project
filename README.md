# daml-capstone-auction-project

This project is built on top of DAML SDK 2.6.4 using empty skeleton.
# Auction Platform with DAML

This project is an implementation of a simple Auction Platform using DAML (Digital Asset Modeling Language). The platform allows auctioneers to create auctions, bidders to participate and bid on items, and the auctioneer 

## Introduction

This is a simple auction project written in DAML. A smart contract where sellers can propose items for sale along with a trigger price. Potential buyers can accept the proposal by placing bids. Auction can end in two scenarios.

1. If the highest bid exceeds the trigger price, the contract accepts the proposal, and the highest bidder wins the item.
2. If Seller decides to end the auction, the contract accepts the proposal, and the highest bidder at that point of time wins the item.

Also note Only AuctionAccount holders with enough balance can place bids.
It is built as a part of DAML Fundamentals certification.
 

## Getting Started

To run this project locally, you'll need to have DAML SDK installed on your machine. Follow the official DAML documentation to install the SDK: [DAML SDK Installation](https://docs.daml.com/getting-started/installation.html)

### Cloning the Repository

First, clone this repository to your local machine using the following command: 

### Running the Tests

To run the test scenarios for the auction platform, you can use the DAML Script feature to execute the defined test scripts.

1. Open a terminal window and navigate to the root directory of the project.

2. Run the tests using the following command:
    
    ```daml test```

### Running the Project

To run the project, you can use the DAML Sandbox feature to spin up a local instance of the ledger.

1. Open a terminal window and navigate to the root directory of the project.

2. Run the project using the following command:
    
    ```daml start```

    This will start the sandbox and deploy the auction platform on the ledger.


This will execute the defined test scenarios and verify the correctness of the auction platform's behavior.

## Project Structure

The project is organized into three DAML modules:

1. `Main.daml`: Contains the main templates and choices to implement the auction platform.

2. `Test.daml`: Contains test scripts to verify the functionality of the auction platform.

3. `Setup.daml`: Contains setup scripts to create test parties and auction accounts for testing.

## Supported Functionality

The auction platform mainly supports the following functionalities:

- Auctioneer can create auctions and set reserve prices for items.
- Bidders can create and verify their accounts to participate in auctions.
- Bidders can deposit funds into their accounts.
- Bidders can place bids on active auctions.
- The auctioneer can close the auction manually or automatically when the reserve price is reached.
- Bidders cannot bid on closed auctions.
 

