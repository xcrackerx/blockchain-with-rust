# Creating a Blockchain by Rust

## 60 Days of Code with Polkadot by Blockchained India
### Assignment - Week 2
### Submitted By : Mohd Ibrahim Mallick


## Steps to Run:

1. Fork the repository 
```
https://github.com/xcrackerx/blockchain-with-rust.git
```

2. Run the command :
```bash
RUST_LOG=info cargo run
```

- This starts the client locally. The blockchain is not persisted anywhere.

- You can start it in multiple terminals to get multiple connected peer-to-peer clients.

In each client, you can enter the following commands:

* `ls p` - list peers
* `ls c` - print local chain
* `create b $data` - `$data` is just a string here - this creates (mines) a new block with the data entry `$data` and broadcasts it

- Once a block is created by a node, it's broadcasted and the blockchain in all other nodes is updated (if it's a valid block).

- On startup, a node asks another node on the network for their blockchain and, if it's valid and longer than the current local blockchain, it updates it's own chain to the longest one it receives.

## Output

![Output](/output.png)