---
description: Information about the Wallets of Zenon Network
---

# Wallets

You can access the latest versions of both the Zenon Core Legacy Wallet and the S Y R I U S Network of Momentum Wallet at the bottom of the official Zenon Network page.&#x20;

[https://zenon.network](https://zenon.network)

### Alphanet Wallets

#### What is the Syrius Wallet** ?** <a href="what-is-the-syrius-wallet" id="what-is-the-syrius-wallet"></a>

The first public tests of the Network of Momentum began in 2021. These public tests were signalled with the release of the Syrius wallet. These initial versions of Syrius are fully functioning Beta versions of the Network of Momentum wallet where you can do everything you will be able to do on the Network of Momentum, but in a test phase. All the Zenon ZNN and Quasar QSR coins on Syrius wallet are test versions of the actual NoM coins and are not redeemable for real ZNN or QSR.

The Syrius Wallet will be the go-to wallet on the Network of Momentum once it transitions from the Testnet to the Alphanet.

#### When will cold wallet support be available? <a href="q-when-will-cold-wallet-support-be-available" id="q-when-will-cold-wallet-support-be-available"></a>

The implementation for cold wallet support is possible and can be developed after Alphanet launch.

#### Is there a Mobile Wallet for Zenon Network of Momentum?

There will be a mobile version of Syrius as well as community-built mobile wallets, which are in test phase. Nothing is released yet.

#### I would like to change the Node my Syrius wallet points to, how do I do that?

Go to Syrius ( make sure it's version 5.0 or later ) Go to the settings tab. Scroll down >> Bottom left /Node Management >> Add Node >> and put in the address of your new Node aggregator, an example is ' peers.zenon.wiki ' then click 'Confirm Node'.

### Legacy wallet

#### Zenon Network guide for the Legacy Wallet is here.

https://zenon.network/howto

#### Community Member guide for the Legacy Wallet is here.

https://crypto-iverson.medium.com/so-you-bought-znn-de91d97a2bcb

#### I downloaded the Legacy wallet but it didn’t make me create a recovery phrase, why? <a href="q-i-downloaded-the-legacy-wallet-but-it-didnt-make-me-create-a-recovery-phrase-why" id="q-i-downloaded-the-legacy-wallet-but-it-didnt-make-me-create-a-recovery-phrase-why"></a>

The legacy wallet doesn’t use recovery phases, if you back up a copy of your wallet.dat file ( File >> Backup Wallet>>Save As) it contains your private key.

#### I downloaded the Legacy wallet but it's taking a long time to sync, why? <a href="q-i-downloaded-the-legacy-wallet-but-it-didnt-make-me-create-a-recovery-phrase-why" id="q-i-downloaded-the-legacy-wallet-but-it-didnt-make-me-create-a-recovery-phrase-why"></a>

The Legacy wallet ( make sure it's version 1.6.5 ) is picking up over 2 years of blockchain data from other nodes - that's over 3GB of info. It should take a couple of hours depending on your connection and the Nodes. The green bar at the bottom disappears when it's done.

#### Where do I find the .dat backup of my Legacy Wallet on WIndows?

if you are on Windows, your Zenon Core wallet.dat is located at:

C:\Users\[username]\AppData\Roaming\znn OR C:\Users\[username]\AppData\Roaming\zenon

There’s a backup of your wallet in c:/users/**your username**/appdata/roaming/zenon

#### How do you get the private keys from legacy wallet? Is there a command?

Yes - Go to tools >> click on 'debug console'&#x20;

type: walletpassphrase "your walletpassphrase here"&#x20;

type: dumpprivkey "your znn pub address here"&#x20;

This will return the private key. You can copy/save it. Ensure you clear your clipboard afterwards.&#x20;

type: walletlock

There is a key for each of the addresses in the Core Wallet, so do the above for each address in your legacy wallet which contains ZNN.
