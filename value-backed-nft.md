---
description: Aka. Voucher NFT
---

# Value-backed NFT

![The value-backed NFT represents a specific value of USD similar to banknotes](<.gitbook/assets/ang-pow-preview (1).png>)

The value-backed NFT is a financial voucher NFT backed by the value of multi-collateral assets, the NFT itself has a value attached and can be minted and redeemed by anyone, the minter must locking a certain amount of collateral tokens in a reserve pool, each NFT represents the specific amount of currencies, commodities and digital assets aims to solve the illiquid problem of traditional NFT.

The protocol combines a number of mature approaches that proven from DeFi side and we eager to adopt into NFT market ensure stability and resilience are met.

### Stability Mechanism

NFT can be minted and redeemed as its price tag when the collateral ratio is equal to 100%, however it's unlikely that the ratio will be maintained at 100% all the time due to volatility of collateral token prices.

We propose the mechanism to dynamically adjust the collateral level to be used during mint and redeem actions to help the ratio pegged at closer to 100%, at the beginning, users can create new NFT in debt form by depositing collateral assets into the smart contract and if the value of underlying collateral lower than the 100%, the redeemer have to send out a portion of collateral to be remained on the smart contract in order to adjust the ratio gradually shift back to 100%, the discount will be given when the ratio is higher than 100% with the same purpose.

$$
y=\log_{b}\left(kx+1\right)
$$

The given formula is used to calculate the offset fee and the discount that will be applied when:

x = Current Collateral Ratio, y = Target Collateral Ratio&#x20;

b = Logarithm base, k = Constant, vary by the volatility&#x20;

When minting and redeeming occurs on the protocol, the target ratio has been calculated according to the current ratio at that time and constants defined by the team.

![How the protocol controls the price](<.gitbook/assets/Add a little bit of body text (1).png>)

### Minting&#x20;

The protocol allows anyone to mint the value-backed NFT which is ERC-1155 complaint and can be traded on any well-known NFT exchange such as OpenSea. It's recommended the minter takes particular note of the rules that have been enforced by the smart contract to avoid further confusion.

At the very beginning, the $100 NFT can be minted by placing $100 of value into the system, each variant of NFT has its own vault and the collateral ratio must be calculated separately.

![The vault is separate for each variant](<.gitbook/assets/Untitled Diagram.drawio (1).png>)

When the collateral ratio is higher than 100%, there will be an arbitrage opportunity to mint the NFT as special price, the discount will be greater when the collateral ratio is far away from 100% and eventually bring the ratio down to the normal state.

Let's take the example if the variant's collateral value equals to $12,000 and the outstanding NFT value equals to $10,000 ($100 NFT x 100 Units Minted) then the collateral ratio is 120%, the target ratio has been calculated from the given formula to bring the ratio down, presuming that the target ratio is 110% then we have $1,000 to giveaway as a discount, to mint $100 NFT we need to deposit only $100-($1,000x$100/$12,000) = $92.

### Redeeming

The redeemer can claim back the full amount of collateral when the ratio is higher than 100% as there are sufficient collateral assets locked in the smart contract to pay it back while the offset fee will be deducted when the ratio dropping below than 100%.

| Collateral Ratio | NFT Variant | Redeem Price |
| ---------------- | ----------- | ------------ |
| 70%              | $100        | $65          |
| 90%              | $100        | $97          |
| 100%             | $100        | $100         |
| 120%             | $100        | $100         |



For example, if the variant's collateral value equals to $9,000 and the outstanding NFT value equals to $10,000 which means the ratio = 90%, the smart contract will calculate the target ratio to be achieved in a single transaction, assuming that the target is 95%, $500 is needed to shift the ratio from 90% to 95% then the offset fee will be charged regarding to the size of NFT to be redeemed, in this scenario the $100 NFT will be redeemed as $100 - ($500x$100/$10,000) = $95.
