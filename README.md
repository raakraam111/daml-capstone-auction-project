# daml-capstone-auction-project

This project is built on top of DAML SDK 2.6.4 using empty skeleton.
# Auction Platform with DAML

This project is an implementation of a simple Auction Platform using DAML (Digital Asset Modeling Language). The platform allows auctioneers to create auctions, bidders to participate and bid on items, and the auctioneer to close the auction when a reserve price is reached.

## Introduction

This is a simple auction project written in DAML. A smart contract where sellers can propose items for sale along with a trigger price. Potential buyers can accept the proposal by placing bids. Auction can end in two scenarios.

1. If the highest bid exceeds the trigger price, the contract accepts the proposal, and the highest bidder wins the item.
2. If Seller decides to end the auction, the contract accepts the proposal, and the highest bidder at that point of time wins the item.
3. Only AuctionAccount holders with enough balance can place bids.
4. Auction Participants can only place bids in USD Currency.


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

