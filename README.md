Full Stack ERC20 App

This repository contains a complete full-stack ERC20 application, including the smart contract backend, a web-based DApp, and a mobile-friendly frontend.

The project demonstrates how an ERC20 token can be created, deployed, and interacted with across different platforms using Web3 technologies.

Project Overview

Backend

ERC20 smart contract written in Solidity

Web Frontend

Lightweight Web3.js DApp

Mobile Frontend

JSON-based mobile interface (Jasonette-style)

This repository explains how all components work together and provides a simple workflow for deploying the contract and connecting both web and mobile clients.

1. Backend (Smart Contracts)

The backend consists of Solidity smart contracts that implement the ERC20 token standard.

The majority of the ERC20 logic is based on trusted OpenZeppelin implementations to ensure security and reliability.

Contracts Used

ERC20

ERC20Basic

SafeMath

StandardToken

BasicToken

These contracts handle token transfers, balances, and total supply logic.

Custom Contract

ExampleToken.sol

This is the only customized contract in the project. It defines:

Token name

Symbol

Decimals

Initial total supply

No development frameworks such as Truffle or Hardhat were used to keep the setup simple and transparent.

Deployment

To deploy the contract:

Open Remix IDE

Copy all files from the contracts folder

Compile and deploy the contract to an Ethereum network (testnet recommended)

Once deployed, copy the contract address.
This address is required for both the web and mobile applications to interact with the token.

2. Web Frontend

The web application is implemented as a single HTML file that interacts directly with the deployed ERC20 contract.

Key Points

Uses Web3.js

No build tools or compilation required

Entire logic is visible in the source code

Connects to the deployed ERC20 contract using its address

Allows users to:

View token balances

Send tokens

Interact with the contract through a browser wallet

This approach keeps the DApp easy to understand and beginner-friendly.

3. Mobile Frontend

The mobile version is built using a JSON-based, markup-driven approach inspired by Jasonette.

The mobile app is view-based and consists of multiple screens:

Views

Main View

Displays token information

Allows token transfers

Private Key Scanner

Imports a user wallet via QR code

Recipient Scanner

Scans a recipient address QR code for sending tokens

The mobile app connects to the same ERC20 contract used by the web app, ensuring consistency across platforms.
