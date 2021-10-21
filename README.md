# A Decentralized Auction To Raise Money For The Great Barrier Reef 
## Description
This Decentralized Application uses Solidity, JavaScript, and HTML/CSS for deployment on the Ethereum Blockchain.

## Development Enviroment
Before our Dapp can run there are a few technical requirement before we start. Please install:
- Ganache
- Node.js
- Web3.js
- Lite-server
- Truffle

## Directory Structure
The directory structure used for this Dapp was created using Truffle Box. Truffle Box contains modules, Solidity contracts & libraries, front-end files. We used the pet-shop suite to build upon.
> mkdir reef-auction
>
> cd reef-auction
>
>truffle unbox pet-shop

The important folders in the directory include:
- `contracts`: Contains the code for the Auction smart contract
- `migrations`: Contains the JavaScript scripts to deploy and run migrations (adapted from the tutorial)
- `src`: Contains the JavaScript and HTML/CSS for the front end, as well as the code that enables interaction with the smart contract
- `test`: Contains the unit tests for the smart contract

## Instructions for Local Deployment
1. Download the prerequisites to run the application. 
2. Run Ganache, and connect MetaMask to Ganache. Detailed instructions for this step can be found in Sections 3.1 and 3.2 in `documents/setup_instructions.pdf`
3. Clone the repo
```
$ git clone https://github.com/RichardPatriquin/Reef-Auction.git
```
4. Migrate to root folder of the repo
5. If you would like to reinitialize the app (if for example, you used this application in the past), you will need to delete any `.json` files in `build/contracts`
6. Test the contract functions using unit tests specified in `test/TestAuction.sol` (not essential)
```
$ truffle test
```
7. Compile the contracts `Auction.sol` and `Migrations.sol` located in `contracts/`
```
$ truffle compile
```
8. Migrate the contract to your local server through Ganache. The contract needs to be compiled (Step 7) before it can be migrated
```
$ truffle migrate
```
9. Run the local server
```
$ npm run dev
```

**Note:** Steps 6/7 will create a new folder directory `build/contracts` with `.json` files for the smart contract `Auction.sol` and `Migrations.sol`. These `.json` files contain the "contract" information used to run the app locally

## Team
- [Richard Patriquin](https://github.com/RichardPatriquin)
-

## Questions/Contributions/Future Work
- The app does not have payment processing for bids and doesn't track money. As it stands, it's a CRUD application where the web3 wallet only requests the wallet holder to pay gas fees for computation
- The app doesn't allow users to create their own auctions
- There's no start and end time for auctions so bids can be placed indefinitely
- There's no ability to associate the final item to a wallet. More work needs to be done with tokenizing items and associating wallets to tokens
- Improvements can be made to the UI. Some examples of improvements include:
  1. Better front end interactivity for the requirements in the smart contract backend. Currently, the submit button is not active if the requirements of the bid are not met. Someone could easily design JS functionality to improve the UI.
  2. More attractive HTML/CSS layout
- Refer to the executive summary located at `documents/executive_summary` for a more detailed description of future projects and work that can be done to improve this app
- Please reach out to either of us for any other feedback
