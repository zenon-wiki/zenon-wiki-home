---
description: Information about the Wallets of Zenon Network
---

# Wallets

Get the latest version of the S Y R I U S wallet here:

[Zenon Network Wallets download](https://zenon.network/#downloads)

### Syrius Wallet

The Syrius Wallet is the go-to wallet on the Network of Momentum. It's the command center for Delegating, Staking, Managing Tokens and Transacting.

**How do I get Plasma for sending fee-less transactions?**&#x20;

You need QSR to generate Plasma. In the Plasma tab in Syrius select the address you want to generate Plasma for, select the amount of QSR you want to fuse to that address ( minimum of 20 QSR recommended ) and click 'Fuse'. If you have no Plasma yet a PoW is done to fuel the process. The QSR can be unfused at any time with no loss. [More info here.](fees-and-plasma.md)

#### **I would like to change the Node my Syrius wallet points to, how do I do that?**

In the Syrius wallet go to the Settings tab. Scroll down >> Bottom left /Node Management >> Add Node >> and put in the address of your new Node aggregator, select it and click 'Confirm Node'. [More info here.](nodes-pillars-and-sentinels.md#nodes-syrius-and-the-network)

**Syrius is giving me an 'Unlock Failed' error.**

This is related to the node your wallet is connected to. Try quitting Syrius, disconnecting your computer from the internet, relaunching & opening Syrius and changing the node.

Learn how to change the Syrius node [here](nodes-pillars-and-sentinels.md#nodes-syrius-and-the-network).

Other community workarounds are linked [here.](../#community-resources)

#### **How do I delegate for rewards in the Syrius wallet?**

In the Pillar tab of Syrius you will find a list of active Pillars on the Network and their voting weight. You can select any of those by simply tapping 'delegate'. The entire balance of the address you're currently in is then delegated to that Pillar.&#x20;

If you want to delegate to other Pillars at the same time you need to move a portion of your funds across to another address within your wallet. Move to that address ( select it in the settings tab ) and then delegate those funds in that address to another Pillar. This is a good way to discover which Pillars are yielding greater returns.

You can find more info on Delegating and Staking [here.](staking-and-incentives.md)

**I'm creating a new Syrius wallet but can't make a password.**

Syrius requires that passwords contain the following.

A small letter&#x20;

A capital letter

A symbol like @#$¢

A number

**How do I backup my Syrius wallet?**

You do that in the Settings tab. Scroll down > bottom right 'Backup'

#### **When will cold wallet support be available?** <a href="#q-when-will-cold-wallet-support-be-available" id="q-when-will-cold-wallet-support-be-available"></a>

The implementation for cold wallet support is possible and can be developed after Alphanet launch.

#### **Is there a Mobile Wallet for Zenon Network of Momentum?**

There will be a mobile version of Syrius as well as community-built mobile wallets, which are in test phase. Nothing is released yet.

### Legacy wallet

#### **Guides for the Legacy Wallet are here.**

[Legacy wallet How-to](https://zenon.network/howto)&#x20;

[Crypto Iverson Guide ](https://crypto-iverson.medium.com/so-you-bought-znn-de91d97a2bcb)

#### **I downloaded the Legacy wallet but it didn’t make me create a recovery phrase, why?** <a href="#q-i-downloaded-the-legacy-wallet-but-it-didnt-make-me-create-a-recovery-phrase-why" id="q-i-downloaded-the-legacy-wallet-but-it-didnt-make-me-create-a-recovery-phrase-why"></a>

The legacy wallet doesn’t use recovery phases, if you back up a copy of your wallet.dat file ( File >> Backup Wallet>>Save As) it contains your private key.

#### **I downloaded the Legacy wallet but it's taking a long time to sync, why?** <a href="#q-i-downloaded-the-legacy-wallet-but-it-didnt-make-me-create-a-recovery-phrase-why" id="q-i-downloaded-the-legacy-wallet-but-it-didnt-make-me-create-a-recovery-phrase-why"></a>

The Legacy wallet ( make sure it's version 1.6.5 ) is picking up over 2 years of blockchain data from other nodes - that's over 3GB of info. It should take a couple of hours depending on your connection and the Nodes. The green bar at the bottom disappears when it's done.

#### **Where do I find the .dat backup of my Legacy Wallet on WIndows?**

if you are on Windows, your Zenon Core wallet.dat is located at:

C:\Users\[username]\AppData\Roaming\znn OR C:\Users\[username]\AppData\Roaming\zenon

There’s a backup of your wallet in c:/users/**your username**/appdata/roaming/zenon

#### **How do you get the private keys from legacy wallet? Is there a command?**

Go to tools >> click on 'debug console'&#x20;

type: walletpassphrase "your walletpassphrase here"&#x20;

type: dumpprivkey "your znn pub address here"&#x20;

This will return the private key. You can copy/save it. Ensure you clear your clipboard afterwards.&#x20;

type: walletlock

There is a key for each of the addresses in the Core Wallet, so do the above for each address in your legacy wallet which contains ZNN.

