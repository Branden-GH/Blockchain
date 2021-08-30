# Genesis Block Creation (Proof of Authority)
Here is a guide and instruction on a Proof of Authority new genesis block:

## Created new accounts for Node1 and Node2
  By creating both accounts this generated a keystore folder and geth folder with both the open access key and private key.  This allowed communication between the two nodes.
  
## Genesis Creation

  Genesis instructions were followed I named my network blockchainexample and chose the Proof of Authority consesus algorithm.
  After the genesis block was created I initialized the nodes
  -code: ./geth --datadir node1 init blockchainexample.json
  
![Node1 init](https://user-images.githubusercontent.com/81596605/131276395-ab2e7b41-f298-4f5b-9fd8-8982db2c907b.PNG)

 -code: ./geth --datadir node2 init blockchainexample.json
 
![Node2 Init](https://user-images.githubusercontent.com/81596605/131276919-39353a03-d62b-4042-bd46-4c90d3057b1a.PNG)

## Running the nodes in separate terminals

 ./geth --datadir node1 --unlock "SEALER_ONE_ADDRESS" --mine --rpc --allow-insecure-unlock
 
![Node1 mine](https://user-images.githubusercontent.com/81596605/131277386-6d9c8217-cb92-4652-bf5e-20edbe0db097.PNG)

 ./geth --datadir node2 --unlock "SEALER_TWO_ADDRESS" --mine --port 30304 --bootnodes
 
![Node2 mine](https://user-images.githubusercontent.com/81596605/131277413-76b713e6-7cbf-4d16-a175-d139dea58848.PNG)

## Change the Network on MyCrypto to match the Network created during the Genesis Creation
  -Make sure network ID matches
  -ETH crypto is selected
  -Correct Port is entered: http://127.0.0.1:8545
## Your wallet should then have unimaginable wealth!
![proofoffunds](https://user-images.githubusercontent.com/81596605/131277653-37eddd08-29fd-48d9-9c6e-3ab165cbb180.PNG)
## Transaction between Node1 and Node2 with your new uploaded Ethereum
![Node2 transaction](https://user-images.githubusercontent.com/81596605/131277817-1b85d2a5-063e-4335-bf86-79a04509a9bc.PNG)
![proofofsend](https://user-images.githubusercontent.com/81596605/131277820-5a2d4765-0c50-4ebd-93ca-cf9c0696cd47.PNG)
## Checking TX status
![TxStatus](https://user-images.githubusercontent.com/81596605/131277887-4e9dab01-804e-4327-b55e-64e28e0c8ef5.PNG)


