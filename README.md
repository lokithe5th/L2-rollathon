# L2-rollathon
Rollathon Submission

# Supply Chain DApp  

The dapp allows for a company's QA to record quality metrics and provides a method for downstream supply chain participants to verify given quality metrics at a later date.

## Use Case  

It is sometimes necessary in the course of normal supply chain operations to verify any given data regarding a product's quality.  

For example, should a quality dispute arise between a supplier and an end-user, a supplier may present the end-user with their own in-house data, generated from internal QA procedures, to prove the quality of the supplied product. Such data may be treated as untrustworthy by the end-user, given the incentive of the supplier to mitigate their own risk (i.e. the supplier may want to cover their own ass by fudging their data). 

This application allows for supply chain participants to submit data as soon as it is generated. The data necessary for attestation is then stored and can be verified at a later date by any party in the supply chain. This allows for trustless verification of data required in the supply-chain.  

## Implementation  

The DApp consists of different pieces:

- Smart contracts on an L2 blockchain which govern access, token economics, submission and attestation of data
- A javascript front end which allows interaction with the contracts by the supplier and the end-user  

