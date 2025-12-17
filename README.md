# Full Stack ERC20 App

This repository contains a complete full-stack ERC20 application, including a Solidity smart contract backend, a Web3.js web application, and a mobile-ready JSON frontend.

The project demonstrates how an ERC20 token can be created, deployed, and interacted with across multiple platforms using the same Ethereum smart contract.

---

## Project Overview

The application is divided into three main parts:

### Backend
- ERC20 smart contract written in Solidity  
- Based on standard ERC20 logic  
- Custom token configuration including name, symbol, decimals, and total supply  

### Web Frontend
- Browser-based decentralized application built with Web3.js  
- Connects directly to the deployed ERC20 contract  
- Allows users to view balances and send tokens  

### Mobile Frontend
- JSON-based mobile interface  
- Displays token information and supports token transfers  
- Uses QR code scanning for wallet and recipient addresses  

---

## Deployment

The smart contract can be deployed using Remix IDE by compiling and deploying the Solidity contracts to an Ethereum network.

Once deployed, the contract address is used by both the web and mobile applications to interact with the token.

---

## Purpose

This project is intended as a learning example of full-stack blockchain development, showing how smart contracts, web applications, and mobile interfaces can work together in an ERC20 ecosystem.
