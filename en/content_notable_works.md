# SCRF: Notable Works

We have open bounties available for anyone who can suggest additions, deletions, corrections or updates to this page. Please see [forum](https://www.smartcontractresearch.org/t/bounty-call-for-notable-works-key-scholarship/73) for details.

## Table of Contents

- [Auditing and Security](#auditing-and-security)
  - [The Security Reference Architecture for Blockchains\: Towards a Standardized Model for Studying Vulnerabilities, Threats, and Defenses](#the-security-reference-architecture-for-blockchains-towards-a-standardized-model-for-studying-vulnerabilities-threats-and-defenses)
  - [A Survey on Ethereum Systems Security\: Vulnerabilities, Attacks, and Defenses](#a-survey-on-ethereum-systems-security-vulnerabilities-attacks-and-defenses)
  - [A Survey on the Security of Blockchain Systems](#a-survey-on-the-security-of-blockchain-systems)
  - [246 Findings From our Smart Contract Audits\: An Executive Summary](#246-findings-from-our-smart-contract-audits-an-executive-summary)
  - [Ethereum Smart Contract Security Best Practices](#ethereum-smart-contract-security-best-practices)
  - [List of Ethereum Smart Contracts Post-Mortems](#list-of-ethereum-smart-contracts-post-mortems)
  - [EEA EthTrust Security Levels Specfication v1](#eee-ethtrust-security-levels-specification)
- [Oracles and Data](#oracles-and-data)
  - [The Blockchain as a Software Connector](#the-blockchain-as-a-software-connector)
  - [Town Crier: An Authenticated Data Feed for Smart Contracts](#town-crier-an-authenticated-data-feed-for-smart-contracts)
  - [ChainLink: A Decentralized Oracle Network](#chainlink-a-decentralized-oracle-network)
  - [ASTRAEA\: A Decentralized Blockchain Oracle](#astraea-a-decentralized-blockchain-oracle)
  - [Augur\: A Decentralized Oracle and Prediction Market Platform](#augur-a-decentralized-oracle-and-prediction-market-platform)
  - [From Oracles to Trustworthy Data On-chaining Systems](#from-oracles-to-trustworthy-data-on-chaining-systems)
  - [Shintaku\: An End-to-End-Decentralized General-Purpose Blockchain Oracle System](#shintaku-an-end-to-end-decentralized-general-purpose-blockchain-oracle-system)
- [Tooling and Languages](#tooling-and-languages)
  - [Vyper\: A security comparison with solidity based on common vulnerabilities](#vyper-a-security-comparison-with-solidity-based-on-common-vulnerabilities)
  - [Safer smart contract programming with Scilla](#safer-smart-contract-programming-with-scilla)
  - [A Survey of Tools for Analyzing Ethereum Smart Contracts](#a-survey-of-tools-for-analyzing-ethereum-smart-contracts)
  - [Slither\: A Static Analysis Framework For Smart Contracts](#slither-a-static-analysis-framework-for-smart-contracts)
  - [Smashing Ethereum Smart Contracts for Fun and Real Profit](#smashing-ethereum-smart-contracts-for-fun-and-real-profit)
  - [KEVM\: A Complete Semantics of the Ethereum Virtual Machine](#kevm-a-complete-semantics-of-the-ethereum-virtual-machine)
- [Mechanism Design](#mechanism-design)
  - [Mechanism Design Theory](#mechanism-design-theory)
  - [Mechanism Theory](#mechanism-theory)
  - [Market Structure in Bitcoin Mining](#market-structure-in-bitcoin-mining)
  - [Credible Neutrality as a Guiding Principle](#credible-neutrality-as-a-guiding-principle)
  - [Combinatorial Information Market Design](#combinatorial-information-market-design)
- [Privacy](#privacy)
  - [When the cookie meets the blockchain\: Privacy risks of web payments via cryptocurrencies](#when-the-cookie-meets-the-blockchain-privacy-risks-of-web-payments-via-cryptocurrencies)
  - [PERIMETER: A network-layer attack on the anonymity of cryptocurrencies](#perimeter-a-network-layer-attack-on-the-anonymity-of-cryptocurrencies)
  - [Tor\: The Second Generation Onion Router](#tor-the-second-generation-onion-router)
  - [Untraceable electronic mail, return addresses, and digital pseudonyms](#untraceable-electronic-mail-return-addresses-and-digital-pseudonyms)
  - [Zerocash\: Decentralized Anonymous Payments from Bitcoin](#zerocash-decentralized-anonymous-payments-from-bitcoin)
  - [The Double Ratchet Algorithm](#the-double-ratchet-algorithm)
- [Governance and Coordination](#governance-and-coordination)
  - [Quadratic Voting\: How Mechanism Design Can Radicalize Democracy](#quadratic-voting-how-mechanism-design-can-radicalize-democracy)
  - [An Economic Theory of Political Action in a Democracy](#an-economic-theory-of-political-action-in-a-democracy)
  - [Liquid Democracy\: An Algorithmic Perspective](#liquid-democracy-an-algorithmic-perspective)
  - [Decentralized Network Governance\: Blockchain Technology and the Future of Regulation](#decentralized-network-governance-blockchain-technology-and-the-future-of-regulation)
- [Scaling](#scaling)
- [Cryptography](#cryptography)
  - [A Graduate Course in Applied Cryptography](#a-graduate-course-in-applied-cryptography)
  - [Method of providing digital signatures (Merkle trees)](#method-of-providing-digital-signatures-merkle-trees)
  - [Merkling in Ethereum](#merkling-in-ethereum)
  - [Verkle Trees](#verkle-trees)
  - [Verkle trees (Blog post)](#verkle-trees-blog-post)
  - [MiMC: Efficient Encryption and Cryptographic Hashing with Minimal Multiplicative Complexity [AGRRT16]](#mimc-efficient-encryption-and-cryptographic-hashing-with-minimal-multiplicative-complexity-agrrt16)
  - [Baby Jubjub Elliptic Curve](#baby-jubjub-elliptic-curve)
  - [Pedersen Hash [HBHW19]](#pedersen-hash-hbhw19)
  - [POSEIDON: A New Hash Function for Zero-Knowledge Proof Systems [GKRRS19]](#poseidon-a-new-hash-function-for-zero-knowledge-proof-systems-gkrrs19)
  - [How To Simulate It – A Tutorial on the Simulation Proof Technique](#how-to-simulate-it--a-tutorial-on-the-simulation-proof-technique)
  - [Roll_up](#roll_up)
  - [Succinct Non-Interactive Zero Knowledge for a von Neumann Architecture (zk-SNARKs) [BCTV14b]](#succinct-non-interactive-zero-knowledge-for-a-von-neumann-architecture-zk-snarks-bctv14b)
  - [On the Size of Pairing-based Non-interactive Arguments [GROTH16]](#on-the-size-of-pairing-based-non-interactive-arguments-groth16)
  - [Bulletproofs: Short Proofs for Confidential Transactions and More [BBBPWM18]](#bulletproofs-short-proofs-for-confidential-transactions-and-more-bbbpwm18)
  - [Sonic: Zero-Knowledge SNARKs from Linear-Size Universal and Updatable Structured Reference Strings [MBKM19]](#sonic-zero-knowledge-snarks-from-linear-size-universal-and-updatable-structured-reference-strings-mbkm19)
  - [PlonK: Permutations over Lagrange-bases for Oecumenical Noninteractive arguments of Knowledge [GWC19]](#plonk-permutations-over-lagrange-bases-for-oecumenical-noninteractive-arguments-of-knowledge-gwc19)
  - [Scalable, transparent, and post-quantum secure computational integrity (zk-STARKs) [BBHR18]](#scalable-transparent-and-post-quantum-secure-computational-integrity-zk-starks-bbhr18)
  - [Secure Multiparty Computation (MPC)](#secure-multiparty-computation-mpc)
- [Consensus](#consensus)

## Auditing and Security

### The Security Reference Architecture for Blockchains\: Towards a Standardized Model for Studying Vulnerabilities, Threats, and Defenses

- **Source:** <https://arxiv.org/abs/1910.09775>
- **Authors:** Ivan Homoliak, Sarad Venugopalan, Daniël Reijsbergen, Qingze Hum, Richard Schumi, Pawel Szalachowski
- **Description:** This paper proposes a 4-layer security reference architecture for blockchains and identifies known threats, countermeasures, and dependencies at each layer
- **Relevance:** This paper is relevant because it is one of the first contributing towards the standardization of security threat analysis in the blockchain space
- **Citation:** I. Homoliak, S. Venugopalan, D. Reijsbergen, Q. Hum, R. Schumi and P. Szalachowski, "The Security Reference Architecture for Blockchains: Toward a Standardized Model for Studying Vulnerabilities, Threats, and Defenses," in IEEE Communications Surveys & Tutorials, vol. 23, no. 1, pp. 341-390, Firstquarter 2021, doi: 10.1109/COMST.2020.3033665.

### A Survey on Ethereum Systems Security\: Vulnerabilities, Attacks, and Defenses

- **Source:** <https://arxiv.org/abs/1908.04507>
- **Authors:** Huashan Chen, Marcus Pendleton, Laurent Njilla, Shouhuai Xu
- **Description:** This paper provides a holistic survey of Ethereum security, stratifying vulnerabilities, attacks, and defenses
- **Relevance:** This paper is relevant because it is one of the first to investigate the security issues across different layers of the Ethereum architecture

### A Survey on the Security of Blockchain Systems

- **Source:** <https://arxiv.org/abs/1802.06993>
- **Authors:** Xiaoqi Li, Peng Jiang, Ting Chen, Xiapu Luo, Qiaoyan Wen
- **Description:** This paper performs a high-level review of blockchain security as a whole.
- **Relevance:** This paper is relevant because it covers attacks in a wide time range (2009 to 2017)

### 246 Findings From our Smart Contract Audits\: An Executive Summary

- **Source:** <https://blog.trailofbits.com/2019/08/08/246-findings-from-our-smart-contract-audits-an-executive-summary/>
- **Authors:**
- **Description:** This blog post from Trail of Bits shares aggregate data of the findings in their audits
- **Relevance:** This post is relevant because it provides researchers with real-world data from audits performed by an industry player

### Ethereum Smart Contract Security Best Practices

- **Source:** <https://consensys.github.io/smart-contract-best-practices/>
- **Authors:** Consensys
- **Description:** This post provides key security considerations when developing Ethereum smart contracts
- **Relevance:** This post is relevant because it is a state-of-the-art catalog, providing a reference point for educating developers and auditors

### List of Ethereum Smart Contracts Post-Mortems

- **Source:** <https://forum.openzeppelin.com/t/list-of-ethereum-smart-contracts-post-mortems/1191>
- **Authors:** OpenZeppelin
- **Description:** This post outlines a list of Ethereum smart contracts post-mortems
- **Relevance:** This post is relevant because it provides lessons from real-world case studies. It is a state-of-the-art list that serves as a reference point for educating developers and auditors

### EEA EthTrust Security Levels Specification

- **Source:** <https://entethalliance.org/specs/ethtrust-sl/>
- **Authors:** Enterprise Ethereum Alliance (EthTrust Security Levels Working Group)
- **Description:** An industry-developed set of requirements for (Solidity) smart contract audits, to provide a basis for ensuring that audits meet a reasonable level of quality  in identifying potential vulnerabilities (three levels, from automatable tests to a full audit of code, business logic and documentation).
- **Relevance:** This specification was developed and is maintained by a stnadardisation group with active participation from multiple security audit firms alongside other stakeholders with relevant expertise.

## Oracles and Data

### The Blockchain as a Software Connector

- **Source:** <http://www.pautasso.info/biblio-pdf/blockchain-wicsa2016.pdf>
- **Authors:** Xiwei Xu, Cesare Pautasso, Liming Zhu, Vincent Gramoli, Alexander Ponomarev, An Binh Tran, and Shiping Chen
- **Description:** This paper describes the blockchain as an intermediation layer between applications, and introduces the concept of the  _validation oracle_, which bridges external data into the siloed blockchain.
- **Relevance:** Introduced a number of usecases in which oracles are now actively used, or are being developed towards.
- **Citation:** X. Xu et al., "The Blockchain as a Software Connector," 2016 13th Working IEEE/IFIP Conference on Software Architecture (WICSA), 2016, pp. 182-191, doi: 10.1109/WICSA.2016.21.

### Town Crier: An Authenticated Data Feed for Smart Contracts

- **Source:** <https://eprint.iacr.org/2016/168.pdf>
- **Authors:** Fan Zhang, Ethan Cecchetti, Kyle Croman, Ari Juels, Elaine Shi
- **Description:** This paper introduces a trusted hardware backed oracle solution that allows for secure delivery of confidential information to Ethereum smart contracts.
- **Relevance:** This application provides a mechanism for the execution of smart contracts on a public blockchain while preserving the end to end integrity of confidential data.

### ChainLink: A Decentralized Oracle Network

- **Source:** <https://link.smartcontract.com/whitepaper>
- **Authors:** Steve Ellis, Ari Juels, and Sergey Nazarov
- **Description:** This paper introduces a framework for decentralized oracle networks, a reputation model using on-chain data, and describes the modular features necessary to generalize this framework for a broad variety of usecases.
- **Relevance:** The authors identify decentralization at the data source and individual oracle level, and propose use cases such as off-chain computation.

### ASTRAEA\: A Decentralized Blockchain Oracle

- **Source:** <https://arxiv.org/abs/1808.00528>
- **Authors:** John Adler, Ryan Berryhill, Andreas Veneris, Zissis Poulos, Neil Veira, and Anastasia Kastania
- **Description:** Proposes a trustless, permissionless, and decentralized blockchain oracle based on voters and certifiers playing a game to certify truth value.
- **Relevance:** The mechanism of this oracle was built with incentive alignment in mind for the actors within the system, and the authors conclude that all rational actors within the system behave honestly.

### Augur\: A Decentralized Oracle and Prediction Market Platform

- **Source:** <https://github.com/AugurProject/whitepaper/blob/master/v1/english/whitepaper.pdf>
- **Authors:** Jack Peterson, Joseph Krug, Micah Zoltu, Austin K. Williams, and Stephanie Alexander
- **Description:** The team introduces a mechanism for predicting outcomes, staking on either side of the prediction, and ultimately resolving the true outcome.
- **Relevance:** While the long tail oracle method introduced in this paper hasn’t seen significant adoption for execution of smart contracts, the assessments around incentives and risks provide valuable insights.

### From Oracles to Trustworthy Data On-chaining Systems

- **Source:** <https://www.redaktion.tu-berlin.de/fileadmin/fg308/publications/2019/Heiss-et-al-oracles_preprint.pdf>
- **Authors:** Jonathan Heiss, Jacob Eberhardt, and Stefan Tai
- **Description:** The authors introduced Trustworthy Data On-chaining, a novel holistic perspective on reliable data provisioning for smart contracts that allows for evaluating existing Oracle.
- **Relevance:** The authors identify truthfulness as a fundamentally new requirement, which means that no execution of blockchain state transition is caused by untruthful data provisioning, but instead data is always provisioned in a well-intended way.

### Shintaku\: An End-to-End-Decentralized General-Purpose Blockchain Oracle System

- **Source:** <https://gitlab.com/shintaku-group/paper/raw/master/shintaku.pdf>
- **Authors:** Ryuuji Kamiya
- **Description:** This work defines the concept of end-to-end decentralization and presents a system architecture for implementing an oracle under such constraints
- **Relevance:** This work extends the original Astraea oracle design and attempts to reduce its complexity to more rigorously handle the special case of the verifier’s dilemma.

## Tooling and Languages

### Vyper\: A security comparison with solidity based on common vulnerabilities

- **Source:** <https://arxiv.org/abs/2003.07435v4>
- **Authors:** Mudabbir Kaleem, Anastasia Mavridou, Aron Laszka
- **Description:** This paper provides a qualitative analysis of Vyper from a standpoint of common vulnerabilities found in Solidity smart contracts
- **Relevance:** This paper is relevant because it points the issues that Vyper solves in comparison to Solidity and which ones remain unsolved.

### Safer smart contract programming with Scilla

- **Source:** <https://dl.acm.org/doi/pdf/10.1145/3360611> ([presentation also available](https://www.youtube.com/watch?v=adfNZVRJmHU))
- **Authors:** Lya Sergey, Vaivaswatha Nagaraj, Jacob Johannsen, Amrit Kumar, Anton Trunov, and Ken Chan Guan Hao
- **Description:** This paper presents and evaluates Scilla, a industrial graded smart contract programming language with built-in security mechanisms
- **Relevance:** This paper is relevant because it shows how Scilla is safe by design, as well as a framework for light-weight verification of Scilla programs. Official page: <https://scilla-lang.org/>.

### A Survey of Tools for Analyzing Ethereum Smart Contracts

- **Source:** <https://arxiv.org/abs/2105.06974v1>
- **Authors:** Monika Di Angelo, G. Salzer
- **Description:** This paper catalogs different analysis tools currently available (at the time of writing), making a qualitatively comparison between them
- **Relevance:** This paper is relevant because it gives a list of useful tools that developers could experiment with, as well as a starting point for researchers grasping the current state of the art.

### Slither\: A Static Analysis Framework For Smart Contracts

- **Source:** <https://arxiv.org/pdf/1908.09878.pdf>
- **Authors:** Josselin Feist, Gustavo Grieco, Alex Groce
- **Description:** This paper describes Slither, a static analysis tool for Solidity contracts.
- **Relevance:** This paper is relevant since Slither is a widely used tool supporting automatic identification of certain classes of vulnerabilities, refactoring opportunities, and general optimizations.

### Smashing Ethereum Smart Contracts for Fun and Real Profit

- **Source:** <https://github.com/b-mueller/smashing-smart-contracts>
- **Authors:** Bernhard Mueller
- **Description:** This paper describes describes Mythril, a static analysis tool for Solidity contracts and EVM bytecode
- **Relevance:** This paper is relevant because Mythril is a widely used tool supporting automatic identification of certain classes of vulnerabilities. Github page: <https://github.com/ConsenSys/mythril>

### KEVM\: A Complete Semantics of the Ethereum Virtual Machine

- **Source:** <https://ieeexplore.ieee.org/document/8429306>
- **Authors:** Everett Hildenbrandt and Manasvi Saxena and Xiaoran Zhu and Nishant Rodrigues and Philip Daian and Dwight Guth and Brandon Moore and Yi Zhang and Daejun Park and Andrei Stefanescu and Grigore Rosu
- **Description:** This paper describes an executable formal specification of the Ethereum Virtual Machine using the K framework
- **Relevance:** This paper is relevant because the KEVM spec can be extended to prove smart contracts correctness

## Mechanism Design

### Mechanism Design Theory

- **Source:** <https://www.nobelprize.org/uploads/2018/06/advanced-economicsciences2007.pdf>
- **Authors:** Prize Committee of the Royal Swedish Academy of Sciences
- **Description:** In 2007 Leonid Hurwicz, Eric Maskin, and Roger Myson were jointly awarded the Nobel Prize in Economic Sciences for their advancement of mechanism design theory.
- **Relevance:** This paper delves into their works and discusses applications of the theories presented. It is a good foundation to gather other literature from regarding the evolution of mechanism design.

### Mechanism Theory

- **Source:** <https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2542983>
- **Authors:** Matthew O. Jackson
- **Description:** Different applications of mechanism design are presented, primarily using Dominant Strategy and Bayesian mechanism designs.
- **Relevance:** Provides a mathematical basis and proofs for different types of mechanisms.

### Market Structure in Bitcoin Mining

- **Source:** <https://www.nber.org/system/files/working_papers/w24242/w24242.pdf>
- **Authors:** June Ma, Joshua S. Gans, Rabee Tourky
- **Description:** Analyzes the Proof-of-Work mechanism design, showing it formally maps onto dynamic game models.
- **Relevance:** Provides a technical foundation for economic analysis of PoW protocols.

### Credible Neutrality as a Guiding Principle

- **Source:** [Credible Neutrality As A Guiding Principle 1](https://nakamoto.com/credible-neutrality/)
- **Authors:** Vitalik Buterin
- **Description:** Defines the concept of credible neutrality for a protocol.
- **Relevance:** Provides an important framework for mechanism designers to qualitatively evaluate their protocols. Spawned other such principles such as governance minimization.

### Combinatorial Information Market Design

- **Source:** <https://link.springer.com/article/10.1023/A:1022058209073>
- **Authors:** Robin Hanson
- **Description:** Introduces the Logarithmic Market Scoring Rule (LMSR)
- **Relevance:** LMSR provides a foundation for other market valuation models such as the "constant product automated market maker" utilized by Uniswap.

## Privacy

### When the cookie meets the blockchain\: Privacy risks of web payments via cryptocurrencies

- **Source:** <https://arxiv.org/abs/1708.04748>
- **Authors:** Steven Goldfeder, Harry Kalodner, Dillon Reisman, and Arvind Narayanan
- **Description:** This paper proposes a 4-layer security reference architecture (SRA) for blockchains and identifies known threats, countermeasures, and dependencies at each layer.
- **Relevance:** This paper would be relevant for understanding how user behaviors with merchants can potentially impact the security of a blockchain via cookies deployed in cryptocurrency merchant APIs.

### PERIMETER: A network-layer attack on the anonymity of cryptocurrencies

- **Source:** <https://scholar.google.com/citations?view_op=view_citation&hl=fr&user=fVgBFrUAAAAJ&citation_for_view=fVgBFrUAAAAJ:8k81kl-MbHgC>
- **Authors:** Maria Apostolaki, Cedric Maire, Laurent Vanbever
- **Description:** This paper presents a stealthier and harder-to-mitigate attack exploiting the interactions between the networking and application layers.
- **Relevance:** It builds on a line of work on network-level attacks on anonymity, including “Hijacking Bitcoin” and “Bitcoin over Tor is not a good idea”.

### Tor\: The Second Generation Onion Router

- **Source:** <https://www.nrl.navy.mil/itd/chacs/sites/www.nrl.navy.mil.itd.chacs/files/pdfs/Dingledine%20etal2004.pdf>
- **Authors:** Roger Dingledine, Nick Mathewson, and Paul Syverson
- **Description:** This paper revisits onion routing in the original Tor network and proposes overcoming limitations in the original design by adding perfect forward secrecy, congestion control, directory servers, integrity checking, configurable exit policies, and a practical design for location-hidden services via rendezvous points.
- **Relevance:** Tor is the largest and longest running publicly available network for private routing and communication.

### Untraceable electronic mail, return addresses, and digital pseudonyms

- **Source:** <https://dl.acm.org/doi/10.1145/358549.358563>
- **Authors:** David L. Chaum
- **Description:** One of the first attempts to solve the "traffic analysis problem" (keeping confidential who converses with whom and when).
- **Relevance:** Introduces the concept of a Mix-Net which is foundational concept often revisited in privacy design.

### Zerocash\: Decentralized Anonymous Payments from Bitcoin

- **Source:** <https://ieeexplore.ieee.org/abstract/document/6956581>
- **Authors:** Eli Ben-Sasson , Alessandro Chiesa , Christina Garman, Matthew Green, Ian Miers, Eran Tromer, and Madars Virza
- **Description:** Shows how Bitcoin can be extended to provide strong anonymity guarantees using zero-knowledge proofs.
- **Relevance:** Introduces using zero-knowledge proofs with blockchains and laid the foundation for z-cash and other zero-knowledge based blockchain constructions.

### The Double Ratchet Algorithm

- **Source:** <https://signal.org/docs/specifications/doubleratchet/doubleratchet.pdf>
- **Authors:** Trevor Perrin and Moxie Marlinspike
- **Description:** The Double Ratchet algorithm is used by two parties to exchange encrypted messages where the parties derive new keys from every double message, ensuring that interception of keys for a given double message will not enable decoding an entire chain of messages.
- **Relevance:** Used in privacy focused messengers including Signal, Matrix and Status.

## Governance and Coordination

### Quadratic Voting\: How Mechanism Design Can Radicalize Democracy

- **Source:** <https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2003531>
- **Authors:** Steven Lalley and E. Glen Weyl
- **Description:** Individuals pay for as many votes as they wish using a number of "voice credits" quadratic in the votes they buy.
- **Relevance:** A canonical work that has inspired much discussion and design in emerging crypto protocol design.

### An Economic Theory of Political Action in a Democracy

- **Source:** <http://www.jstor.org/stable/1827369>
- **Authors:** Anthony Downs
- **Description:** Introduces the modern rational voter theory
- **Relevance:** Creates a framework for understanding the utility value of voting

### Liquid Democracy\: An Algorithmic Perspective

- **Source:** <https://par.nsf.gov/servlets/purl/10063518>
- **Authors:** Anson Kahng, Simon Mackenzie, and Ariel D. Procaccia
- **Description:** A study on liquid democracy to determine if it leads to better decision making than direct voting.
- **Relevance:** Liquid democracy is an active area of exploration in crypto networks.

### Decentralized Network Governance\: Blockchain Technology and the Future of Regulation

- **Source:** <https://www.rug.nl/research/portal/files/120767599/fbloc_03_00012.pdf>
- **Authors:** Andrej Zwitter and Jilles Hazenberg
- **Description:** The role that blockchain technology can play in what we term _decentralized network governance._
- **Relevance:** A new mode of governance based on the regulation of new power relationships between the state and actors in the digital domain.

## Scaling

## Cryptography

### A Graduate Course in Applied Cryptography

- **Source:** <http://toc.cryptobook.us/book.pdf>
- **Authors:** ​​Dan Boneh and Victor Shoup
- **Descripton:** A book that has relevant content for both beginning and advanced cryptographers; beginning readers can learn how cryptographic systems work and detailed proofs are provided for more advanced readers.
- **Relevance:**  
Some notable chapters:  
Ch.8 - Hashing is used everywhere.  
Ch.9.8 - TLS is the standard of [libp2p handshake protocol.](https://github.com/libp2p/specs/blob/master/tls/tls.md) (Ethereum 2.0)  
Ch.15.2.1 - Edwards form of eliptic curve is used in zero knowledge circuits for its performance.  
Ch.15.5.3 - Eliptic curve pairing is used in BLS signature.(aggregate signature to increase network throughput, Ethereum2.0)  
Ch.19.3 - Eliptic curve digital signature algorithm (ECDSA) is used in transactions.  

### Method of providing digital signatures (Merkle trees)

- **Source:** <https://patents.google.com/patent/US4309569>
- **Authors:** Ralph C. Merkle
- **Description:** Original research detailing Merkle trees as a method of providing a digital signature for purposes of authentication of a message, which utilizes an authentication tree function of a one-way function of a secret number.
- **Relevance:** Merkle trees allow for efficient and secure verification of different blocks of data, which is a foundational part of blockchain technology.

### Merkling in Ethereum

- **Source:** <https://blog.ethereum.org/2015/11/15/merkling-in-ethereum/>
- **Authors:** Vitalik Buterin
- **Description:** How Merkle trees are used in Ethereum.
- **Relevance:** A practical application of Merkle trees in a functional blockchain.

### Verkle Trees

- **Source:** <https://math.mit.edu/research/highschool/primes/materials/2018/Kuszmaul.pdf>
- **Authors:** John Kuszmaul
- **Description:** Original research detailing how large Merkle tree proofs can require huge bandwidth consumption and how Verkle trees can be an alternative.
- **Relevance:** How/Why Verkle trees could replace Merkle trees for many applications.

### Verkle trees (Blog post)

- **Source:** <https://vitalik.ca/general/2021/06/18/verkle.html>
- **Authors:** Vitalik Buterin
- **Description:** A possible practical application of Verkle trees in a functional blockchain.
- **Relevance:** An advantage to Verkle trees over Merkle trees is that proof sizes decrease by a factor of 6-8.

### MiMC: Efficient Encryption and Cryptographic Hashing with Minimal Multiplicative Complexity [AGRRT16]

- **Source:** <https://eprint.iacr.org/2016/492.pdf>
- **Authors:** Martin Albrecht, Lorenzo Grassi, Christian Rechberger, Arnab Roy, and Tyge Tiessen
- **Description:** An efficient hashing algorithm with few multiplications (lower multiplication complexity).
- **Relevance:** The computation is *friendly* in scenarios such as: fully homomorphic encryption (FHE), zero knowledge proof (ZK), or secure multi-party computation (MPC).

### Baby Jubjub Elliptic Curve

- **Source:** <https://eips.ethereum.org/EIPS/eip-2494>
- **Authors:** Barry WhiteHat, Jordi Baylina, and Marta Bell ́es
- **Description:** Baby jubjub is the Ethereum variant of jubjub Edwards eliptic curve on Zcash. The jubjub curve and baby jubjub curve are generated from bls12-381 curve and bn254 curve, respctively. 
- **Relevance:** Baby jubjub eliptic curve (and pairing based cryptography) is used in zero knowledge circuits for its performance. Baby jubjub is not implemented in EVM as of yet, and using on mainnet should be avoided.

### Pedersen Hash [HBHW19]

- **Source:** <https://raw.githubusercontent.com/zcash/zips/main/protocol/sapling.pdf>, page 60
- **Authors:** Daira Hopwood, Sean Bowe, Taylor Hornby, and Nathan Wilcox
- **Description:** It's a CRHF (collision resistant hash function) compared to MiMC. Also designed to be circuit friendly. The output of Pedersen hash is a compressed point on an elliptic curve.
- **Relevance:** First proposed by the Zcash team, and it's now being used by open source toolkits on Blockchains as cryptographic primitives. The Ethereum variant of Pedersen Hash can be found [here.](https://iden3-docs.readthedocs.io/en/latest/_downloads/4b929e0f96aef77b75bb5cfc0f832151/Pedersen-Hash.pdf)

### POSEIDON: A New Hash Function for Zero-Knowledge Proof Systems [GKRRS19]

- **Source:** <https://eprint.iacr.org/2019/458.pdf>
- **Authors:** Lorenzo Grassi1, Dmitry Khovratovich, Christian Rechberger, Arnab Roy, and Markus Schofnegger
- **Description:** A family of hash functions defined over GF(p) objects. The circuit constraints needed in various zero knowledge proving system is significantly reduced with the use of POSEIDON hash.
- **Relevance:** Some of the hashing algorithms inside Plonk, GROTH16, Bulletproofs, Redshift, or STARKs, can be replaced to further increase efficiency.

### How To Simulate It – A Tutorial on the Simulation Proof Technique

- **Source:** <https://eprint.iacr.org/2016/046.pdf>
- **Authors:** Lindell, Yehuda.
- **Description:** A tutorial about simulation which fills in the gaps people often overlooked when learning cryptography, especially zero-knowledge proof.
- **Relevance:** The key from interactive zero knowledge scheme to non interactive zero knowledge scheme is the existence of simulator. The verifier can thus interact with the simulator instead of the prover. However, such simulation paradigm feels very arcane to newcomers. This tutorial paper provided a systematic way to learn it, and the importance to it.

### Roll_up

- **Source:** <https://github.com/barryWhiteHat/roll_up>
- **Authors:** Barry Whitehat 
- **Description:** The original work of rollups on Blockchain.
- **Relevance:** It brought a new era on data compression on chain, and an innovation on general scalibility.

### Succinct Non-Interactive Zero Knowledge for a von Neumann Architecture (zk-SNARKs) [BCTV14b]

- **Source:** <https://eprint.iacr.org/2013/879.pdf>
- **Authors:** Eli Ben-Sasson, Alessandro Chiesa, Eran Tromer, Madars Virza
- **Description:** Original research that makes improvements on previous zk-SNARK work.
- **Relevance:** The two key contributions to previous zk-SNARK work are: a universal circuit generator that scales additively with program size and a zk-SNARK for arithmetic circuit satisfiability.

### On the Size of Pairing-based Non-interactive Arguments [GROTH16]

- **Source:** <https://eprint.iacr.org/2016/260.pdf>
- **Authors:** Jens Groth
- **Description:** The first widely used zk-SNARK construction on Blockchain, due to its succinctness and construction with quadratic arithmetic program.
- **Relevance:** [GROTH16] is still the fastest proving system with smallest proof size. However, the requirement of a *trusted setup* is its Achille's heel.

### Bulletproofs: Short Proofs for Confidential Transactions and More [BBBPWM18]

- **Source:** <https://eprint.iacr.org/2017/1066.pdf>
- **Authors:** Benedikt Bunz, Jonathan Bootle, Dan Boneh, Andrew Poelstra, Pieter Wuille, and Greg Maxwell
- **Description:** Bulletproofs have a short proof size and no trusted setup.
- **Relevance:** In blockchains, where proofs are transmitted over a network or stored for a long time, short proofs reduce overall cost. Famously used in Monero.

### Sonic: Zero-Knowledge SNARKs from Linear-Size Universal and Updatable Structured Reference Strings [MBKM19]

- **Source:** <https://eprint.iacr.org/2019/099.pdf>
- **Authors:** Mary Maller, Sean Bowe, Markulf Kohlweiss, Sarah Meiklejohn
- **Description:** Sonic is a zk-SNARK that supports a universal and continually updatable structured reference string, whose size scales linearly.
- **Relevance:** Sonic addresses the tradeoff between universality and functional requirements of an untrusted setup.

### PlonK: Permutations over Lagrange-bases for Oecumenical Noninteractive arguments of Knowledge [GWC19]

- **Source:** <https://eprint.iacr.org/2019/953.pdf>
- **Authors:** Ariel Gabizon, Aztec Zachary J. Williamson, Oana Ciobotaru
- **Description:** States that the version of Sonic enabling fully succinct verification still requires relatively high proof construction overheads.
- **Relevance:** Plonk aims to improve on Sonic, as it is a universal SNARK with fully succinct verification and significantly lower prover running time. It's the most promising proving system in the coming days on Ethereum.

### Scalable, transparent, and post-quantum secure computational integrity (zk-STARKs) [BBHR18]

- **Source:** <https://eprint.iacr.org/2018/046.pdf>
- **Authors:** Eli Ben-Sasson, Iddo Bentov, Yinon Horesh, Michael Riabzev
- **Description:** A transparent ZK system (ZK-STARK) in which verification scales exponentially faster than database size.
- **Relevance:** Relevant to both scalability and privacy with respect to blockchains, in addition to being post-quantum secure as well.

### Secure Multiparty Computation (MPC)

- **Source:** <https://eprint.iacr.org/2020/300.pdf>
- **Authors:** Lindell, Yehuda.
- **Description:** A great up-to-date review about the importance of secure multiparty computation.
- **Relevance:** One of the most apparent scenario is social recovery (via secret sharing) of wallet keys, which solved general user’s pain on private key and memonics (seed phrase) lost. It’s getting more and more likely that we’ll see some MPC solution mixed with layer 2 rollups, in order to gain some unique property under such combination, to solve issues such as MEV/frontrunning, where the relevant researches can already be found recently.

## Consensus
