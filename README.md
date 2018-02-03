# Block_Chain_Self_Study
on window
-----------------

## 1. Download Geth(version 1.7.3)

## 2. Running Geth on test network
### - Make genesis.json file
### - Initialize Geth
C:\Program Files\Geth>geth --datadir c:/data_testnet init c:/data_testnet/genesis.json
### - Run Geth
C:\Program Files\Geth>geth --networkid 4649 --nodiscover --maxpeers 0 --datadir c:/data_testnet console 2>> c:/data_testnet/geth.log
### Create new account
personal.newAccount("pass0")
※ pass0 == PassWord
### Start Mining
miner.start(1)
### Stop Mining
miner.stop
### Check Block Number
eth.blockNumber
### Check Balance
eth.getBalance(eth.accounts[0])
### Unlock Account before Send
personal.unlockAccount(eth.accounts[0],"pass0")
### Send Ether
eth.sendTransaction({from:eth.accounts[0], to:eth.accounts[1], value:web3.toWei(10,"ether")})
