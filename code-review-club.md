# Code Review Club

ZENON WIKI Code Review Club is a weekly discussion group for the Zenon community to learn about code related to Zenon and Bitcoin.

Discussion is generally conducted on Thursdays at 1700 UTC in the [#code-review:zenon.wiki](https://matrix.to/#/#code-review:zenon.wiki) matrix room.

Material, discussion questions, and sometimes exercises will be posted on Fridays the week prior. While the review club will not be a line-by-line walkthrough of the material and code, we understand that not everyone is always able to read the material ahead of time

Meetings will be an hour long and focused on the discussion questions and any results from exercises. Participants are expected to follow the [Zenon Code of Conduct](https://zenon.wiki/code-of-conduct.html) at all times.

For the convenience of the community, read-only bridges will be provided where possible. [Telegram](https://t.me/zenon\_wiki\_code\_review\_club)

If you are the maintainer of a Zenon related project and would like host a session please contact @george:zenon.wiki

### Upcoming meetings

#### #4: Addresses

**Overview**

Addresses are one of the fundamental concepts for any network.\
This week we'll discuss Zenon's addresses, its heritage, and its implications.

**Time & Place**

2022-02-24 1700 UTC

[#code-review:zenon.wiki](https://matrix.to/#/#code-review:zenon.wiki)

**Material**

* [go-zenon: address.go](https://github.com/zenon-network/go-zenon/blob/master/common/types/address.go)
* [btcd: bech32.go](https://github.com/btcsuite/btcd/blob/master/btcutil/bech32/bech32.go)
* [bip-0173](https://github.com/bitcoin/bips/blob/master/bip-0173.mediawiki)
* [bip-0350](https://github.com/bitcoin/bips/blob/master/bip-0350.mediawiki)

**Discussion Questions**

* What dependencies does the code for zenon addresses have?
* What character set do zenon addresses use? - Any interesting spellings you notice?
* What relationship do zenon addresses have with bitcoin?
* What implications does this have?
* What is the underlying type of an address?
* How many bytes are zenon addresses?
* What does the first byte of an address signify?
* Why do all zenon addresses begin with z1q?
* What kind of cryptographic primitives are used for zenon addresses?

### Previous meetings

\#3: Ledger API: Show and Tell

\#1,#2: Ledger API: go-zenon & znn\_sdk\_dart
