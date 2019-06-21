# Python Bitcoin blockbook Client

## Install and use

### Install
```
pip install bitcoin-client
```
### Examples

Init
```
BITCOIN_EXPLORER = ...
bitcoin_client = BitcoinClient(BITCOIN_CONF)
```

Get last height.
```
height = bitcoin_client.get_last_height()
```

Get block hash by block num.
```
hash = bitcoin_client.get_block_hash(height)
```

Get sender address.
```
address = bitcoin_client.get_sender_address(hash)
```

Get block info by hash per page
```
block = bitcoin_client.get_block(hash)
block = bitcoin_client.get_block(hash, 2)
```

Get tx info by tx hash.
```
tx = bitcoin_client.get_tx(hash)
```

