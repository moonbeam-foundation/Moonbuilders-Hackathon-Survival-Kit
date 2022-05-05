# Moonbuilders Hackathon Survival Kit
Everything you need to get started building on Moonbeam, optimized for builders

![Banner Image](https://i.ibb.co/w6fsn7h/Featured-Images-9.png)

## What's Moonbeam?
Moonbeam is a fully Ethereum-Compatible Environment on Polkadot. Moonbeam is much more than just an EVM implementation: it’s a highly specialized Layer 1 chain that mirrors Ethereum’s Web3 RPC, accounts, keys, subscriptions, logs, and more. The Moonbeam platform extends the base Ethereum feature set with additional features such as on-chain governance, staking, and cross-chain integrations.

## What's Polkadot?
Polkadot is a Layer 0 protocol designed to enable interoperability amongst the hetereogenous L1 blockchains that run on top of it. Polkadot provides the security, governance, and cross chain communication to enable seamless interoperability between parachains, or L1 blockchains that serve various specialized use cases. Moonbeam is a Polkadot parachain. 

## Meet the Networks (and block explorers)
* **<a href="https://moonscan.io/" target="_blank">Moonbeam</a>** - Mainnet, operating as a parachain on the Polkadot Relay Chain
* **<a href="https://moonriver.moonscan.io/" target="_blank">Moonriver</a>** - Canary network, or experimental mainnet. Moonriver is a parachain on the Kusama Relay Chain
* **<a href="https://moonbase.moonscan.io/" target="_blank">Moonbase Alpha</a>** - The public testnet for Moonbeam and Moonriver. You can get testnet tokens in the [#Moonbase-Faucet Channel on Moonbeam's Discord](https://discord.gg/9RYqehSWRv).

## Introducing Moonbeam's 2022 MIT Bitcoin Expo Bounties
[![Introductory Video](https://img.youtube.com/vi/Vbz3ONOyFmg/hqdefault.jpg)](https://youtu.be/Vbz3ONOyFmg)

### Challenge #1: Build an App with [Moonriver's Chainlink Price Feeds](https://docs.moonbeam.network/builders/integrations/oracles/chainlink/)
Chainlink price feeds are a critical piece of infrastructure of many DeFi applications. The Moonbeam Docs Site has detailed documentation on how you can [easily integrate chainlink price data into your application](https://docs.moonbeam.network/builders/integrations/oracles/chainlink/). The challenge here is simply to use Chainlink price data as a valuable component of your application. You can also checkout the below video guide showing you how to interact with Chainlink price feeds through [AggregatorV3Interface.sol](https://github.com/smartcontractkit/chainlink/blob/develop/contracts/src/v0.8/interfaces/AggregatorV3Interface.sol):

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

#### Rewards:
* 1st place: 1,000 USDT 
* 2nd place: 500 USDT

#### Evaluation Criteria: 
* At a minimum the project should consider at least one cross chain asset on Moonriver. Given the incremental nature of adding other assets, we expect submissions to attempt to list all cross chain assets (there are 10 at the time of writing). 
* Is the data being fetched programmatically? You can see the [current total supply information here for all of the cross chain assets on Moonriver](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Fmoonriver.api.onfinality.io%2Fpublic-ws#/assets). 
* The best submissions will integrate additional data such as total supply on origin chain, and other statistics of their choice.
* There’s not much time to design a pretty interface so we’re not expecting anything fancy. But a clean UI or innovative approach to displaying this information is a major plus. 

## Helpful Resources
* Moonbeam Documentation Site: https://docs.moonbeam.network/ 
* Moonbuilders Academy: https://academy.moonbeam.network/ 
* Developer Hub at Discord: https://discord.gg/moonbeam
