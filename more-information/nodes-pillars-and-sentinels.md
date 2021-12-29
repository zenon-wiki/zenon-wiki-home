---
description: Information on launching and running Nodes Pillars and Sentinels.
---

# Nodes Pillars & Sentinels

### **A quick overview of the network structure**

The Network of Momentum runs on Validators called Pillars and Sentinels. **Pillars** are the strongest, most stable validators and require considerable investment to launch, ensuring they are run by teams that are serious about the protocol. **Sentinels** require decent investment but are easier to dismantle so they can be run by a broader base of actors. **Nodes** are communication clients that relay information between wallets and the network of Pillars and Sentinels and require no investment to launch personally, but public nodes that serve many wallets need to be beefier to handle the load.

### **Nodes, Syrius and the Network**

**The Syrius wallet is not a node**

This means that Syrius needs to link up to a node to find out what is happening on the Network. The node your Syrius wallet is linked up to is shown in the Settings tab, bottom left, under ‘Node Management’.

Your experience on the Network is directly linked to the speed of the node you’re connected to. Much like how your wifi connection dictates the Internet experience you're having on your phone.

If you’re piggy-backing off your neighbours wifi you’re sharing their bandwidth and at their mercy.&#x20;

If you find another neighbour's wifi with a better router your experience will improve.

If you have your own router connected to the network those contraints are removed.

**Running your own node improves the Network.**&#x20;

If fewer people rely on the centralised public nodes / routers then there will be less congestion and bottlenecks at those shared nodes. So starting up your own router improves your experience and then relieves congestion, improving others experience. A node is light on resources and requires little CPU power to run. It’s worth doing.

**What are the hardware requirements to run a node on my computer?**

Here are the requirements from the team to run a public node on the Alphanet. Private nodes do not require the high bandwidth.

​[Alphanet Node Requirements.​](https://testnet.znn.space/#!requirements.md)

**I want to run a node locally on my own machine to speed up the network. How can I do that?**

You do not need ZNN or QSR in your wallet to run a node.

Official and Community guides are linked[ here.](../getting-started.md#run-your-own-node-if-you-can)

**I would like to change the Node my Syrius wallet points to, how do I do that?**

In the Syrius wallet go to the Settings tab. Scroll down >> Bottom left >Node Management >> Add Node >> Enter the address of your new node (examples below) then click 'Confirm Node'. Make sure it's selected and exit.

**Community RPC Nodes:**

ws://chadasscapital.com:35998

ws://nodes.zenon.place:35998

ws://node01.nodez.space:35998&#x20;

ws://node02.nodez.space:35998&#x20;

ws://node03.nodez.space:35998

#### **If you have the "Unlock Failed" problem in your Syrius wallet try these workarounds:**

["Error Unlock Failed"](https://medium.com/@sirajarab/syrius-wallet-error-unlock-failed-b7b9cc627574) Syrius wallet fix by Siraj

["Error Unlock Failed"](https://medium.com/@rufusizthebezt/how-to-get-around-the-error-unlock-failed-on-syrius-wallet-acf074d3e63e) Syrius wallet fix by Rufus

### **Pillars and Sentinels**

**Are there any guides for deploying Pillars and Sentinels on the Network of Momentum?**

Zenon Network has added a Pillar deployment tutorial [here](https://github.com/zenon-network/znn-bundle).

Community Member SultanOfStaking has a Github focussed on this [here.](https://github.com/sultanofstaking?tab=repositories)

**Why are Pillars and Sentinels so expensive?**

The Network of Momentum probably wouldn’t perform very well if nodes didn’t have stable uptimes and could join/leave at will. This is currently an issue with Lightning and why it ends up being more centralized than we would like. High collateral is skin in the game to prevent that. The high price of buy-in also constitutes as COLLATERAL, meaning possible punitive actions for bad behaviour. Especially when we start talking about BTC interoperability.

Having a stable set of nodes is important for each step of a transaction. Every transaction has to be sent to a sentinel who then has to send to other sentinels before sending to a pillar. Pillars use virtual voting for consensus which also need a relatively stable voting set.

The NoM is not like BTC where we can randomly send to any node and receive blocks every 10 minutes. Momentums are much faster.

**How do I reclaim ZNN & QSR from a spawned, but undeployed Sentinel?**

Make sure you have downloaded the Syrius Bundle and that znnd and znn-cli are in the same folder as your Syrius Wallet. Then go to the folder they are in and hold the shift key and right click your mouse. Select "Open Powershell Window Here" Then type: ./znn-cli start znnd

then type: ./znn-cli enableRPC

then type: ./znn-cli resync select "Y"

then type: ./znn-cli start znnd

then type: ./znn-cli frontierMomentum

keep doing this every few minutes until it catches up to momentum on Explorer

when its caught up type: ./znn-cli sentinel.list --keyStore z1qz8tylu88et6ffy227pw8gak5qvn5awg35l96x --passphrase yourComplexPassphrase

but use your address

get your sentinel ID from list.

then type: ./znn-cli sentinel.revoke 3577d585df05a354fbe08ed58d4e7a3e718ce18b399d46f9f81d96687b608537 --keyStore z1qz8tylu88et6ffy227pw8gak5qvn5awg35l96x --passphrase yourComplexPassphrase

but use your sentinel ID and address instead of example here.

that should deposit tQSR and tZNN back in your wallet
