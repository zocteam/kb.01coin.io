/*
Title: Disabled Premine
Sort: 2
ShowOnHome: true
*/

![](https://github.com/deadthings/kb.01coin.io/raw/contrib/Official%20Documents/DisabledPremine01.png)

# Details Concerning 01coin’s Disabled Premine

By: deadthings
Date: May 3, 2018

Prior to the release of the 01coin 0.12.1.6 wallet, the zocteam had to be deliberately cagey about how exactly we planned to disable the premine. This was to ensure that the original development team did not try to spend the premine before we could implement the changes to the code that would disable it. In fact, one of the members of the original development team contacted us shortly before the wallet release, and did say “We can behave in a cat-and-mouse way…” regarding the potential for moving the premine around before any blocking mechanism had a chance to be implemented. 

Naturally, then, our silence regarding the details of our solution led to many unanswered questions from the community. This document aims to answer some of those questions. Our hope is that this will help improve the overall transparency of the 01coin project and may provide future guidance for other would-be developers looking to takeover a coin from a negligent or malicious development team on behalf of the community and address the issue of the premine without having to fork or swap the network.

Fortunately, one concerned and dedicated member of the 01coin community named TheHiman posed many good and challenging questions of the zocteam in a series of direct messages. While much of the content of those questions is highly technical in nature, I would like to take this opportunity to respond publicly to a few of the questions specifically regarding the premine. Please note that the questions as posed below are not verbatim quotations; they have been edited for clarity and length, but the pith and meaning of each has been maintained.

--

**Q:** I see how you’ve patched the code to disable the premine. Are you sure that this patch is really consensus-checked too? It must be bulletproof.

**A:** Yes, the code is consensus-checked at every transaction. Still, the possibility remains for a network actor to modify their client software and attack the network with transaction attempts from a disabled address. However, because the rest of the network, including regular wallets, pools and masternodes are unified, these transaction attempts will always be refused as invalid. If there are other nodes on the network that accept these transaction attempts while the rest of the network rules them as invalid, then those nodes are automatically dropped from the network for non-consensus. This is why many people who had not yet updated their wallets or masternodes by the time the old devs did unsuccessfully try to spend the premine on April 18 were dropped from the network and stopped receiving rewards. 
 
For reference, the pertinent code can be found at lines 1025 to 1041 of main.cpp in the current master branch.

![](https://github.com/deadthings/kb.01coin.io/raw/contrib/Official%20Documents/DisabledPremine02.png)

**Q:** The most important problem is that users can continue to use old wallets that confirm transactions from the disabled premine address. You must enforce wallet/chain version number so that old wallets must be disconnected and users are forced to upgrade.

**A:** This was a point of considerable discussion and debate among the zocteam prior to launch. We did indeed consider implementing a protocol version increase so that the network would immediately refuse connections to outdated peers. We also considered implementing a change in masternode collateral (from 1,000 coins to 1,001 coins) to instantly break all masternodes ensuring only up-to-date ones held by the zocteam and a few others who were notified prior to launch (such as shared masternode service providers) would be online, thus ensuring the entirety of the network – albeit a significantly smaller network than before – would be running updated wallets. 

It was concluded that “ninja-launching” like this would be unfair to the members of the 01coin community who would necessarily lose rewards as a result. Instead, we wanted to give the community a bit more time to update. We accomplished this by making sure a) that all online pools generating Proof of Work blocks were updated prior to public launch. Thus, no newly generated block would approve a transaction from the blocked premine address. Also, through the behind-the-scenes cooperation of many large masternode owners, we were able to have approximately 60 to 80 masternodes updated prior to launch. While this was only a minority of masternodes online at the time, it was enough to support the Proof of Work consensus. In this manner, a ninja (hard) release could be avoided and all 01coin network actors would have some time to update before the old nodes would fall offline. 

It turned out, of course, that the old developers put 01coin’s network consensus to the test almost immediately when they tried to spend the premine within only a few hours of public release of v0.12.1.6. This action knocked many of the old nodes offline, effectively impacting the network in a similar way that protocol enforcement would have. But the point is, immediately disabling old wallets and masternodes was not necessary to achieve overall network consensus. Having said that, a protocol version increase is planned for a future release in order to help keep the network up-to-date.

**Q:** Users need to know that the chain will fork if they do not upgrade their wallet. It is best instead to announce a date of a mandatory update and then enforce only new wallets on the network.

**A:** As described above, the update could not be pre-announced with a specific date because then we would most likely be forever stuck playing a game of cat-and-mouse with the old devs as they kept moving the premine from one address to another, or worse, breaking it up into a myriad of smaller addresses. The zocteam had to do a balancing act between being open and transparent with the community about our intentions, while retaining the element of surprise when it came to making sure that the premine would stay put. 

When the old devs attempted to spend their premine immediately following public release of the new wallet, it did in fact rupture the 01coin blockchain. While all new wallets refused the transaction, old wallets were split essentially 50/50 as to whether they confirmed or denied the transaction. But as stated earlier, the presence of new wallets on the masternode network and in the pools necessarily tipped the odds in favour of a transaction refusal. The network then dropped all nodes that had approved the transaction for “bad behaviour” – thus essentially creating a side chain that eventually died off due to a lack of block generation without any Proof of Work network hash. When wallet owners on the side chain realized they had stopped receiving rewards, they started the process of updating their wallets. Today, the masternode network is stronger than ever, as shown by this chart from masternodes.online: 

![](https://github.com/deadthings/kb.01coin.io/raw/contrib/Official%20Documents/DisabledPremine03.png)

At this point, I invite members of the community to pose any additional questions you may have regarding the disabled premine or anything else, for that matter. It is our goal to be completely transparent in our development of 01coin as we work towards implementing a Decentralized Autonomous Organization based on Chain of Trust theory and 100% community governance. Our next step towards achieving this will be sharing our development planning board publicly. We are currently using Trello for this, and if it does not offer observer functionality we may have to switch platforms or find an otherwise suitable solution. Rest assured, though, we are actively looking into this so that we can make the project as transparent as possible as soon as possible. 

Thank you for being a part of the 01 community, where all members are contributors! With 01coin, the future is in your hands.

Regards, 
deadthings, on behalf of the zocteam
