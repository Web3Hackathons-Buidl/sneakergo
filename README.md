```markdown
# SneakerGo

![SneakerGo Logo](assets/sneakergo-logo.png)

SneakerGo is a decentralized platform that allows users to buy, sell, and trade limited-edition sneakers using blockchain technology. By leveraging Web3 and smart contracts, SneakerGo ensures a secure, transparent, and trustless environment for the sneaker community.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Smart Contracts](#smart-contracts)
- [Contributing](#contributing)
- [License](#license)

## Features

- Buy, sell, and trade limited-edition sneakers on a decentralized platform
- Authenticate sneakers and verify ownership through blockchain technology
- Transparent transaction history and user ratings
- Secure, trustless environment for sneaker enthusiasts
- Verified listings from trusted sellers
- Low fees compared to traditional secondary markets

## How It Works

SneakerGO works as follows:

- Sellers can list limited sneaker items for sale on the platform by filling out details about the sneaker including photos, condition, size and asking price. Listings are recorded on the Polygon blockchain.
- Buyers can browse listings on the platform and purchase items using MATIC tokens.
- Once a buyer purchases an item, the funds are held in escrow until the buyer confirms they have received the item as described.
- Sellers ship the item to the buyer. Once the buyer confirms receipt and satisfaction, the funds are released from escrow and distributed to the seller.

## Prerequisites

Before you get started, make sure you have the following:

- Node.js (v14.x or higher)
- npm (v7.x or higher)
- MetaMask browser extension

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Web3Hackathons-Buidl/sneakergo.git
   ```

2. Navigate to the project directory:

   ````bash
   cd sneakergo
   ```

3. Install the dependencies:

   ````bash
   npm install
   ```

## Usage

1. Start the local development server:

   ````bash
   npm run start
   ```

2. Open your browser and navigate to `http://localhost:3000`.

3. Connect your MetaMask wallet and start using SneakerGo!

## Smart Contracts

SneakerGo's smart contracts are written in Solidity and deployed on the Ethereum blockchain. The main contracts are:

- `Sneaker.sol`: Represents a limited-edition sneaker with unique properties
- `SneakerMarket.sol`: Handles the buying, selling, and trading of sneakers

For more information about the smart contracts, please refer to the [Smart Contracts documentation](docs/SMART_CONTRACTS.md).

## Contributing

We welcome contributions from the community. If you'd like to contribute to SneakerGo, please follow these steps:

1. Fork the repository.
2. Create a new branch with a descriptive name.
3. Make your changes and commit them with a clear, concise message.
4. Push your changes to your fork.
5. Open a pull request in the original repository.

For more information, please read our [Contributing Guide](CONTRIBUTING.md).

## License

SneakerGo is released under the [MIT License](LICENSE).
```
# sneakergo
Step 1: Use Cli to upload Assets. Create Sneaker Cards
Deploy separate Contracts for Each Asset in Sneaker collection: ERC1155 Edition
Const Heel.sol contract address =0x241f87E7112BCA7E919d4f1842f399995a0adbd8
Const Sole.sol contract address = 0xB2e01A55228D9b2c5a3DF14139372E1A4A122c05
Const Laces.sol contract address = 0x587412e3B7245ee58E1f0D07F3B9D3cD1418221A
Const Upper.sol contract address = 0x917685185174530C62d5Ad591d36BE85f3c18f3F
Const panels.sol contract address = 0xC2a576e8778AE79A60E3142DE210EBA8f85d6dcd
Const Vamp.sol contract address = 0x5B9012ea223A9C312132055b3F61bf4Ba8EFf9cF
Const Logo.sol contract address = 0x39F19F1343C738cE80414f1ef1b0d2134D300f6F
Const SerialNumber.sol contract address = 0x98d2f5ad4d39c1A688F05f4d42dC2FA78397DceA


Step 2: Deploy Marketplace to List Items to purchase Registry Index. Buy Listings on Sneaker Marketplace: Marketplace contract address on my chainlet:0x6dd68485d463B57BF4ad649D36c2c16DA50e2925
Step 3: Deploy contracts to Mint the 3D Sneaker Assets. 
Step 4: Write a Sneakerbox Script. Create a sneakerPack and add the contract addresses to the sneaker Pack that ‘owns’ the sneakerBox sneakerbox: 0x2b046C5F2286FB6f9FEF3e7486E7FCF50b535056
Step 5: Use Unity to Render 3D Sneaker Assets using SDK to fetch the Data
-Download the Thirdweb Unity SDK package 
-Import package via Assets in Unity 
-File > Build Settings > Switch to platform WebGL
-Player Settings > Resolution Presentation (ThirdWeb)
-other settings > “uncheck” “AutoGraphics”
Assets create a C# script add createAssetBundle
>Build AssetBundles
>BringPrefab over into assets
>AssetBundle > TestBundle
>BuildassetBundles>Files => upload to IPFS URI
>Terminal npx thirdweb@latest upload ./testbundle
Npx thirdweb@latest create –templae 3d-asset-nft-script
	Cd 3d-asset-nft-script
-replace -contract address 
-replace IPFS URI
-replace private Key (Metamask)
If you try to add your custom chainlet to Thirdweb make sure that you:
Add https:// + rpc node + “..jsonrpc.sp1.sagarpc.io”
ex:https://sneakerhunt-1685370732045988-1.jsonrpc.sp1.sagarpc.io
Make sure you add your chainlet to “mainnet” on Metamask go to the left on settings and ensure you have the same chainID in the Network ID in Thirdweb “Add Custom Network” you should name it “yourchainletname+mainnet” for network type select Mainnet and add your rpc url from step 1. Along with Currency symbol and an Image if you have one* then click “Add Network”
Deploy your contracts: NFT Collection, ERC1155 Edition, Pack, Marketplace.
SneakerGO [Sample Game] is now on @DoraHacks! Read more about this project - its vision, team, product updates on: https://dorahacks.io/buidl/6545
