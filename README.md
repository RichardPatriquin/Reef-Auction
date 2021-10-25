# A Decentralized Auction To Raise Money For The Great Barrier Reef 
## Description
This Decentralized Application uses Solidity, JavaScript, and HTML/CSS for deployment on the Ethereum Blockchain.
![Homepage](https://github.com/RichardPatriquin/Reef-Auction/blob/main/images/homepage.png)

## Development Enviroment
Before our Dapp can run there are a few technical requirement before we start. Please install:
- Ganache
- Node.js
- Web3.js
- Lite-server
- Truffle

## Directory Structure
The directory structure used for this Dapp was created using Truffle Box. Truffle Box contains modules, Solidity contracts & libraries, front-end files. We used the pet-shop suite https://www.trufflesuite.com/tutorial to build upon.
First create a directory, then inside the directory type:
```
$truffle unbox pet-shop
```
![Directory](https://github.com/RichardPatriquin/Reef-Auction/blob/main/images/directory.png)
The important folders in the directory include:
- `contracts`: Contains the code for the Auction smart contract
- `migrations`: Contains the JavaScript scripts to deploy and run migrations 
- `src`: Contains the JavaScript and HTML/CSS and images for the front end, as well as the code that enables interaction with the smart contract


## Instructions for Local Deployment
1. Download the prerequisites to run the application. 
2. Run Ganache, and connect MetaMask to Ganache.
3. Clone the repo
```
$ git clone https://github.com/RichardPatriquin/Reef-Auction.git
```
4. Migrate to root folder of the repo
5. If you would like to reinitialize the app (if for example, you used this application in the past), you will need to delete any `.json` files in `build/contracts`

6. Compile the contracts `Auction.sol` and `Migrations.sol` located in `contracts/`
```
$ truffle compile
```
7. Migrate the contract to your local server through Ganache. The contract needs to be compiled (Step 6) before it can be migrated
```
$ truffle migrate
```
8. Run the local server
```
$ npm run dev
```

**Note:** Steps 6 will create a new folder directory `build/contracts` with `.json` files for the smart contract `Auction.sol` and `Migrations.sol`. These `.json` files contain the "contract" information used to run the app locally

## Team
- [Richard Patriquin](https://github.com/RichardPatriquin)
- [Yohei Waki](https://github.com/Y-eddiee)
- [Shahadath Farouk](https://github.com/shahadh999)
- [Simon Sakkal](https://github.com/simongs10)
- [Matthew Buchanan](https://github.com)

## Future Work
- Function to relist your reef for sale
- 