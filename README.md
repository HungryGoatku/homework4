# homework4 || I.A.
Made an old solidity contract compatible with version ^0.5.1 with Remix online IDE

## LINK for reference on old solidity contract
[Click here please](https://coursetro.com/posts/code/102/Solidity-Mappings-&-Structs-Tutorial)

# Requirements to run this smart contract
There are a few things you'll need to install beforehand.

By the way, I'm running this on Windows10 command line prompt

- Node.js : version 12.16.2 is what I'm running, depending on your machine you can run latest version.
[Link for Node.js](https://nodejs.org/en/)

- Truffle: This popular development framework will make it a breeze; Link will have command to install 
[Here's link for Truffle](https://www.trufflesuite.com/truffle)

- Ganache: Nice GUI for your Ethereum blockchain festivities; Link will lead you to download page
[Here's link for Ganache](https://www.trufflesuite.com/ganache)

- Git: Nice distritbuted version-control system; Link will lead you to download page whether Windows, MAC, Linux
[Here's link for Git](https://git-scm.com/downloads)

- Metamask: Cryptowallet for blockchain apps; a google chrome ONLY extension

[Here's link for Metamask](https://metamask.io/)

# Now that we have all of that situated, we can begin 

- Make a nice directory for smart contract that you know you'll remember, very imporant

- Now what ever directory you're in, you'll want to "Truffle init" 

This will create or "unbox" the migrations, contracts, test folders and truffle-config.js file in whichever directory you're in

# IMPORTANT for truffle-config.js file

- For lines 45-49, remove the comments as this will activate the file
- Line 47: this is the port in which the blockchain will be coming from;

either 7545 for using Ganache GUI or 8585 if using ganache client through command line prompt

# Next, new Migration file to deploy SmartContract
- Within 'migrations' folder, copy the 1st one and open it within any text editor, ideally Notepad++
- Once you opened it, create new file and copy content into new file for new .js file
- This should be new .js file : 

var Courses = artifacts.require("./Courses.sol");

module.exports = function(deployer) {
  deployer.deploy(Courses);

};

# Remember to have SmartContract within directory
Have Courses.sol within 'contracts' folder in order to compile

# You are ready to get the show on the road
- First you want to get into right directory: example mines: C:\Users\isaac\Documents\BlockChain\HW4
- Once here, you'll want to "Truffle Compile" in order to get the contracts going
- Next, you'll want to "Truffle Migrate" in order to deploy/compile the contracts so it can interact with the blockchain
- In case something happened, you can do "Truffle migrate --reset" in order to reset terminal you're working in

# What you should see if successful up to this point

![](Images/Blockchain README image.PNG)
