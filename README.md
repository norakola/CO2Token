# CO2-Token-Reward-System
CO2 Token Reward System
This project is a CO2 Token Reward System designed to motivate companies to reduce their carbon emissions by leveraging blockchain technology. By implementing an ERC-20 token, named CO2, the system rewards companies for reducing their CO2 output and penalizes them if their emissions increase. The project consists of a smart contract written in Solidity, and a front-end React application that interacts with the blockchain via MetaMask.

# Overview
The system works by allowing users (companies) to input their electricity consumption and CO2 emissions. Based on this data, the system calculates the user’s average carbon footprint. If the user reduces their CO2 emissions over time, they are rewarded with CO2 tokens. If their emissions worsen, these tokens are burned (penalizing the user). The main objective is to create an incentive for companies to lower their carbon output and encourage environmental responsibility.


# Step-by-Step Guide: Earn CO2 Tokens on Your MetaMask Wallet
Prerequisites:
MetaMask Wallet: You need to have the MetaMask Wallet installed as a browser extension to log in.

Sepolia Testnet: You’ll need Sepolia ETH (Testnet currency) to cover the gas fees for transactions. You can get Sepolia ETH for free from a faucet-> https://www.sepoliafaucet.io/.

Node.js & npm: Ensure you have Node.js and npm (Node Package Manager) installed on your computer to run the web application.

# 1. Install and Set Up MetaMask:
Install MetaMask Wallet:

Go to MetaMask and install the browser extension (for Chrome, Firefox, etc.).
Create a new wallet or import an existing one.

# Add Sepolia Testnet:
Open MetaMask and select the network dropdown at the top.
Choose "Sepolia Test Network" or add it manually by selecting "Add Network" and entering the following details:

Network Name: Sepolia

New RPC URL: https://sepolia.infura.io/v3/YOUR_INFURA_KEY

Chain ID: 11155111

Currency Symbol: SEP (Sepolia ETH)

Get Sepolia ETH for Gas Fees:
To make transactions on the Sepolia Testnet, you need Sepolia ETH.
You can request Sepolia ETH from a faucet such as Sepolia Faucet.

# 2. Download and Run the Web Application:
Clone the Repository:
Open your terminal or command line.
Clone the repository to your local machine using the following command:

git clone https://github.com/your-username/your-repository.git

# Install Dependencies:
Navigate to the cloned repository folder:

cd your-repository

Install the necessary packages:

npm install

# Run the Web Application:
Start the web application with the following command:

npm run

# 3. Use the Web Application:
Open the Website:

Once you run npm run, the application will start on your local server (usually at http://localhost:3000).

Open this URL in your browser to access the web application.


# Log in with MetaMask:
The web application should prompt you to connect with your MetaMask Wallet. Click "Connect with MetaMask."

MetaMask will open, and you can confirm the connection.


# Enter Your Electricity Costs:
Input your monthly electricity costs into the application.
Based on your input, CO2 tokens will be calculated and credited to your MetaMask Wallet.

# 4. What's Happening Behind the Scenes?
CO2 Tokens: CO2 tokens are credited to your MetaMask Wallet in the Sepolia Testnet. These tokens represent the amount of CO2 saved based on your electricity costs.
Gas Fees: Every transaction in the testnet requires gas fees, which are paid in Sepolia ETH. This covers the transaction cost for writing data to the blockchain.

# 5. Conclusion:
Now you have a complete guide on how to use the web application, input your electricity costs, and earn CO2 tokens. Make sure you always have enough Sepolia ETH in your wallet to cover gas fees for transactions.

Enjoy experimenting with CO2 tokens!

# Additional Notes:
Testnet vs Mainnet: Note that these transactions are happening on the Sepolia Testnet. On the mainnet, real ETH and CO2 tokens would be used.
Gas Fees: Sepolia ETH is only for testnet purposes and has no real value. It's only used to cover gas fees for transactions.


# Key Features:
CO2 Token (ERC-20): A custom cryptocurrency built using the ERC-20 standard.

Reward System: Companies earn CO2 tokens as a reward for reducing their carbon emissions.

Penalty System: If the average electricity consumption (and thus the CO2 emissions) increases, tokens are burned from the user's wallet.

Real-Time CO2 Tracking: Users can track their CO2 emissions and energy consumption, see their improvements or regressions over time, and view the status of their CO2 token balance.

Smart Contract: Written in Solidity, the contract manages the CO2 token operations.

Frontend Application: A React.js app that connects to the smart contract and displays the user data, including the current energy consumption, CO2 emissions, and CO2 token balance.



# Project Structure
CO2-Token-Reward-Sytsem/

   |-CO2/
   
      |--contracs/
         |--- CO2Token.sol         # The ERC-20 Smart Contract for the CO2 token
         
      |--scripts/
         |---deploy.js             # Deploying the Smart Contract Address   
         |---hardhat.config.js     # Node Provider
         
      |--artifacts/   
         |--contracts/ 
           |---CO2Token.json       # ABI (defines the methods to interact with the smart 
                                    contract, both frontend and backend.)    
      |-react-app /
        |--src/
           |---App.js                # The React app that connects the smart contract to the 
                                     frontend

  

# How It Works
1. Smart Contract: CO2Token.sol
The smart contract defines the CO2 token (an ERC-20 token) and handles all token transfers and burning logic based on the user’s electricity consumption and CO2 emissions.

Reward Mechanism: Whenever a user submits their energy consumption data and CO2 emission improvements, the contract will reward them with CO2 tokens.
Penalty Mechanism: If the user’s average consumption increases (and CO2 emissions worsen), the smart contract will burn a set amount of their CO2 tokens as a penalty.

React Application: App.js
The React app is responsible for connecting the smart contract to the front-end. It interacts with the MetaMask wallet and allows the user to input their energy data, track CO2 emissions, and view their token balance.

MetaMask Integration: The React app communicates with MetaMask to allow users to send and receive CO2 tokens (with web.js)

Tracking CO2 Emissions: The app displays the user’s average electricity consumption, CO2 emissions in tons, and token balance in real time.

Frontend Interactions: Users can input their energy data, view whether they’re improving or worsening their emissions, and check if they are being rewarded or penalized.

# Technologies Used
Solidity: Smart contract language used to develop the CO2 token.
Ethereum: Blockchain platform for deploying the smart contract.
React.js & JavaScript: Frontend framework for building the web application.
Web3.js & ethers.js: Library to interact with the Ethereum blockchain from the frontend.
MetaMask: Browser extension that allows users to interact with the Ethereum network via their wallet.
Alchemy : Connects the app to the Ethereum Sepolia testnet via the ALCHEMY_SEPOLIA_ENDPOINT, a node.
