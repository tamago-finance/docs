# Tamago V1 👴

The V1 is no longer supported and updated, it's a liquid synthetic asset issuance protocol with flexible collateral reserves aims to accelerate the real-world business adoptions with DeFi. The protocol utilizes a under-collateralization scheme as we seen in popular DeFi protocols such as MakerDAO, Synthetix and UMA.

Since we recently shifted the direction to Metaverse, the V1 is used as a base to developing further research and the UI still there without maintenance, we encouraged users in V1 to withdraw their collateral back and move to V2.

#### $TAMG Token

The 1 million of $TAMG token has been minted and circulated on Polygon chain, the token itself will soon to be obsolete, the early token holder will receive exclusively right to claim the new token after upcoming IDO in 2022.

The token V1 contract addresses:

| Contract Name         | Address                                    | Chain   |
| --------------------- | ------------------------------------------ | ------- |
| Tamago Token (ERC-20) | 0x53BDA082677a4965C79086D3Fe69A6182d6Af1B8 | Polygon |
| Token Manager         | 0x38b073e96434Ec00A10eBb2f87f2Ee31579cb040 | Polygon |

#### Minting

When minting the synthetic asset, the collateral must be deposited on the smart contract through the overcollatelization scheme and the value of the collateral must be exceed the value of the loan all the time unless the debt position will be liquidated by anyone.

The total output can be defined by following equation:&#x20;

$$
Z = (X*Px)+(Y*Py) / (Pz*Cr) , Cr > Lr
$$

Cr = the collateral ratio, Lr = the liquidation ratio

Z = total synthetics to be minted, Pz = the price of reference asset in USD

X = total non-stablecoin collateral, Px = the price of non-stablecoin token in USD

Y = total stablecoin collateral, Py = the price of stablecoin token in USD

It's recommended to use more portion of stablecoin assets during the bear market and the opposite on the bull market to keep volatility under control, the smart contract has a helper function to indicates whether the market is on rise or fall and proper calculate each portion for the minter conveniently.
