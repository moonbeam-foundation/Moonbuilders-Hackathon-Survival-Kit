# EthDenver Moonbuilder's Survival Guide 2024
Everything you need to get started building on Moonbeam, optimized for builders

![Banner Image](https://i.ibb.co/1RJfyXV/header.jpg)

Welcome to EthDenver! For a full write-up of Moonbeam's participation in EthDenver, check out [this blog post](https://medium.com/moonbeam-network/lets-moonbeam-chill-at-ethdenver-23-789adca04849). 

## Talks & Workshops ✏️
*To be announced*
 
## 🎥 Introducing Moonbeam's 2024 EthDenver Bounty
In this [bounty introduction video](https://youtu.be/pufGqu1h8YU), Kevin reveals Moonbeam's 2023 Bounties including the challenge descriptions, expectations, and prizes.

[![Introductory Video](https://i.ibb.co/y8x2kP7/You-Tube-Thumbnails-72.png)](https://youtu.be/i1tiljpVET0?si=abZR7yaE0wfNrJPV)

## Moonbeam's 2024 Eth Denver Bounty: Cross-Chainify any dApp with Moonbeam
- *$10,000 in Prizes, 3 winners*
- *TLDR: Take any open-source dApp (existing or new) and make it cross-chain with Moonbeam! Use General Message Passing (GMP) to trigger an on-chain action. Moonbeam can be either the chain sending the message or receiving the message.*

### Bounty Requirements
Your goal with this bounty is to take any dApp and enhance it to be a cross-chain dApp. The dApp can be pre-existing and open source (you didn't create it) OR it can be your own dApp. To cross-chainify your dApp, you can use any General Message Passing (GMP) provider to send messages to or from Moonbeam. Thus, Moonbeam should be either the network sending the cross-chain message or receiving the cross-chain message. Typically, your cross-chain messages will include smart contract calls such that a user can interact with a smart contract from a different chain, providing a seamless cross-chain experience to the end user. 

### What does success look like? What are possible features that you are looking for?

The best submissions for this bounty will clearly demonstrate enhancing a dApp with cross-chain capabilities. The best ones will have an elegant UX and demonstrate a clear use-case being fulfilled. 

For example, suppose you're working on an NFT Marketplace that's currently deployed to Polygon. For your bounty submission you'd like to add cross-chain support for Moonbeam users to interact with the NFT Marketplace directly from Moonbeam. Success here would involve setting up cross-chain contract calls from Moonbeam to Polygon to interface with the NFT Marketplace on Polygon. If a user wants to buy an NFT, the user would confirm the transaction on Moonbeam, a cross-chain message will be sent to Polygon, and the NFT will be delivered to the user's corresponding address on Polygon (e.g. the same address as their Moonbeam address). The user didn't need to bridge funds, they didn't need to have any Matic tokens on Polygon (all gas is paid on Moonbeam) and they didn't need to switch to a different network in their wallet. All of this combines to provide an excellent experience to the end-user on Moonbeam. 

### What are the UI / UX Requirements?
Most submissions will be a web-based dApp, but you’re more than welcome to build on mobile as well. Browser-based dApps can ideally be deployed to a publicly accessible hosted URL (e.g. Vercel). If not deployed, that’s fine too, just indicate clear instructions in the ReadMe how to build and run the dApp locally. 

The dApp should use any GMP provider supported by Moonbeam or Moonbase Alpha, including but not limited to Axelar, Wormhole, LayerZero, Hyperlane, or Polkadot’s native XCM to build the cross chain components of the dApp. 

## Can you give me some examples of cool stuff to build?

What are some examples of some great cross-chain dApp ideas? We're so glad you asked! Here are a few to get you started:

### Build a Cross-Chain NFT Marketplace and Minter

NFTs have exploded in popularity in recent years. With good reason - they’re fun, engaging, and addictive. But by and large, most NFT projects are not yet truly cross-chain. You may interact with NFT marketplaces that have support for multiple chains, but these are typically just single-chain NFT marketplaces that repeatedly ask users to switch their networks. 

Picture an NFT marketplace on Moonbeam that allows you to buy and sell NFTs on many different chains from Moonbeam as the hub chain. This is made possible by [general message passing or GMP](https://moonbeam.network/blog/what-is-gmp/), which allows you to send a message to another connected chain (Moonbeam is highly interconnected), and take an action such as buying an NFT or listing one of your NFTs for sale. As an example, let’s say I wanted to buy an NFT on Polygon. I’ll confirm the purchase transaction on Moonbeam, paying the fees in Moonbeam’s GLMR token, and the dApp will send a cross-chain message to Polygon to buy that NFT, and it will be delivered to my corresponding address on the Polygon network. 

In addition to the marketplace feature, it would be nice to have (although not necessary) the ability for users to mint their own NFTs on the chain of their choice. For example, the user might want to mint 100 ERC-721s on Polygon, and they can do this via a cross-chain call sent directly from Moonbeam to Polygon, without acquiring MATIC tokens. While you may already have MATIC tokens lying around, not every user will have tokens for every chain that they want to interact with, and it can be hard to manage via bridging. Moonbeam is connected to a huge variety (and growing number) of chains via GMP providers like [Axelar](https://docs.moonbeam.network/builders/interoperability/protocols/axelar/), [Hyperlane](https://docs.moonbeam.network/builders/interoperability/protocols/hyperlane/), [LayerZero](https://docs.moonbeam.network/builders/interoperability/protocols/layerzero/), and [Wormhole](https://docs.moonbeam.network/builders/interoperability/protocols/wormhole/). These protocols make it truly easy to call a contract on a remote chain - all you need to do is specify the destination chain, the contract address you want to interact with, and the payload (contract call data). With general message passing, you can future proof your NFT marketplace. 

TLDR: Make an NFT marketplace on Moonbeam that allows you to buy and sell NFTs on several different chains! 

### Build a Cross-Chain DeFi Helper

Managing DeFi activities across multiple chains can be a cumbersome task. For a user to participate in DeFi different chains, they typically need to bridge funds, acquire the gas token of the destination chain, deposit/stake funds, and of course, claim rewards. Moonbeam is uniquely positioned as a hub for cross-chain connectivity via a variety of GMP protocols and that means you can take part in DeFi on many different chains without ever leaving Moonbeam. How does that work? The answer lies in Moonbeam’s extensive integrations with a variety of GMP protocols, including Axelar, [Axelar](https://docs.moonbeam.network/builders/interoperability/protocols/axelar/), [Hyperlane](https://docs.moonbeam.network/builders/interoperability/protocols/hyperlane/), [LayerZero](https://docs.moonbeam.network/builders/interoperability/protocols/layerzero/), [Wormhole](https://docs.moonbeam.network/builders/interoperability/protocols/wormhole/), and of course, [Polkadot's native XCM](https://docs.moonbeam.network/builders/interoperability/xcm/overview/)

These protocols make it truly easy to call a contract on a remote chain - all you need to do is specify the destination chain, the contract address you want to interact with, and the payload (contract call data). It’s that simple.

So, imagine a scenario where a user has $100 in USDC on Moonbeam that they want to put to work. It just so happens that there is a juicy opportunity on Aave on Polygon. You can use a GMP Protocol like Axelar to simultaneously bridge the $100 in USDC to Polygon and deposit in Aave, all in one click. The user doesn’t have to have any Polygon tokens (they will pay for the cross-chain transaction with GLMR on Moonbeam), and they don’t have to switch networks or perform any wizardry. They just need to click and confirm 1 transaction that you’ve prepared for them. This is just an example of what you can do and it is not meant to be the only example 

The design of your cross-chain DeFi Helper is entirely up to you. You can make it as simple (for example, click here to stake and we will automatically find the best opportunity for you) or as advanced (display a list of the highest-yielding opportunities on any connected chain, allowing the user to choose their desired one). Your dApp should aim to simplify the degen’s life at each step of the process - depositing, withdrawing, and claiming rewards. Moonbeam can be either your hub network coordinating the cross-chain actions on another network or a connected network dispatching actions on a particular DeFi protocol on Moonbeam. In other words, Moonbeam must be 1 of the networks you use. 

Remember these are just suggestions to get you thinking - you can go an entirely different direction. The above examples will not be favored or prioritized in the judging. 


### Remind me, what's GMP again?

General Message Passing (GMP) Protocols allow you to send messages to other chains, including messages that contain contract call data and can trigger actions on remote chains such as buying an NFT, making a swap, & much more. Moonbeam has integrated with a variety of GMP Protocols including [Axelar](https://axelar.network/), [Hyperlane](https://www.hyperlane.xyz/), [LayerZero](https://layerzero.network/), [Wormhole](https://docs.wormhole.com/wormhole/) & of course, Polkadot's native [XCM](https://wiki.polkadot.network/docs/learn-xcm). These protocols make it truly easy to call a contract on a remote chain - all you need to do is specify the destination chain, the contract address you want to interact with, and the payload (contract call data). It’s that simple. 


### Rewards:
* 1st place: 6,000 USDC 
* 2 Runner Ups: 2,000 USDC each

## 🎥 How the Bounties will be Judged + Tips for Success
In this [Bounty Judging Video](https://youtu.be/NVMUfx8BF3I), Kevin explains the judging guidelines and tips for success. Sample projects are also discussed! 

[![Judging Guidelines Video](https://i.ibb.co/3YKf8q3/34.png)](https://youtu.be/NVMUfx8BF3I)


## What's Moonbeam?
Moonbeam is a smart contract platform for building cross-chain connected applications that can access users, assets, and services on any chain. By uniting functionality from Ethereum, Cosmos, Polkadot and more into a single platform, Moonbeam solves today's fragmented user experience — unlocking true interoperability and paving the way for the next generation of applications. The Moonbeam platform uses integrated cross-chain messaging to allow developers to create smart contracts that access services across many remote blockchains. This approach, plus Moonbeam's developer-friendly EVM platform, vast tool support, and modern Substrate architecture, creates the ideal development environment for building connected applications.

## What's Polkadot?
[Polkadot](https://polkadot.network/) unites and secures a growing ecosystem of specialized blockchains called parachains. Apps and services on Polkadot can securely communicate across chains, forming the basis for a truly interoperable decentralized web. Moonbeam is a Polkadot parachain. 

## Meet the Networks (and block explorers)
* **<a href="https://moonscan.io/" target="_blank">Moonbeam</a>** - Mainnet
* **<a href="https://moonbase.moonscan.io/" target="_blank">Moonbase Alpha</a>** - Public testnet

## Connect to the Moonbeam Networks
You can connect your wallet to the following Moonbeam networks automatically by visiting the Moonbeam docs site and pressing the **[Connect MetaMask](https://docs.moonbeam.network/)** button at the top or manually with the following instructions:
* [Moonbeam](https://docs.moonbeam.network/builders/get-started/networks/moonbeam/)
* [Moonbase Alpha](https://docs.moonbeam.network/builders/get-started/networks/moonbase/)

## Moonbase Alpha Faucet
* You can get [DEV testnet tokens here](https://apps.moonbeam.network/moonbase-alpha/faucet/).
* You can make a swap for [testnet cross chain assets here](https://moonbeam-swap.netlify.app/#/swap).
* If you need more tokens in bulk for testing purposes don't hesitate to reach out to us in [Discord](https://discord.gg/moonbeam).

## Resources for Bounty 1 - Use a GMP Protocol to Remotely Call a Contract
Moonbeam has integrated with a variety of GMP protocols including Axelar, Hyperlane, LayerZero, and Wormhole. Of course, you can also use Polkadot's native XCM to perform cross chain contract calls within the Polkadot ecosystem. It's recommended that you familiarize yourself with the GMP protocol you'd like to build with by following their tutorial. 

### Building a Cross-Chain DApp with Axelar? Start Here
* Make your first cross-chain contract call [in this step-by-step tutorial](https://moonbeam.network/blog/connected-contracts-axelar/)
* For a comprehensive overview of the Axelar protocol, visit [Axelar Academy](https://axelar.academy/ecosystem/introduction-to-axelar/)
* For hands-on docs and examples, visit [Axelar Docs](https://docs.axelar.dev/dev/intro)
* [Send a cross chain message with Axelar](https://docs.axelar.dev/dev/build/gmp-messages)

### Building a Cross-Chain DApp with Hyperlane? Start Here
* Make your first cross-chain contract call [in this step-by-step tutorial](https://moonbeam.network/blog/connected-contracts-with-hyperlane/)
* [Hyperlane Docs](https://docs.hyperlane.xyz/docs/introduction/readme)
* [Send a cross chain message with Hyperlane](https://docs.hyperlane.xyz/docs/apis/messaging-api/send)

### Building a Cross-Chain DApp with LayerZero? Start Here
* Make your first cross-chain contract call [in this step-by-step tutorial](https://moonbeam.network/blog/connected-contracts-layerzero/)
* [Code samples](https://layerzero.gitbook.io/docs/evm-guides/code-examples)
* [Send a cross chain message with LayerZero](https://layerzero.gitbook.io/docs/evm-guides/master/how-to-send-a-message)

### Building a Cross-Chain DApp with Wormhole? Start Here
* Get started with Wormhole [in this step-by-step tutorial](https://moonbeam.network/blog/connected-contracts-wormhole/)
* [Wormhole Docs](https://docs.wormhole.com/wormhole/)
* [Wormhole xDapp Development Guide book](https://book.wormhole.com/)

### Building a Cross-Chain DApp using Polkadot's XCM? Start here
* [XCM Overview](https://docs.moonbeam.network/builders/interoperability/xcm/overview/)
* [Moonbeam and XCM](https://youtu.be/uadmRX_HWzw)
* [Remote Execution](https://docs.moonbeam.network/builders/interoperability/xcm/xcm-transactor/)
* [Remote EVM Calls](https://docs.moonbeam.network/builders/interoperability/xcm/remote-evm-calls/)


### Prefer Video Tutorials? 
Jeremy from the Moonbeam Team has created an excellent series of videos explaining the ins and outs of all of the GMP protocols integrated with Moonbeam. 

* [Architecture of Connected Contracts](https://drive.google.com/file/d/1PxaKgRxaQFbKpk49q-BAtFsbfdtm0LYI/view?usp=sharing)
* [Architecture of Axelar's GMP Framework](https://drive.google.com/file/d/1Lez5fAatVxIyDIEWCIQNV_f3OVsiafsT/view?usp=sharing)
* [Writing Connected Contracts with Axelar](https://drive.google.com/file/d/1-_-7QdeFXRkYqEYPDLk1s1f3qOMgJiGy/view?usp=sharing)
* [Writing Connected Contracts with LayerZero](https://drive.google.com/file/d/1Ek6L8ffCvW0bLcNMUAtDAJFCGEhV95ZT/view?usp=sharing)
* [Building in the Interchain with Hyperlane](https://www.youtube.com/watch?v=0YYNOCrxSmY&ab_channel=MoonbeamNetwork)
* [Wormhole Architecture](https://drive.google.com/file/d/1UW__Fgs825a-lKQ_KbdzveIJT1X-2iV_/view?usp=sharing)
* [Writing Connected Contracts with Wormhole](https://drive.google.com/file/d/1hYAMnI9bYzfkFBqO3a9gxuz2aHX07rkl/view?usp=sharing)

## General Resources

### Building a web app as part of your DApp? Start here 
* [ScaffoldEth](https://github.com/scaffold-eth/scaffold-eth) is a fantastic way to quickly spin up a React frontend that connects to your solidity smart contract. [Learn how to use ScaffoldEth with Moonbeam here](https://docs.moonbeam.network/builders/build/eth-api/dev-env/scaffold-eth/). 
* [Configure your preferred developer environment for Moonbeam](https://docs.moonbeam.network/builders/build/eth-api/dev-env/)
* [Use JS libraries like Ethers.js or Web3.js to integrate smart contract functionality into your webapp](https://docs.moonbeam.network/builders/build/eth-api/libraries/)

### Office Hours
*To be announced*

### Additional places to Get Help
* [**Hackathons** Channel of the Moonbeam Discord](https://discord.gg/moonbeam)
* Come by the Moonbeam Booth (Devtopia, Booth R) anytime! 

### Judging Criteria
Projects should meet bounty specific requirements. All Moonbeam bounties will be judged according to the standard ethDenver judging guidelines - that is: 
* Theme Fit
* Originality & Innovation
* Ease of use (UI/UX)
* Sustainability (marketplace viability)
* Technical complexity
* Level of Completion

### General Helpful Resources
* [Moonbeam Docs Site](https://docs.moonbeam.network/) 
* [Moonbuilders Academy](https://academy.moonbeam.network/) 
* [Developer Discord](https://discord.gg/moonbeam)
* [Getting Started with the Moonbase Alpha Testnet](https://docs.moonbeam.network/builders/get-started/networks/moonbase/) 

#### Disclaimer
We reserve the right to withhold bounty payouts where low quality submissions do not meet our bounty requirements.
