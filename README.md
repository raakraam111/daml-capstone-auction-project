# daml-capstone-auction-project

## Introduction

This is a simple auction project written in DAML. A smart contract where sellers can propose items for sale along with a trigger price. Potential buyers can accept the proposal by placing bids. Auction can end in two scenarios.

1. If the highest bid exceeds the trigger price, the contract accepts the proposal, and the highest bidder wins the item.
2. If Seller decides to end the auction, the contract accepts the proposal, and the highest bidder at that point of time wins the item.
3. Only AuctionAccount holders with enough balance can place bids.
4. Auction Participants can only place bids in USD Currency.


It is built as a part of DAML Fundamentals certification.

## Prerequisites

This project is built on top of DAML SDK 2.6.4 using empty skeleton.

## Commands used
### Create a new project
daml new daml-capstone-auction-project
