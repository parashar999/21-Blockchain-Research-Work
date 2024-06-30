### Overview of ICP Features

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Protocol Basis**              | Threshold cryptography, state machine replication, novel consensus algorithm                                     |
| **Smart Contracts**             | Canisters                                                                                                       |
| **Performance & Scalability**   | Near-native performance, scalable execution                                                                     |
| **Compute & Storage**           | Capable of running heavy applications like image classification fully on-chain                                  |
| **Web Integration**             | Can host web assets, serve HTTP requests, interact with RPC nodes and Web2 servers                               |
| **Cross-Blockchain Interaction**| Can hold assets and make transactions on blockchains like Bitcoin and Ethereum using threshold signatures       |

### Subnets

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Definition**                  | Shards of the blockchain; each runs decentralized nodes and its own consensus algorithm                          |
| **Message Flow**                | Asynchronous, processed through boundary nodes to target subnets                                                 |
| **Cost & Security**             | Varies with subnet size                                                                                          |

### Threshold Signatures

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Security Mechanism**          | Private key split into secret shares among nodes                                                                |
| **Validation**                  | Efficient state and result validation through digital signatures                                                 |
| **Cross-Blockchain**            | Smart contracts can sign transactions for other blockchains like Bitcoin and Ethereum                            |

### Smart Contracts (Canisters)

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Execution Environment**       | WebAssembly, supporting JS, TypeScript, Rust, Python, Motoko                                                    |
| **Web Integration**             | Can serve web assets, handle HTTP requests                                                                      |
| **Storage**                     | WebAssembly memory (cleared on upgrade), stable memory (preserved on upgrade)                                    |

### Accounts and Keys

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Address Derivation**          | Derived from public key, referred to as principals                                                              |
| **Private Key Services**        | Smart contracts can securely store private keys for user accounts                                               |

### Tokens

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Implementation**              | By smart contracts, ICRC-2 standard for fungible tokens                                                         |

### Messages

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Programming Model**           | Actor model, asynchronous message passing                                                                       |

### Cycles

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Cost Model**                  | Canisters pay for resource usage by burning cycles, fixed price                                                 |

### Governance

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Governance Model**            | Decentralized autonomous organization (DAO) called Network Nervous System (NNS)                                  |
| **Voting**                      | Community votes on proposals, ensures protocol uniformity                                                       |

### Nodes

| Feature                         | Details                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **Standards**                   | High hardware standards (64 CPU cores, 512 GiB RAM, 30 TB NVMe SSD)                                              |
| **Provider Vetting**            | Requires DAO voting, ensures reliability and decentralization                                                    |

### Comparison with Ethereum

| Feature                              | Ethereum                                | ICP                                           |
|--------------------------------------|-----------------------------------------|-----------------------------------------------|
| **Virtual Machine**                  | EVM                                     | WebAssembly                                   |
| **On-chain Web3**                    | -                                       | Yes                                           |
| **Bridgeless Bitcoin**               | -                                       | Yes                                           |
| **Smart contracts can sign messages**| -                                       | Yes                                           |
| **HTTP calls to Web2 from smart contracts**| -                                | Yes                                           |
| **Languages**                        | Solidity, Vyper, Yul                    | JS, Python, Rust, Solidity, Motoko, and more  |
| **Programming model**                | Atomic transactions                     | Async message passing                         |
| **Upgradability**                    | Immutable                               | Upgradable or immutable                       |
| **Gas model**                        | User pays                               | Smart contract pays                           |
| **Gas price**                        | Variable                                | Fixed                                         |
| **Compute**                          | Few million instructions/block          | 2 billion instructions/block (per subnet)     |
| **Finality**                         | ~15 min                                 | ~1.4 s                                        |
| **Average tx/msg fee**               | ~$1                                     | ~$0.000001                                    |
| **Stack size**                       | 32 KB (1024 of 256-bit values)          | 5 MB                                          |
| **Code size**                        | 24 KB (more with code sharing)          | 10 MB                                         |
| **Memory size**                      | Few KB                                  | 404 GiB (4 GiB Wasm memory + 400 GiB stable memory) |
| **Storage cost**                     | $18M per GiB (based on 640K gas per KB) | $5 per GiB per year                           |
| **Number of nodes**                  | ~7K                                     | ~500 in total, 13-40 per subnet               |
