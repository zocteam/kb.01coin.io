/*
Title: What to Do When Your 01coin Node Goes Out of Sync
Sort: 4
ShowOnHome: true
*/

In order to participate in network consensus, your 01coin node must remain in sync with the rest of the network. Your node is pretty good at taking care of that all on its itty-bitty lonesome, but sometimes things go wrong. Sometimes a single node can get stuck, and sometimes a big chunk of the network can hive itself off onto a sidechain.

Following these simple steps laid out in this quick reference guide will help you get your 01coin node back in sync, and smack a smile back on your face just like Justin Timberlake circa 1997.

![](https://cdn.steemitimages.com/DQmcVefF5WAQHHmCbivpeoPH45mWckGNq8aqiBVFp8bGRnE/image.png)
<p style="text-align: center;">Justin Timberlake's 01coin node is NSYNC</p>

1.) The first step when performing *any* wallet maintenance whatsoever is to backup your wallet. You do this by going to File > Backup Wallet, and then saving it to a location you'll be able to remember later.

![](https://cdn.steemitimages.com/DQmeZJyjYsMvS8J8W7ZkUNx1cbk4fmMViCvaouhm6B9UkaL/image.png)

2.) Next, close your wallet by going to File > Exit. Wait for the wallet to fully shut down.

3.) Navigate to your 01coin data directory. The default location for this directory depends on your operating system:

- Windows: %appdata%\ZeroOneCore\
- Mac OS X: ~/Library/Application Support/ZeroOneCore/
- Linux: ~/.zeroonecore

4.) Make sure to keep a copy of your backups folder, wallet.dat, zeroone.conf and masternode.conf files. Delete everything else. We say it again: **DO NOT** delete your backups folder, wallet.dat, zeroone.conf or masternode.conf files. 

5.) Download and extract the latest 01coin bootstrap.dat file from [here](https://github.com/zocteam/zoc-bootstrap) and save it into your 01coin data directory. Once done, your data directory should look a little something like this:

![](https://cdn.steemitimages.com/DQmV6TyBbLr1UF5QoUXYDX5Rnrzpo4sj85eW4rKJeX4L4nu/image.png)

6.) Restart your 01coin wallet and wait for it to index and process the blocks in the bootstrap file (it will take some time).

![](https://cdn.steemitimages.com/DQmaRfkPZ7uXmjp5HvHNndF9E3RKUtXp3Lai55tp2UBcZ6u/image.png)

7.) ...

8.) Profit just like Justin Timberlake circa 2019!

![jtmoney.jpg](https://cdn.steemitimages.com/DQmdfkqDaCvDhKmLdWX3xV28MBj8158ES7psoS45eHuwkoC/jtmoney.jpg)
