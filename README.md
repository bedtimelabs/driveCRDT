# driveCRDT
driveCRDT is a proposed BIP300 Drivechain utilizing Conflict-Free Repilicated Data Type smart contracts


## DriveCRDT: A Comprehensive Technical Overview

### Abstract

DriveCRDT is an ambitious project designed to integrate Bitcoin payments directly into the IPLD decentralized internet using the principles of BIP300 and BIP301 drivechains. Instead of leveraging the RSK sidechain, DriveCRDT employs the capabilities of Orderlesschain. However, a significant shift involves rewriting Orderlesschain from Go to Rust, aiming for seamless integration with other Rust-based components like IPVM. The project aspires to combine the security and immutability of the Bitcoin blockchain with the flexibility and scalability of the IPLD, all while ensuring compatibility with existing and future IPLD-based systems.

### Core Components

#### Bitcoin Drivechain

Drivechains, as proposed in BIP300 and BIP301, allow Bitcoin to be temporarily offloaded to alternative, non-native blockchains called "sidechains". DriveCRDT uses this mechanism to offload Bitcoin to the Orderlesschain, which is integrated with the IPLD.

#### Orderlesschain Integration with IPLD

The original Orderlesschain, written in Go, is being transitioned to Rust to ensure compatibility with other components like IPVM. This Rust-based Orderlesschain will be built directly into the IPLD, benefiting from the decentralized data structure's inherent scalability and flexibility.

#### CRDTs in DriveCRDT

Conflict-free Replicated Data Types (CRDTs) are data structures that allow multiple replicas to be updated independently. In DriveCRDT, these CRDTs will manage state in the Orderlesschain, ensuring consistency without a global transaction order.

### Additional Integrations

#### WebNative File System (WNFS)

DriveCRDT may also integrate WNFS, a decentralized file system that allows users to control their data and share it across applications and devices. It uses IPFS for data storage and IPLD for data structuring.

#### InterPlanetary Virtual Machine (IPVM)

With IPVM written in Rust, its integration with DriveCRDT becomes more feasible. IPVM allows for the execution of WebAssembly (Wasm) code in a distributed manner, using IPLD for data structuring.

#### Name Name System (NNS)

NNS, a decentralized naming system, could be integrated to provide intuitive naming conventions and address resolutions, enhancing user experience.

### Development and Future Plans

The initial phase involves rewriting Orderlesschain in Rust. This transition not only ensures compatibility with IPVM but also sets the stage for future integrations. Once the Rust-based Orderlesschain is stable, the team will explore integrating other components like WNFS, IPVM, and NNS. The ultimate goal is to create a robust, scalable, and user-friendly platform that brings Bitcoin's security to the decentralized web.

### Conclusion

DriveCRDT, with its innovative approach and commitment to leveraging the best of both Bitcoin and the IPLD, stands as a testament to the future of decentralized applications and services. By rewriting core components in Rust and planning for extensive integrations, DriveCRDT is poised to be a significant player in the decentralized web landscape. Like its sibling, IPsatoshi, DriveCRDT welcomes contributions and collaborations to realize its vision.
