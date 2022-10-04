# NFT Marketplace

This repo contains boilerplate code for making an NFT Marketplace using React and Solidity. Using this boilerplate, you can make a website using which NFTs (Non-Fungible Tokens) can be purchased and owned by users.

This is a project available on Codedamn which helps you to learn key concepts of Blockchain and Web3 by building an NFT Marketplace. If you want to have a hands on experience of building a DApp that can be used in real-world and learn key concepts of Blockchain and Web3 by practicing, feel free to attempt this cool challenge. 

Feel free to check out the Codedamn Web3 Learning Path to learn more about How to Become a highly-skilled Blockchain Developer.

## What's Already Done for You

- The React App is already set up for you
- A Hardhat Environment is already setu up using which you can communicate with Solidity Smart Contract and perform other different cryptography functions. 
- The A Basic Smart Contract based on ERC-721 Standards is also written for you.
- The assets (images to be used as NFT and their metadata, and a question mark logo image).

## What you need to do

Your task is to make a frontend for the DApp (Decentralised App) using React JS. You can use Material UI for the purpose, or can also create a frontend from scratch. For reference of how the UI should potentially look like, you can refer the image below

![UI-Reference.png](https://raw.githubusercontent.com/navyansh007/nft-marketplace-project/master/UI%20Reference.png)

After making the frontend, define the functions in the smart contract to mint an NFT in exchange of some crypto tokens (like Ethereum), and current token ID, etc. After defining all required functions in the smart contract, call those functions in the frontend to make a usable DApp.

The DApp should have following functions:

- Ability to authenticate users using Ethereum Wallet, like Metamask
- Ability to mint an NFT by paying some amount
- Hide NFTs with a question mark which are not yet minted. The Question Mark image can be found in assets.
- Show minted NFTs from their IPFS address. For this, you need to upload the ```nfts``` folder under ```assets``` folder to the IPFS. You can use [Pinata](https://www.pinata.cloud/) to upload it to IPFS.
- Keep track of the ID of each NFT minted.

## How to run the project

After cloning this repo, you need to follow these steps:

- In the project folder, install required dependencies using ```npm install``` command.
- Run ```npx hardhat node``` command to make a local blockchain, in which you can do development locally. It will give you some wallets to interact with.
- Import any one of those provided wallets into your Ethereum Wallet. Make sure to have your network as ```localhost```
- Run the ```deploy.js``` script under ```assets``` folder using ```npx hardhat run ./scripts/deploy.js --network hardhat``` to deploy the smart contract on local blockchain. You will get the smart contract address after deployment.
- You will get the ABI of the smart contract under the ```artifacts``` folder in ```src```
- Start modifying the ```App.js``` file in ```src``` to see some changes in the frontend.
