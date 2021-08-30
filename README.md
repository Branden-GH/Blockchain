# Blockchain (Proof of Authority)
Here is a guide and instruction on a Proof of Authority new genesis block

# Step 1. Created new accounts for Node1 and Node2
  By creating both accounts this generated a keystore folder and geth folder with both the open access key and private key.  This allowed communication between the two to begin mining.
# Step 2. Genesis Creation
  Genesis instructions were followed I named my network blockchainexample and chose the Proof of Authority consesus algorithm.
  After the genesis block was created I initialized the nodes
 #  -code: ./geth --datadir node1 init blockchainexample.json
 #  -code: ./geth --datadir node2 init blockchainexample.json
![Node1 init](https://user-images.githubusercontent.com/81596605/131276395-ab2e7b41-f298-4f5b-9fd8-8982db2c907b.PNG)
