---
description: Empowering every NFT community with WEB3 Smart On-Chain Raffle solutions
---

# NFT Luckbox Project



NFT Luckbox is a community-driven giveaway tool for Web3 & NFT projects. Built on open and collaborative infrastructure. NFT Luckbox helps Web3 projects and NFT artists connect with other NFT holders and build better communities.

At the same time, the NFT holders who contribute to the listing network have a chance to participate in the growth of the new projects.

### Background

Current NFT raffle solutions are highly centralized. In order to launch a giveaway campaign one must contact and coordinate with a mediator, consuming both valuable time and resources. Once the campaign has ended, the process of choosing the campaign winners is also untransparent and unverifiable. Oftentimes these mediators use outdated Web2 technology such as Google Forms or Gleam to collect addresses, which is both inconvenient and prone to error.

Not to mention the possibility of scams that can shatter a community’s brand image. Web3 projects demand Web3 solutions that are decentralized, transparent, trustable, and verifiable.

NFT Luckbox is a one-stop solution for all your raffle/giveaway needs. The smart contract itself is decentralized and transparent, meaning the raffles can be verified on the blockchain. We provide projects with smart on-chain raffle/giveaway solutions which streamline the giveaway process, reducing execution time to a matter of days compared to centralized protocols which can take anywhere from weeks to months.

Gone are the days where it is necessary to manually collect user addresses using Google Forms and/or other software. We let projects easily perform Airdrops to their chosen communities, gaining traction from the users of that community. At the same time, these users will also gain exposure to new NFT projects. A win-win for everyone.

We are trusted by various WEB3 projects including [0xMonkey](https://nftluckbox.xyz/project/9), [The Weirdo Ghost Gang](https://nftluckbox.xyz/project/8), [Laser Cat](https://nftluckbox.xyz/project/7), [ApeX](https://nftluckbox.xyz/project/5), [Smart Collector Card](https://nftluckbox.xyz/project/4), [Naga Dao](https://nftluckbox.xyz/project/3), and [Mao Dao](https://nftluckbox.xyz/project/2) among others.

### NFT LUCKBOX Raffle Features

Our NFT Luckbox solution presents many exclusive features which benefit both raffle organizers and raffle participants. These include:

* An intuitive and well-conceived raffle solution that allows newer users to easily understand the inner workings of the platform and better tailor their campaigns to their respective communities.&#x20;
* A transparent and verifiable raffle solution that does not rely on the trust of any specific parties.&#x20;
* A free-of-charge solution, we don’t charge additional fees for using our service.&#x20;
* A raffle board on our main website ([https://nftluckbox.xyz](https://nftluckbox.xyz)) displays all on-going raffles such that users can easily view and participate in the raffles.&#x20;
* &#x20;An effective notification system that promptly alerts raffle prize winners through email about their prize winnings.

### Architecture

* Built upon Chainlink VRF&#x20;
* Customizable Campaign&#x20;
* Automated regular Holder list update&#x20;
* Bot generated Merkle Tree&#x20;
* Verifiable through API & Smart Contract&#x20;
* Seed Generation from Chainlink VRF

### Chainlink VRF

The Chainlink VRF is used to generate a random number for drawing the game without the risk of manipulation by the attacker, the system makes requests to VRF nodes to get the new numbers in 1-3 minute intervals, the number will be persisted in the factory contract and can be accessed from the NFT LUCKBOX contract for further drawing according to the probability that has been set by the owner of the NFT LUCKBOX contract.

### Drawing Mechanism <a href="#b940" id="b940"></a>

NFT LUCKBOX utilizes the Chainlink VRF algorithm to randomly pick a holder from the holder list. Essentially, the smart contract puts the holder list wallet addresses and the randomly generated (VRF) output through a mathematical operation in order to select the winner(s). The number of winners for each raffle campaign is set by the creators. For raffle campaigns with multiple winners, the random number will be hashed multiple times to pick the winners. This is the standard approach for selecting raffle campaign "winners" from the NFT Luckbox.

### How to start a raffle?

Campaign hosts should first select the community who they wish to distribute the prize to, before setting a launch date and prize details. As of writing, projects will need to manually submit their[ application](https://nftluckbox.xyz/raffles/create).\


![](<.gitbook/assets/4 STEP.png>)
