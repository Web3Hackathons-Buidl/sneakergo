# sneakergo
Step 1: Use Cli to upload Assets. Create Sneaker Cards
Deploy separate Contracts for Each Asset in Sneaker collection: ERC1155 Edition
Const Heel.sol contract address =
Const Sole.sol contract address = 
Const Laces.sol contract address =
Const Upper.sol contract address =
Const panels.sol contract address =
Const Vamp.sol contract address = 
Const Logo.sol contract address =
Const SerialNumber.sol contract address =


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
