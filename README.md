# nervos-testnet
### Gitcoin: 0) Setup A Local CKB Node And CKB Indexer For The Testnet#

1. Setup a CKB Node:

![NODE](node.jpg)

2. Setup a CKB Indexer

![Indexer](indexer.jpg)

------------

### Gitcoin: 1) Create A Godwoken Account On The EVM Layer 2 Testnet

![Account](account.jpg)

https://explorer.nervos.org/aggron/address/ckt1qyqr0ue8xd08g4n9thyrrrkuvhrtjet29rwsvfpkl0


Deposit 
![Deposit](Deposit.jpg)

------------

### Gitcoin: 2) Deploy A Simple Ethereum Smart Contract On Polyjuice
![Deployed](Deployed.jpg)

Transaction hash: 0x31b39ef655191bc84a7f79c0804f84e5d97c8b19c35a8cf8832f48f857bd3f27

Deployed contract address: 0x16C024484E7531338ce849b8621c4F15C2436e3d

------------

### Gitcoin: 3) Issue A Smart Contract Call To The Deployed Smart Contract
![Call-contract](Call-contract.jpg)

 transactionHash: 0xac91cc38caf6e69f71513722db348c1ee3e93d0b84a8b66285b3b35af6fddadf
 contract address: 0x16C024484E7531338ce849b8621c4F15C2436e3d
 
 
ABI:
 
[
    {
      "inputs": [],
      "stateMutability": "payable",
      "type": "constructor"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "x",
          "type": "uint256"
        }
      ],
      "name": "set",
      "outputs": [],
      "stateMutability": "payable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "get",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    }
]

------------

### Gitcoin: 4) Issue An SUDT Token On Layer 1 And Deposit It To Layer 2

1-A link to the Layer 1 address you funded on the Testnet Explorer:
https://explorer.nervos.org/aggron/address/ckt1qyqr0ue8xd08g4n9thyrrrkuvhrtjet29rwsvfpkl0

2-A screenshot of the console output immediately after using sudt-cli to create your SUDT tokens on Layer 1:
![create-sudt](create-sudt.jpg)

3-A link to the transaction ID created by sudt-cli on the Testnet Explorer:
https://explorer.nervos.org/aggron/transaction/0x47f3ed4f907b7b3803d78ab534f53d2591d717f7169ef51a1bbf3e7f008f4bb7

4-A screenshot of the console output immediately after you have successfully submitted a deposit to Layer 2 using the account-cli tool:
![deposited-layer2](deposited-layer2.jpg)

5-The SUDT ID from the console output after executing the deposit script (in text format).

Your sudt id: 1581

------------
 
### Gitcoin: 5) Deploy The ERC20 Proxy Contract For The Deposited SUDT
![5-deployed-sc](5-deployed-sc.jpg)

Deployed SUDT-ERC20 Proxy contract address: 0x70E9C8cd289d78B874e5F4b8FfD95df37B3203Cb

![5-check-balance](5-check-balance.jpg)

Using Ethereum address: 0xe36ee8026c907667B916ee8059508787497B0eE2

------------

### Gitcoin: 6) Use Force Bridge To Deposit Tokens From Ethereum To Polyjuice
![6-deposited](6-deposited.jpg)

#### Deposit receiver address:
ckt1q3dz2p4mdrvp5ywu4kk5edl2uc4p03puvx07g7kgqdau3n3dmypkqnxzuefxyp9wdghglncj77k5wt6p59sx6kukyjlwh5s467qgp8m25yqqqqqsqqqqqvqqqqqfjqqqqpczty2pg0a5e9st9xz4rxx55ut7a23jaud5cda6xv2e06xfq3nm56gqqqqpqqqqqqcqqqqqxyqqqqx7asf60w8pqpte2sfcfn90fdfzxue7ff2g8sawe9wacnqat6jmygqngqqqqpxv9ejjvgz2u63w3l839aadguh5rgtqd4devf97a0fpt4uqsz0k4cmwaqpxeyrkv7u3dm5qt9gg0p6f0v8wyq9rqgqqqqqqcq5gr3fm

Ethereum address: 0xe36ee8026c907667B916ee8059508787497B0eE2

https://rinkeby.etherscan.io/tx/0x6d6d0a8ec0da36cb36e188c5dfb22bb8b636877f6dc94d86e5424ac4ad014b87

https://explorer.nervos.org/aggron/transaction/0x7dda98bbc4baab0e885457855261e5fa4fe31e7d4751d944e7423a2651a5ff34








