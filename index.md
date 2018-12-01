## Introduction

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

![Hyperledger Composer](https://github.com/palnapatel/Capstone-Event/blob/master/Composer%20Playground.png)
![Composer](https://github.com/palnapatel/Capstone-Event/blob/master/Composer2.png)

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/palnapatel/capstone-event/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
