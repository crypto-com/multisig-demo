# Proof of Goods and Services: demo use case using threshold multi-signatures
## Warning: 
This project is under heavy development and for demo purpose only, please don't use it on mainnet. 

## Task lists: 
- [X] Merchant panel
- [ ] Escrow panel


## Build

### Build Prerequisites
- Crypto.com Chain - sample-chain-wallet: https://github.com/crypto-com/sample-chain-wallet/tree/multi-sig-demo
  <br> (To enable multi-sig feature, please change branch to `multi-sig-demo` on sample-chain-wallet)
### Build instructions
- #### Multi-sig web backend
```bash
$ cd backend
$ cargo install diesel_cli --no-default-features --features sqlite
$ diesel setup
$ cargo run
```
if ubuntu : sudo apt-get install libsqlite3-dev <br>
if fedora : sudo dnf install libsqlite3x-devel

- #### Multi-sig web frontend
```bash
$ cd frontend
$ npm install
$ ng serve --port 4201
```
Navigate to http://localhost:4201/.
## License

[Apache 2.0](./LICENSE)