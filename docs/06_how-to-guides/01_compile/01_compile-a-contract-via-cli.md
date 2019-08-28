## How to compile a contract via CLI

Prerequisites:
---
You have the source of your contrat saved in one of your local folders, e.g. `./examples/hello`
For details on how to create your first contract follow [this tutorial here](https://developers.eos.io/eosio-home/docs/your-first-contract)

Follow these steps to compile your contract
---

1. Navigate to the hello folder in examples (./examples/hello)
2. You should then see the hello.cpp file
3. Now run the compiler
```
$ eosio-cpp -abigen hello.cpp -o hello.wasm
```
4. Or with CMake
```
$ mkdir build
$ cd build
$ cmake ..
$ make
```
This will generate two files:
- The compiled binary wasm (hello.wasm)
- The generated ABI file (hello.abi)