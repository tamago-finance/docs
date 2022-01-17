---
description: The NFT Gachapon powered by Chainlink VRF
---

# NFT Luckbox 🎲

NFT Luckbox is the NFT lottery project which is the first use case of the value-backed NFT as well as it can be a good tool for NFT creators to distribute their products, the user can be divided into 2 groups of:

* Users - The drawer who willing to pay a ticket to draw the Gachapon contract that made and maintained by its owner.
* Owners - The owner of the Gachapon contract who will receive the fee when the user draws his/her Gachapon contract.

### Background

Normally, the only way for NFT artists and projects to distribute their NFT is listing on the NFT exchange likes OpenSea, many of them are struggle because of many reason, we're making the Gashapon-liked smart contract to help distributing along with generating some revenues at the same time.

The Gashapon which is vending machine that dispense capsules of toys. These vending machines appear almost at every corner in Japan's streets. People love the excitement to open a box that is full of hope and imagination with infinite possibility. People buy special NFT with lower price. There really is something for everyone, no matter your age, gender or interests. In terms of NFT owners and creaters, they don’t find the right buyers for the right NFT. The boxes consisting of unique/ the hottest NFT will.

### Chainlink VRF

The Chainlink VRF is used to generate a random number for drawing the game without the risk of manipulation by the attacker, the system make a request to VRF nodes to get the new number within 1-3 minutes interval, the number will be persisted in the factory contract and can be accessed from any Gachapon contract for further drawing according to the probability that has been set by the owner of the Gachapon contract.

### Drawing Mechanism <a href="#b940" id="b940"></a>

The current mechanism is pretty simple, the randomness of the draws is truly fair and accessible for all who are willing to pay the ticket price that has been set by each Gachapon contract owner. Each slot need to set the winning chance by its owner in a percentage term, for example, if there are 2 NFTs in the Gachapon contract each has value of 10%, when the user draws the Gachapon, it will send the request to Chainlink VRF to find the random number between 0–10000, you will receive the first NFT if the number returned between 0–1000 and the second NFT with between 1001–2000, the rule is simple and straightforward.

This is how the current version works, however, the mechanism is continue improving and developing to achieve the high security standards with greater user experience.\
