# EthDenver Moonbuilder's Survival Guide
Everything you need to get started building on Moonbeam, optimized for builders

![Banner Image](https://i.ibb.co/GFVTSR2/export2-clipped.jpg)

## Talks & Workshops ✏️
* **[Buidl Week - Cross-Chain EVM Calls with XCM on Moonbeam/Polkadot](https://events.ethdenver.com/eden23/attendease/networking/experience/26fe998b-c291-47f0-8a7b-42e1de99ddcf/d02df489-2db2-4917-8b53-e4b3547f7f87)** - ***Saturday, February 25 at 10:20am MST @Buidl Hub Mainstage***: In this talk, Stephen Shelton will discuss how Polkadot's interoperability protocol works at a high level. He'll go into more details of how this can be used to access Moonbeam's EVM from a different chain. This opens a new realm of possibilities, as contracts in Moonbeam can access app-specialized blockchains inside the Polkadot ecosystem. But also, these specialized chains can tap into Moonbeam's EVM and all the benefits smart contracts offer.
* **[Camp Buidl - Build your First DAO and deploy it to Moonbeam using HardHat](https://www.ethdenver.com/campbuidl-logistics)** - ***Sunday, February 26 at 12:00pm MST and 4:30pm MST @ [Hydro](https://goo.gl/maps/1Jgpmnwu8ZQWGtLW8)***: In this Camp Buidl workshop, Moonbeam Blockchain Engineer Stephen Shelton will show you how to build your First DAO and deploy it to Moonbeam using Hardhat. You'll also gain an understanding of endpoints and API providers. 
* **[Cross Chain Protocol Architectures: Key Trends and
Challenges in 2023](https://events.ethdenver.com/eden23/attendease/networking/experience/8cade9b6-3b1e-4b51-83e6-91132e2f6e7a/3c2e7611-a7b2-4535-bfcc-3647561bf1c4)** - ***Thursday, March 2nd at 5pm MST @Infrastructure + Scalability Stage***: In this talk, Derek Yoo, Founder of Moonbeam, will share his experience helping dozens of projects pursuing multi-chain strategies. Derek will also dive into cross-chain protocol architectures, current market opportunities, and challenges, including market trends and future directions for cross-chain apps and infrastructure. 
* **[Remote Cross-Chain EVM Calls with XCM](https://events.ethdenver.com/eden23/attendease/networking/experience/0247a52b-aaee-4bcd-b099-41006497962b/fe8cecbb-68ae-4841-a6d1-482f11c05ff0)** - ***Friday, March 3rd at 11:30am MST @Buidl Palace***: Kevin Neilson and Stephen Shelton will introduce you to XCM and Remote EVM Calls. With remote cross-chain EVM calls now live on the testnet, you can now send an XCM message from a remote chain containing a contract call to be executed on Moonbeam's EVM. We'll go through the steps of generating a derivative account on Moonbeam that we'll control remotely via XCM. Then, we'll jump into crafting our remote EVM call - we'll initiate a swap on a Uniswap-style Dex to take place all from a remote chain.
 
## 🎥 Introducing Moonbeam's 2023 EthDenver Bounties
In this [bounty introduction video](https://youtu.be/pufGqu1h8YU), Kevin reveals Moonbeam's 2023 Bounties including the challenge descriptions, expectations, and prizes.

[![Introductory Video](https://i.ibb.co/jbzqB8f/You-Tube-Thumbnails-47.png)](https://youtu.be/pufGqu1h8YU)

## Bounty 1 - Make a Remote Contract Call

General Message Passing (GMP) Protocols allow you to send messages to other chains, including messages that contain contract call data and can trigger actions on remote chains such as buying an NFT, making a swap, & much more.

Moonbeam has integrated with a variety of GMP Protocols including [Axelar](https://axelar.network/), [Hyperlane](https://www.hyperlane.xyz/), [LayerZero](https://layerzero.network/), [Wormhole](https://docs.wormhole.com/wormhole/) & of course, Polkadot's native [XCM](https://wiki.polkadot.network/docs/learn-xcm). These protocols make it truly easy to call a contract on a remote chain - all you need to do is specify the destination chain, the contract address you want to interact with, and the payload (contract call data). It’s that simple. 

In order to be eligible for this bounty, your dApp should have at least some smart contract logic deployed to Moonbeam or Moonbase Alpha. Secondly, it needs to implement a cross-chain contract call that plays a non-trivial role in the application. As an example, if you’re building a cross-chain DEX, a cross-chain contract call that sends a message “HELLO WORLD” to another chain at random intervals would be considered trivial and not related to the dApp’s purpose. 

#### Rewards:
* 1st place: 4,000 USDC 
* 2nd place: 1,000 USDC

## Bounty 2 - Improve your dApp’s UX with Batching or Gasless Transactions

Moonbeam has a variety of precompiles, such as the [batch precompile](https://docs.moonbeam.network/builders/pallets-precompiles/precompiles/batch/) and [call permit precompile](https://docs.moonbeam.network/builders/pallets-precompiles/precompiles/call-permit/) that offer powerful functionality to builders which can vastly improve the UX for dApp users. The [batch precompile](https://docs.moonbeam.network/builders/pallets-precompiles/precompiles/batch/) allows you to combine multiple smart contract calls into a single transaction. These groupings can be atomic or nonatomic at your discretion. 

The quintessential example of a batched transaction that simplifies the UX for end users is batching together the approval and swap transactions for DEX. Rather than a user having to confirm an approval transaction and a swap transaction, the user can confirm a single batched transaction that executes both within the same block. In this case, you’d want the batch transaction to be atomic, because there’s no need to approve an ERC-20 allowance if the swap reverts. 

Another possibility is to use the [Call Permit Precompile](https://docs.moonbeam.network/builders/pallets-precompiles/precompiles/call-permit/). One of the most frustrating experiences for a user new to Web3 is acquiring gas to pay for transactions. You can substantially improve your dApp’s UX by eliminating the requirement that the user hold the native token for gas. Moonbeam’s call permit precompile enables you to do exactly that - with it, you can dispatch any transaction in a gasless manner which can be relayed by Biconomy.

To be eligible for this bounty, your dApp should have at least some smart contract logic deployed to Moonbeam or Moonbase Alpha. Secondly, it must utilize the batch precompile or the call permit precompile (or both) to provide any non-trivial functionality to your dApp. 

#### Rewards:
* 1st place: 4,000 USDC 
* 2nd place: 1,000 USDC

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

## Resources for Bounty 2 - Improve your dApp’s UX with Batching or Gasless Transactions

### Written Tutorials
* [Interacting with the Batch Precompile](https://docs.moonbeam.network/builders/pallets-precompiles/precompiles/batch/)
* [Access the Batch.sol Solidity Interface Here](https://github.com/PureStake/moonbeam/blob/master/precompiles/batch/Batch.sol)
* [Interacting with the Call Permit Precompile](https://docs.moonbeam.network/builders/pallets-precompiles/precompiles/call-permit/)
* [Access the CallPermit.sol Solidity Interface Here](https://github.com/PureStake/moonbeam/blob/master/precompiles/call-permit/CallPermit.sol)

### Video Tutorials
* [Batch Precompile Part 1 - Introduction and Methods of the Batch Precompile](https://drive.google.com/file/d/1E2mpHvuCyb0svFg5dFe5EeYrs4HzLIiU/view?usp=sharing)
* [Batch Precompile Part 2 - Batching Transfers and Contract Calls](https://drive.google.com/file/d/1xy9ovrvkWuU5z4VwnFoZMDUAQhcJDZAg/view?usp=sharing)
* [Call Permit Precompile Part 1 - Introduction to the Call Permit Precompile](https://drive.google.com/file/d/13-G2hp1AN0lFmXLP0t_J254cHoYmaK_w/view?usp=sharing)
* [Call Permit Precompile Part 2 - Using CallPermit.sol to Dispatch a Call](https://drive.google.com/file/d/1EjWmDlBei2rRW5O7OO06Y2PGty5I_QRy/view?usp=sharing)

## General Resources

### Building a web app as part of your DApp? Start here 
* [ScaffoldEth](https://github.com/scaffold-eth/scaffold-eth) is a fantastic way to quickly spin up a React frontend that connects to your solidity smart contract. [Learn how to use ScaffoldEth with Moonbeam here](https://docs.moonbeam.network/builders/build/eth-api/dev-env/scaffold-eth/). 
* [Configure your preferred developer environment for Moonbeam](https://docs.moonbeam.network/builders/build/eth-api/dev-env/)
* [Use JS libraries like Ethers.js or Web3.js to integrate smart contract functionality into your webapp](https://docs.moonbeam.network/builders/build/eth-api/libraries/)

### Office Hours
Office hours are a great place to get help or feedback on your idea. *Note*: You can stop by the Moonbeam Booth anytime for help! These office hours are simply meant to provide a dedicated timeslot with availability of multiple Moonbeam team members. They are held at the Moonbeam Booth (Devtopia, Booth R) at the following times:
* Thursday (3/2) 11:00 am -12:00 pm MST
* Friday (3/3) 2:00 - 3:00 pm MST 
* Saturday (3/4) 5:00 - 6:00 pm MST

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