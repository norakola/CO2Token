# CO2 Token Reward System
The CO2 Token Reward System uses blockchain technology to encourage companies to reduce their carbon emissions. By implementing an ERC-20 token called CO2, the system rewards companies with crypto tokens for lowering their emissions and penalizes them by burning tokens if their emissions increase. These tokens are credited or burned directly in the user's MetaMask wallet.

The system consists of a Solidity smart contract and a React frontend application, which interacts with the blockchain via MetaMask.

# How It Works:
Companies input their electricity consumption and CO2 emission data. The system calculates their average carbon footprint and rewards them with CO2 tokens, which are credited to their MetaMask wallet when emissions are reduced. If emissions increase, tokens are burned as a penalty. The goal is to encourage companies to lower their carbon output and promote environmental responsibility.


# Step-by-Step Guide: Earn CO2 Tokens on Your MetaMask Wallet
Requirements:
MetaMask Wallet: You need to have the MetaMask Wallet installed as a browser extension to log in.

Sepolia Testnet: You’ll need Sepolia ETH (Testnet currency) to cover the gas fees for transactions. You can get Sepolia ETH for free from a faucet -> https://www.sepoliafaucet.io/.

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
You can request Sepolia ETH from a faucet such as Sepolia Faucet. -> https://www.sepoliafaucet.io/.

# 2. Download and Run the Web Application:
Clone the Repository:
Open your terminal or command line.
Clone the repository to your local machine using the following command:

git clone https://github.com/norakola/CO2Token.git

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


# Key Features and How It Works:
CO2 Token (ERC-20): Custom cryptocurrency built to track CO2 emissions and reward users.

Reward System: Users earn CO2 tokens for reducing their energy consumption and CO2 emissions.

Penalty System: Tokens are burned if a user’s electricity consumption increases, resulting in higher CO2 emissions.

Smart Contract (CO2Token.sol): Written in Solidity, it handles token transfers, rewards, and penalties based on energy data.

React.js Frontend (App.js): Connects to the smart contract and MetaMask wallet, displaying energy data, CO2 emissions, and token balance.

MetaMask Integration: Users interact with the app via MetaMask to send and receive CO2 tokens using web3.js.

Real-Time Tracking: Displays real-time tracking of energy consumption, CO2 emissions (in tons), and token balance.

Frontend Interactions: Users can input energy data, track improvements or regressions, and view their rewards/penalties.



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

  

# Technologies Used
Solidity: Smart contract language used to develop the CO2 token.
Ethereum: Blockchain platform for deploying the smart contract.
React.js & JavaScript: Frontend framework for building the web application.
Web3.js & ethers.js: Library to interact with the Ethereum blockchain from the frontend.
MetaMask: Browser extension that allows users to interact with the Ethereum network via their wallet.
Alchemy : Connects the app to the Ethereum Sepolia testnet via the ALCHEMY_SEPOLIA_ENDPOINT, a node.

Enjoy experimenting with CO2 tokens!
