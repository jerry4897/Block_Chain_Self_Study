# Block_Chain_Self_Study
on window
-----------------

## 1. Download Geth

## 2. Running Geth on test network
### - Make genesis.json file
### - Initialize Geth
C:\Program Files\Geth>geth --datadir c:/data_testnet init c:/data_testnet/genesis.json
### - Run Geth
C:\Program Files\Geth>geth --networkid 4649 --nodiscover --maxpeers 0 --datadir c:/data_testnet console 2>> c:/data_testnet/geth.log
