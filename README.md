# Aura
Aura network

## Prerequisite
- Go 1.17+
- Starport 0.18.3
- Cosmos SDK 0.44.0

## Install Aura daemon
Using Makefile
```
    make
```
The **aurad** bin file is located on **$source_directory/bin/** 

## Setup a LocalNet

### Initialize the Chain
```
# <moniker> is the custom username of the node
# <chain-id> is the identity of the chain
aurad init <moniker> --chain-id <chain-id>
```
This command will initialize the home folder containing necessary components for your chain  
(default: ~/.aura)

### Customize the genesis file
A genesis file is a JSON file which defines the initial state of your blockchain. It can be seen as height 0 of your blockchain. The first block, at height 1, will reference the genesis file as its parent.

The docs about genesis customization: https://hub.cosmos.network/main/resources/genesis.html

### Run a node
```
aurad start 
```
## Setup testnet using testnetCmd