---
description: Information on Funding, Launching and Maintaining Pillars
---

# Pillars & Sentinels

#### I am interested in running a node on the Alphanet. Are there requirements or specifications for what is required in terms of hardware capabilities? <a href="q-i-am-interested-in-running-a-node-on-the-alphanet-are-there-requirements-or-specifications-for-wha" id="q-i-am-interested-in-running-a-node-on-the-alphanet-are-there-requirements-or-specifications-for-wha"></a>

Yes the node hardware requirements have already been published for the Testnet. It doesn’t mean Alphanet’s will be the same, but you could imagine these as minimum requirements. You can easily achieve these requirements with a cloud vps.&#x20;

https://testnet.znn.space/#!requirements.md

#### Are there any guides for deploying Nodes on the Network of Momentum?

Yes a Community Member has created some here:

https://github.com/sultanofstaking

#### Why are Pillars and Sentinels so expensive?

The Network of Momentum probably wouldn’t perform very well if nodes didn’t have stable uptimes and could join/leave at will. This is currently an issue with Lightning and why it ends up being more centralized than we would like. High collateral is skin in the game to prevent that. The high price of buy-in also constitutes as COLLATERAL, meaning possible punitive actions for bad behaviour. Especially when we start talking about BTC interoperability.

Having a stable set of nodes is important for each step of a transaction. Every transaction has to be sent to a sentinel who then has to send to other sentinels before sending to a pillar. Pillars use virtual voting for consensus which also need a relatively stable voting set.

The NoM is not like BTC where we can randomly send to any node and receive blocks every 10 minutes. Momentums are much faster.

#### How do I reclaim ZNN & QSR from a spawned, but undeployed Sentinel?

Make sure you have downloaded the Syrius Bundle and that znnd and znn-cli are in the same folder as your Syrius Wallet. Then go to the folder they are in and hold the shift key and right click your mouse. Select "Open Powershell Window Here" Then type: ./znn-cli start znnd

then type: ./znn-cli enableRPC

then type: ./znn-cli resync select "Y"

then type: ./znn-cli start znnd

then type: ./znn-cli frontierMomentum

keep doing this every few minutes until it catches up to momentum on Exploror

when its caught up type: ./znn-cli sentinel.list --keyStore z1qz8tylu88et6ffy227pw8gak5qvn5awg35l96x --passphrase yourComplexPassphrase

but use your address

get your sentinel ID from list.

then type: ./znn-cli sentinel.revoke 3577d585df05a354fbe08ed58d4e7a3e718ce18b399d46f9f81d96687b608537 --keyStore z1qz8tylu88et6ffy227pw8gak5qvn5awg35l96x --passphrase yourComplexPassphrase

but use your sentinel ID and address instead of example here.

that should deposit tQSR and tZNN back in your wallet
