# How to run a node

Min requirements:

4cpu, 16GB ram (yes, 16GB ram MINIMUM is required to avoid swapping).

You will need to set up a VPS and connect via SSH.

This guide assumes you are using Ubuntu 21.04.

#### Step 1

Open firewall rules:

```
ufw allow 35995:35998/tcp
ufw allow 35995:35998/udp
```

#### Step 2

Create znn directory and download alphanet bundle

```
mkdir znn && cd znn
```

```
wget https://github.com/zenon-network/znn-bundle/releases/download/v0.0.1-alphanet/znn-alphanet-bundle-linux-amd64.zip
unzip znn-alphanet-bundle-linux-amd64.zip
```

#### Step 3

Run `./znn-controller` and select option `1) Migrate`

The required genesis and peers files can be downloaded from a decentralized peer-to-peer network, the Interplanetary File System.

* URL to download the initial peers:

```
https://ipfs.io/ipfs/QmeAUQkpoEMNRQ9SFcBV2kmRTXT3WLKAoMxvAtX2ErZubJ?filename=peers.json
```

* URL to download the Alphanet genesis:

```
https://ipfs.io/ipfs/QmVFyGWNt3Ph2mn9MoxZyTgjuMGSs2cDdqXP3B8Ri5AYY5?filename=genesis.json
```

#### Step 4

Run `./znn-controller` and select option `2) Deploy`

* Check the downloaded znnd node version: `znnd version v0.0.1`

#### Step 4

Configure znn to not use a pillar

* Edit `~/.znn/config.json` and set the producer to null by changing this:

```
"Producer": {
        "Index": 0,
        "KeyFilePath": "producer",
        "Password": "<REDACTED>",
        "Address": "<REDACTED>"
    }
```

to this:

```
"Producer": null
```

#### Step 5

Reboot your machine

```
reboot
```

Check status

* After node has rebooted, ssh in again and run:

```
cd znn
./znn-controller
```

Select option `3) Status`

It should say everything OK. You can check the logs with:

```
tail -f ~/.znn/log/zenon.log
```

#### Step 6

Connect to your node

You should be able to connect to your node using:

`ws://<your node ip>:35998`
