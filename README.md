# How to use:
## Smart Contract

1. First fork the Attax repository, then seperate smart-contract folder and open in your code editor (VS Code).
2. Then do 'npm install' at smart-contract folder level in your terminal.
3. Do 'npm install dotenv --save' and create ".env" file at the root level of smart-contract.
4. Change `API_URL`(create an account in Alchemy, generate an api key there, then copy and paste the https link) and `PRIVATE_KEY`(get it from your web3 wallet like metamask) in the "hardhat.config.js".
5. Make sure solidity version is same in all files, otherwise you will get error.
6. Do 'npx hardhat compile', after that do 'npx hardhat run scripts/deploy.js --network polygon_mumbai'. After successful deployment you will get a message like 'Contract deployed to: 0x13D5939cbE332A8173d54405d091FF687714F367' on the console.
7. Now copy and save the deployed contract address safely. Also don't close the code editor, we will use it in our frontend part.

## Front-end

- For this you can use either Replit or do in your local-host. I prefer Replit because it is easy for application deployment.
1. Now seperate our second folder Attax(it is your frontend) inside the forked Attax repository, upload it into your replit  {or}  fork this repil "https://replit.com/@sivasankarkk/Attax#src/utils/MyEpicGame.json".
2. Now you need to carefully do below two things:
3. Get the deployed contract address that you saved earlier and paste it at `CONTRACT_ADDRESS` in "src/constants.jsx".
4. Open our previous section smart-contract folder, go to "artifacts/contracts/MyEpicGame.sol/MyEpicGame.json" & copy the entire "MyEpicGame.json".
   Now open replit, go to "src/utils/MyEpicGame.json", delete the entire data inside it and paste what you have copied from your smart-contract.
   
### Whoo that's it, now your app is ready. Show it to the world with your deployed Replit link.
