# CrossFi testnet Daily snapshots

#### Requrements: (lz4) 
`sudo apt-get install lz4`

___ 

## How to use? 


1. Download latest snapshot

```
wget https://cosmos-snapshots.web3cdn.services/crossfi/testnet/crossfi_daily.tar.lz4
```

2. Stop your indexer/node.
```
systemctl stop cosmovisor
```

3. Cleanup blockchain data
 ```
 rm -rf %YOUR_CROSSFI_FOLDER%/data/
 ```

4. Unpack archive
```
lz4 -c -d crossfi_daily.tar.lz4  | tar -x -C %YOUR_CROSSFI_FOLDER%
```
