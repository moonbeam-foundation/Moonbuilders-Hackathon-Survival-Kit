# Moonbuilders Hackathon Survival Kit
Everything you need to get started building on Moonbeam, optimized for builders

![Banner Image](https://i.ibb.co/GnvpLcw/Featured-Images-4.png)

## What's Moonbeam?
Moonbeam is a platform for cross-chain connected applications that unites assets and functionality from many blockchains. Moonbeam is a fully Ethereum-Compatible Layer-1 blockchain (also known as a *Parachain*) on Polkadot.

## What's Polkadot?
Polkadot is a Layer 0 protocol designed to enable interoperability amongst the hetereogenous L1 blockchains that run on top of it. Polkadot provides the security, governance, and cross chain communication to enable seamless interoperability between parachains, or L1 blockchains that serve various specialized use cases. Moonbeam is a Polkadot parachain. 

## Meet the Networks (and block explorers)
* **<a href="https://moonscan.io/" target="_blank">Moonbeam</a>** - Mainnet, operating as a parachain on the Polkadot Relay Chain
* **<a href="https://moonriver.moonscan.io/" target="_blank">Moonriver</a>** - Canary network, or experimental mainnet. Moonriver is a parachain on the Kusama Relay Chain
* **<a href="https://moonbase.moonscan.io/" target="_blank">Moonbase Alpha</a>** - The public testnet for Moonbeam and Moonriver. 

## Moonbase Alpha Faucet
* You can get [DEV testnet tokens here](https://apps.moonbeam.network/moonbase-alpha/faucet/).
* You can make a swap for [testnet cross chain assets here](https://moonbeam-swap.netlify.app/#/swap).
* If you need more tokens in bulk for testing purposes don't hesitate to reach out to us in [Discord](https://discord.gg/moonbeam).


## 🎥 Introducing Moonbeam's 2022 MIT Bitcoin Expo Bounties
In the below video, Kevin introduces the 2022 Bounties including the challenge descriptions, expectations, and prizes.

[![Introductory Video](https://img.youtube.com/vi/Vbz3ONOyFmg/hqdefault.jpg)](https://youtu.be/Vbz3ONOyFmg)

### Challenge #1: Build an App with [Moonriver's Chainlink Price Feeds](https://docs.moonbeam.network/builders/integrations/oracles/chainlink/)
Chainlink price feeds are a critical piece of infrastructure of many DeFi applications. The Moonbeam Docs Site has detailed documentation on how you can [easily integrate chainlink price data into your application](https://docs.moonbeam.network/builders/integrations/oracles/chainlink/). The challenge here is simply to use Chainlink price data as a valuable component of your application. You can also checkout the below video guide showing you how to interact with Chainlink price feeds through [AggregatorV3Interface.sol](https://github.com/smartcontractkit/chainlink/blob/develop/contracts/src/v0.8/interfaces/AggregatorV3Interface.sol):

#### 🎥 How to Interact with Chainlink Price Feeds
In the below video, you'll learn how to fetch price data from Chainlink price feeds on Moonriver and Moonbase Alpha (the public testnet).

[![Chainlink Price Feeds](https://img.youtube.com/vi/esmeaoQzj_8/hqdefault.jpg)](https://youtu.be/esmeaoQzj_8)

#### Rewards:
* 1st place: 1,000 USDT 
* 2nd place: 500 USDT

#### Evaluation Criteria:
* Does the application correctly integrate Chainlink price feed data?
* Is the price feed data a valuable component of the dapp? Why is the price data needed?
* Is the dApp deployed to Moonbase Alpha (the testnet) or Moonriver?

### Challenge #2: Build an App that Displays the Supply of Cross Chain Assets on Moonriver
[XC-20s](https://docs.moonbeam.network/builders/xcm/xc20/) are Substrate assets that can be transferred cross chain via XCM that also conform to ERC-20 standards. [xcKSM](https://moonriver.moonscan.io/token/0xffffffff1fcacbd218edc0eba20fc2308c778080), or KSM migrated from the Kusama Relay Chain, was the first XC-20 to launch on Moonriver. The challenge here is to build an app that shows cross chain asset statistics, including the supply of each cross chain asset on Moonriver. Under the network -> Assets tab of PolkadotJsApps, you can find a list of all [XC assets on Moonriver and their current supply on Moonriver](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Fmoonriver.api.onfinality.io%2Fpublic-ws#/assets). You can also [fetch this data programmatically via the Polkadot API](https://docs.google.com/document/d/14yFV_vYCdgdDIy46OH6ZQwSBHy3ImrZpF9FGPFVWZXE/edit?usp=sharing). The best projects will feature additional statistics, such as supply on origin chain, total outstanding supply, % of supply migrated to Moonriver, etc. 

## Helpful Resources
* Moonbeam Documentation Site: https://docs.moonbeam.network/ 
* Moonbuilders Academy: https://academy.moonbeam.network/ 
* Developer Hub at Discord: https://discord.gg/moonbeam
