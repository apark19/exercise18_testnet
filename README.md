# exercise18_testnet

## dependencies 
- geth

## Procedure 
<p>1. To start the ethereum testnet nodes, navigate to the root directory of the repo.</br>
   2. Initiate the first node with the command: ./geth --datadir node1 --mine --minerthreads1 --rpc</br>
   --> Be sure to copy the enode address of the first node. This information can be found in the console output.</br>
   3. Initiate the second node with the command: ./geth --datadir node2 --port 30304 --bootnodes {node1_enode_address} --mine --minerthreads 1</br></p>
   
## CLI Options
<p>datadir --> This option denotes the directory that geth should look at when running.</br>
mine --> This option tells geth to enable mining on the network. </br>
minerthreads --> This option denotes how many processes should be initiated to mine. Allows for multiprocessing / concurrent mining for higher block yields, however, this incurs higher CPU demand.</br>
port --> This option denotes which port the miner should be connected to for communication with the Ethereum network.</br>
rpc --> This option denotes the enabling of remote procedure call for the node. This allows node2 and your mycrypto wallet to communicate with node.</br>
bootnodes --> This option denotes where the current node should connect to as the genesis node.</br></p>

## Configuration
<p>- Blocktime = default (15)</br>
- chainid = 123 </br>
- account1_pw = ageLess5534M</br>
- account2_pw = hurtZ78441!</br>
- node1_port = default (30303)</br>
- node2_port = 30304</br></p>

## Sending TXs
<p>1. Navigate to MyCrypto wallet.</br>
2. View & Send </br>
3. Keystore --> Browse for keystore file in node1/keystore </br>
4. Copy & Paste the public address of node2 into the destination address field.
5. Set the amount 
6. Send
