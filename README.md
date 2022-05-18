# L2-rollathon
Rollathon Submission

# Supply Chain DApp  / SuppDApp

The dapp allows for a company's QA to record quality metrics and provides a method for downstream supply chain participants to verify given quality metrics at a later date.  

By leveraging Layer-2 technology it allows a business to enjoy the benefits of crypto technologies with fewer barriers to entry.  

Wide-based adoption of blockchain technology can be driven by cost-effective solutions on L2 protocols, providing a trustless solution for supply chain participants like suppliers, distributors, insurers and end-users.

## Use Case  

It is sometimes necessary in the course of normal supply chain operations to verify any given data regarding a product's quality.  

For example, should a quality dispute arise between a supplier and an end-user, a supplier may present the end-user with their own in-house data, generated from internal QA procedures, to prove the quality of the supplied product. Such data, being presented after the fact, may be treated as untrustworthy by the end-user, given the incentive of the supplier to mitigate their own risk (i.e. the supplier may want to cover their own ass by fudging their data). 

This application allows for supply chain participants to submit data as soon as it is generated. The data necessary for attestation is then stored on the blockchain and can be verified at a later date by any party in the supply chain. This allows for trustless verification of data required in the supply-chain using blockchain technology; by running the project on an L2 a business can provide this service at a cost-effective rate.  

## Implementation  

The DApp consists of different pieces:

- Smart contracts on an L2 blockchain which govern access, token economics, submission and attestation of data
- A javascript front end which allows interaction with the contracts by the supplier and the end-user  

### Contracts  

Take a value, which is essentially the hash of the complete file with the submission timestamp concatenated, and save it in a MerkleTree structure.  

Allow a wallet to verify the file's hash against the stored value and return true/false based on the result.  

Issue tokens on submission of data, require tokens on the request of the data.  

### Token Economics  

> "token/s" refers to the SuppDApp token

Token economics are incentives to encourage or discourage certain behaviours. In the case of SuppDApp, the incentive is for suppliers/service providers to submit their data, for which they are rewarded in tokens. These ERC20 tokens can then be swapped on DEXes. Verification of data on chain by supply-chain participants requires SuppDApp tokens, which can be obtained through trade or from suppliers through purchase or agreements.  

This token economic model allows for participants using the protocol to store data to be rewarded with tokens, which can then be swapped to offset the cost of submitting their data.  

The hope would be for all the participants in the supply-chain to participate, meaning that upstream/downstream participants who also commit data to the chain for verification can use their earned tokens to access the project services without the need for swapping on a DEX. This incentivises enterprise/commercial adoption, but with the added benefit of allowing trustless access to data verification by the end-user, as long as they have the required tokens.