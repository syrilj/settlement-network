---
sidebar_position: 2
---

# Privacy

An extension to the Universal L2 that adds privacy to the Universal Layer 2 (UL2)

## Advantages

- Private Burn
- Private Mint

## Disadvantages

- Need to generate the proof locally
- Need to have a common withdrawal amount

## Process Description

![Universal L2 Privacy Flow](../../assets/universal-l2-flow.png)

1. The User submits a deposit transaction worth 100 USDT into the bridging contract on ETH L1 and receives 100 USDT on a ETH UL2 from the official bridge contract.
2. The User submits a burn transaction for 100 USDT to a **private** burn address, **this burn address is locally generated similar to [EIP-7503](https://ethereum-magicians.org/t/eip-7503-zero-knowledge-wormholes-private-proof-of-burn-ppob/15456)**.
3. **The User** generates a Proof of Burn.
4. The User submits the Proof of Burn and the redemption address to redeem to the AVA UL2 which mints 100 USDT from the official bridge contract.
5. The User submits a withdrawal transaction worth 100 USDT from AVA UL2 and receives 100 USDT on AVA L1.

## Future Expansions

- Can benefit from Fully Homomorphic Encryption (FHE)
- Need to have a way to reveal that transactions are legally compliant
