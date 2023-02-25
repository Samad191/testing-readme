# About
The indexer is a tool that is used to extract events from a Geth node using an RPC method and store it in a CSV file. The data captured is based on a deposit contract on Ethereum.

# Built with
<a href="https://www.typescriptlang.org/" >
<img src="https://camo.githubusercontent.com/3f51c9e4df2ed06b09943fce5082aa1b87de388710df73a072ed260a1fbfcf36/68747470733a2f2f63646e2e776f726c64766563746f726c6f676f2e636f6d2f6c6f676f732f747970657363726970742e737667" width="35px" height="40px" > </img>
</a> 

# Setup
Clone the repo
```sh 
git clone https://github.com/abdulsamijay/Eth-deposit-indexer.git
```
Create build
```sh
npm run build
```


Create a .env file
```sh
API=""
RPC_ENDPOINT=""
MONGO_URI=""
```
Fetch events
```sh
node dsit/index.js --from <fromBlock> --to <toBlock> --fn events
```

<h4>P.S: Before using the following commands your path must be "node dist/index.js" </h4>
# Commands
* <b>--from <fromBlock> --to <toBlock> --fn events</b>    Fetches events from the specified block range
*  -V, --version                                          Output the version number
*  --fn, --fileName <optional fileName>                   File Name
*  --fnFrom, --fileNameFrom <optional fileName>           File Name From
*  --fnTo, --fileNameTo <optional fileName>               File Name To
*  --m, merge                                             Merge files
*  --help                                                 Display help for command
