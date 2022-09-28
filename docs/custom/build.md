
## 命令记录
### cargo run
```
cargo run -p graph-node --release -- \
  --postgres-url postgresql://cryptodata:'euxC&z9WKz7i$u6p'@gz-postgres-03qsbn2n.sql.tencentcdb.com:27528/graph-node \
  --ethereum-rpc NETWORK_NAME:https://mainnet.infura.io \
  --ipfs 127.0.0.1:5001
```

## 问题记录

https://github.com/graphprotocol/graph-node/issues/2244
### 问题
```
ld: library not found for -lpq
```
### 解决
```
 brew install libpq 
 export PQ_LIB_DIR="$(brew --prefix libpq)/lib"
```

