# Introduction

### Motivation

The advancements in telecommunication, semiconductors, and Internet technologies have given rise to the surge of IoT devices. IoT is slowing allowing for the healthcare industry to reduce its dependencies on human and their associated human errors. Also, IoT medical devices are steadily improving healthcare and providing early diagnosis and treatment of serious issues.  

The data confidentiality and integrity of personal health information: patients want to transmit data to doctors or insurance providers without tampering and leakage; doctors, insurance providers wish to check patients’ complete and authentic medical records or case history, etc. We use blockchain to solve this challenge, which also brings other side benefits such as more intelligent and efficient ways to pair doctors with patients.

The device vulnerability in a potentially malicious network environment: as the popularity of medical IoT devices grows, so does the activities of attackers. As the intrusion becomes increasingly sophisticated and in large volume, using human inspection or firewall rules is not sufficient anymore. Poor cybersecurity in IoT medical devices potentially poses risks to both the wellbeing of patients as well as to the infrastructure that keeps the hospital running. It poses serious threats not only to people’s privacy, but also health.


### Objectives

Security is essential for the IoT industry as a whole, but it’s even more critical when you add in patient privacy. The objective of blockchain for healthcare (also called healthchain) is to prototype a secured, standardized health information exchange system. It helps to reduce cybersecurity risk, and potentially reduce impact on safety and operational risk, such as the loss of patient information or interference with the standard operation of a medical device.

The objective of the deep learning analyzer is to prove the concept of using deep learning as a classification method for intrusion detection systems. We want our trained model to be able to detect malicious patterns and notify people even those attacks have never been seen before. Also, the intrusion detection component can be deployed on device, and work efficiently.


### Blockchain

- Blockchain is literally just a chain of blocks. When we say the words “block” and “chain” in this context, we are actually talking about digital information (the “block”) stored in a public database (the “chain”)
- When a block stores new data it is added to the blockchain
- Types of Blockchain - Public, Private, Consortium
- Benefits of Blockchain:
  a. Greater Transparency
  b. Enchanced Security
  c. Improved Traceability
  d. Increased Efficiency and Speed
  e. Reduced Costs
- Blockchain allows multiple different parties to securely interact with the same universal source of truth


### Hyperledger Composer 

- Hyperledger Composer is an extensive, open development toolset and framework to make developing blockchain applications easier
- Hyperledger Composer can be used to quickly model the current business network, containing the existing assets and the transactions related to them
- Using Composer, you define the transactions which can interact with assets, participants who interact with the assets

![Composer](https://hyperledger.github.io/composer/v0.19/assets/img/Composer-Diagram.svg)


### Hyperledger Fabric

- Hyperledger Fabric is an open source enterprise-grade permissioned distributed ledger technology (DLT) platform, designed for use in enterprise contexts, that delivers some key differentiating capabilities over other popular distributed ledger or blockchain platforms
- It is used for developing applications or solutions with a modular architecture, it allows components, such as consensus and membership services, to be plug-and-play
- It leverages container technology to host smart contracts called “chaincode” that comprise the application logic of the system

![Fabric](https://www.altoros.com/blog/wp-content/uploads/2016/11/Hyperledger-Blockchain-Elli-Androulaki-fabric-model.jpg)


## Security

### Benenfits and Concerns

Security aspects of Hyperledger network
a. Enable TLS: encrypt peer traffic in transit
b. Enable ACL: prevents outsider access

- Spoofing: Fabric certificate authority generates X.509 certificates for its members
- Tampering: Use of cryptographic measures (SHA256, ECDSA) make tampering infeasible
- Repudiation: Tracks who did what using digital signatures
- Replay Attacks: Hyperledger Fabric uses read/write sets to validate the transaction. A replay of transactions will fail due to an invalid read set
- Information Disclosure: Hyperledger Fabric provides support for using TLSv1.2 for intransit encryption. It does not encrypt ledger data at rest (the operator's responsibility)
- Elevation of Privileges: Issued identities cannot upgrade their access (for example, create an identity) without manual review of access
- DoS/DDoS: HF is a permissioned network, no anonymous access. Same nodes / Admin can revoke offender’s access, and identity data help find liable person for legal action. Volume-based DDoS requires a large number of member nodes to be compromised, which is unrealistic in a large network and ineffective in a small network


## Working Hyperledger Composer

![composer playground](https://user-images.githubusercontent.com/35075881/49333613-d6f04880-f58f-11e8-994d-93c438c22ec3.png)
![composer2](https://user-images.githubusercontent.com/35075881/49333616-dce62980-f58f-11e8-9b64-ca853daadd72.png)


## Working Hyperledger Fabric

![fabric](https://user-images.githubusercontent.com/35075881/49333618-e1aadd80-f58f-11e8-821c-8ec8586fba51.png)
![fabric 2](https://user-images.githubusercontent.com/35075881/49333619-e40d3780-f58f-11e8-9718-73ac5c6bff46.png)


## Deep Learning IDS

- First, capture network traffic packets and transform them into high-level data sheets with fact labels
- Second, train the labeled data (UNSW-NB15) on machine learning models such as decision trees and neural network
- Third, evaluate the validility of machine learning IDS application by predicting unknown attacks

![feature-creation](https://user-images.githubusercontent.com/35075881/49333628-19b22080-f590-11e8-8085-191e0a851ad9.png)

![ml-ids-module](https://user-images.githubusercontent.com/35075881/49333625-0901aa80-f590-11e8-9053-0f58af89ec88.png)


## System Design

### Overview

![hyperledger-3](https://user-images.githubusercontent.com/35075881/49333666-e8862000-f590-11e8-83d4-8746c6ca2d3d.png)

![class diagram](https://user-images.githubusercontent.com/35075881/49333668-ed4ad400-f590-11e8-9be6-347366653fb9.png)


## Contributors (NEU - MSCY)

- Palna Patel
- Hongchao Wang
- Yunong Chen
- Kushal Mistry
- Ying Wu


