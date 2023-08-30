# DriveCRDT Development Documentation

## Introduction
DriveCRDT is a project focused on constructing a Bitcoin-native internet scaling layer, integrating decentralized storage and compute-over-data capabilities with the Bitcoin network. By leveraging the unique properties of Conflict-free Replicated Data Types (CRDTs), the project seeks to ensure data consistency across a decentralized network. This documentation offers a comprehensive understanding of the project's components and their interplay.

## Table of Contents
- [Vision & Objective](#vision--objective)
- [Core Components & Technologies](#core-components--technologies)
- [Data & Compute Architecture](#data--compute-architecture)
- [User Experience & AI Enhancements](#user-experience--ai-enhancements)
- [Reference Links](#reference-links)

### Vision & Objective
Building a Bitcoin-native internet that integrates decentralized storage and comput-over-data capabilities, aiming to onboard billions of users and ensuring a decentralized, robust, and efficient digital ecosystem.

### Core Components & Technologies

#### Bitcoin Drivechain with CRDTs
- **Description:** CRDTs are data structures that allow multiple replicas to be updated independently and concurrently without coordination. Integrating CRDTs with Bitcoin's drivechain enables Bitcoin users to benefit from greater functionality, allowing for more cohesive industry adoption and use case exploration with expressive asset programmability. 
- **Reference:** [Learn more about CRDTs](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type)

#### AT2 Integration (Potential Route)
- **Description:** AT2 is an Asynchronous Trustworthy Transfers protocol that offers a decentralized approach to asset transfers without the need for global consensus. Its integration can provide enhanced security and efficiency in transactions. Possibilities for both permissioned and open networks.
- **Reference:** [Learn more about AT2](https://arxiv.org/abs/2002.07763)

#### Vegvisir (Potential Route)
- **Description:** Vegvisir is a CRDT-based distributed ledger technology that ensures data consistency in decentralized systems, even in the presence of network partitions. It offers a robust framework for building decentralized applications. Permissioned
- **Reference:** [Vegvisir: A Partition-Tolerant Blockchain for the Internet-of-Things](https://www.researchgate.net/publication/334448816_Vegvisir_A_Partition-Tolerant_Blockchain_for_the_Internet-of-Things)

#### Orderlesschain and IPLD Integration (Potential Route)
- **Description:** Orderlesschain is a decentralized ledger system designed to ensure data consistency and integrity. The potential integration with the InterPlanetary Linked Data (IPLD) can further enhance data interoperability. Given the project's early stages, there's a possibility to port Orderless components to Rust for enhanced interoperability. Permissioned
- **Reference:** [Orderlesschain](https://github.com/orderless-chain)
  - ##### Orderlessfile
    - **Description:** Orderlessfile is a decentralized storage module designed for efficient data storage and retrieval. It focuses on ensuring that data remains consistent, available, and partition-tolerant.
    - **Reference:** [Orderless: A Decentralized File System](https://arxiv.org/pdf/2210.01477.pdf)


### Data & Compute Architecture
#### IPVM, WNFS, IROH
- **Description:** These Rust-based modules collectively offer a comprehensive solution for decentralized computation, distributed file systems, and efficient data storage and retrieval.
- **References:** [IPVM Working Group](https://github.com/ipvm-wg), [WNFS Working Group](https://github.com/wnfs-wg/), [IROH](https://github.com/n0-computer/iroh)

#### UCANs
- **Description:** UCANs, or User-Controlled Authorization Networks, are a decentralized authorization protocol.
- **Reference:** [UCAN Working Group](https://github.com/ucan-wg)

#### TauByte & Bacalhau
- **Description:** Both are Go-native modules. TauByte focuses on efficient data processing, while Bacalhau emphasizes decentralized data integrity.
- **References:** [TauByte](https://github.com/taubyte), [Bacalhau Project](https://github.com/bacalhau-project)

### User Experience & AI Enhancements
#### NNS Integration
- **Description:** The Name Name System (NNS) simplifies transactions by allowing users to send payments to their claimed Decentralized Identifier (DID).
- **Reference:** [NNS Discussion](https://talk.fission.codes/t/nns-the-name-name-system/3684)

#### Petals AI
- **Description:** Petals AI is an advanced AI system that offers insights, predictions, and data-driven recommendations.
- **Reference:** [BigScience Workshop: Petals](https://github.com/bigscience-workshop/petals)

### Reference Links
In addition to the links provided throughout this overview, I have listed some considerable projects and inspiration below:
- [On the Future of Decentralized Computing](https://research.protocol.ai/publications/on-the-future-of-decentralized-computing/vukolic2021.pdf)
- [FabricCRDT: A CRDT Approach to Permissioned Blockchains](https://www.researchgate.net/publication/337455334_FabricCRDT_A_Conflict-Free_Replicated_Datatypes_Approach_to_Permissioned_Blockchains)
- [Merkle-CRDTs](https://research.protocol.ai/blog/2019/a-new-lab-for-resilient-networks-research/PL-TechRep-merkleCRDT-v0.1-Dec30.pdf) | [go-ds-crdt on GitHub](https://github.com/ipfs/go-ds-crdt)
- [Lilypad Network Whitepaper](https://docs.lilypadnetwork.org/research-and-vision/whitepaper)

### Additional References
- [rust-crdt on GitHub](https://github.com/rust-crdt/rust-crdt/tree/master)
- [bft-crdts on GitHub](https://github.com/davidrusu/bft-crdts)
- [maidsafe/brb on GitHub](https://github.com/maidsafe/brb/)
- [maidsafe/brb_dt_at2 on GitHub](https://github.com/maidsafe/brb_dt_at2)
- [hashseq on GitHub](https://github.com/davidrusu/hashseq/tree/master)
