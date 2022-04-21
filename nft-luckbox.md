---
description: Empowering every NFT community with WEB3 Smart On-Chain Raffle solutions
---

# NFT LUCKBOX 🎲

NFT Luckbox is a community-driven giveaway tool for Web3 & NFT projects. Built on open and collaborative infrastructure. NFT Luckbox helps Web3 projects and NFT artists connect with other NFT holders and build better communities.

At the same time, the NFT holders who contribute to the listing network have a chance to participate in the growth of the new projects.

### Background

Current NFT raffle solutions are highly centralized, meaning to launch a giveaway campaign one has to contact a mediator which consumes time and energy. And after the campaign is over the process of choosing the winners is not at all transparent and can't be verified. Often times these mediators use outdated Web2 tech such as Google forms or gleam to collect addresses, which can be a hassle and inconvenient.

Not to mention the possibility of scams in these giveaways which can shatter a brand image. WEB3 projects need smart WEB3 solutions which are decentralized, transparent, trustable, and verifiable.

\
NFT Luckbox is a one-stop solution for all your raffle/giveaway needs. The smart contract itself is decentralized and transparent meaning the raffles can be verified on the blockchain. We provide projects with smart on-chain giveaway solutions which make the process hassle-free and ready to launch in days as compared to centralized protocols which can take weeks to even months.

\
Also, gone are the days when you had to collect user addresses on google forms or other software manually. We let projects choose the community they want to Airdrop to and gain traction from the users of that community. At the same time giving users exposure to new NFT projects. A win-win for everyone.

\
We are trusted by various WEB3 projects including ApeX, Naga Dao, and Mao Dao among others.

### Architecture

* Built upon Chainlink VRF&#x20;
* Customizable Campaign&#x20;
* Automated regular Holder list update&#x20;
* Bot generated Merkle Tree&#x20;
* Verifiable through API & Smart Contract&#x20;
* Seed Generation from Chainlink VRF

### Chainlink VRF

The Chainlink VRF is used to generate a random number for drawing the game without the risk of manipulation by the attacker, the system makes a request to VRF nodes to get the new number within 1-3 minutes intervals, the number will be persisted in the factory contract and can be accessed from the NFT LUCKBOX contract for further drawing according to the probability that has been set by the owner of the NFT LUCKBOX contract.

### Drawing Mechanism <a href="#b940" id="b940"></a>

NFT LUCKBOX utilizes the Chainlink VRF algorithm to randomly pick a holder from the holder list. Essentially, the smart contract puts the holder list wallet addresses and the randomly generated (VRF) output through a mathematical operation in order to select the winner(s).

The number of winners for each raffle campaign is set by the creators. For raffle campaigns with multiple winners, the random number will be hashed multiple times to pick the winners.

This is the standard approach for selecting raffle campaign "winners" from the NFT Luckbox.



### How to start a raffle?

Campaign hosts should first select the community who they wish to distribute the prize to, before setting a launch date and prize details. As of writing, projects will need to manually submit their [application ](https://nftluckbox.xyz/raffles/create)to Luckbox admins to host their raffle campaigns. In future versions, campaign hosts will be able to list their campaigns themselves.

\
