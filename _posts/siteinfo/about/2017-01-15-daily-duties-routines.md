---
date: 2017-01-14 14:45:05
title: Daily Duties & Routine
description: Daily Duties & Routine
type: Document
category: 1-about
---
**Daily Duties & Responsibilities**

*From Notary Node Operator team Chainmakers*

As a NN operator, you take part in securing all the coins and assetchains that secure themselves through delayed Proof of Work, or dPoW. There are many aspects to being a notary node operator, all with the goal to keep notarizations going 24/7.

Monitoring a Notary Node
A large part of being a NN operator is making sure your Notary Node is notarizing. There are many things that can (and will) go wrong, for which you need to set up tools to quickly see what is going wrong.

So, what does a notary need to track to keep notarizing?

Iguana
Notarizing is done through Iguana. Iguana runs as an application on a server, so the most important thing is to check whether Iguana is running, using a simple ping or special scripts.

Coin Management
The coins that are currently notarized, need to be running as well, since a transaction is done for every notarization.
In addition, this means that every coin must have enough funds to be able to do a transaction. Actual transactions are done in small amounts, but many coins have a notarization frequency of 10 blocks. Many small transaction amounts quickly drain your node's balance.

Whenever a new coin is accepted to be notarized, it is important to install the coin's daemon, synchronize the blockchain and set up Iguana to be able to notarize the newly added coin as swiftly as possible.

Coins often need updates. Being on call whenever a coin needs an update is an important task of a notary, especially when the update concerns the security of the node. A notify system exists when all notaries need to be notified quickly. All notaries are part of a notary group in Discord and Riot, the latter being used as a fallback if the Discord service is down.

Notaries are not always near a pc or laptop. Many have set up email services or Telegram bots to be notified of any downtime.

Responsiveness of a Node
For continuity's sake: making sure your node keeps notarizing as much as possible. This has an economic reason:
Each of the 64 nodes mine approximately 1500 KMD per month. Every year, 28 of the 64 best performing nodes get to keep their notary spot, and so they get to keep another year of rewards. It is therefore important to get as many notarizations as possible.

In addition to the previously mentioned things to monitor, a notary tries to keep all its coin wallets as light as possible. Wallet management, as the notaries call it, has keeping as few UTXOs as possible for each coin on the node as its primary goal.
Without getting too technical: it is important for a coin daemon to be able to offer an Unspent Transaction Output (UTXO) to the other notaries, since 13 of the 64 notaries participate in a single notarization.

The probability that your node participates in the next notarization is higher when your coin daemon can supply an UTXO very fast. In order to make this fast, the wallet must not contain too much history, since not only Unspent Transactions are stored in a wallet, but also Spent Transactions.

Scripts have been made that track the size of a wallet, or that periodically reset a wallet to keep the wallet as light as possible.

Another degree in which a node can perform better is to have a good network connectivity to all other nodes. There are many things that help connectivity, such as the physical location of a node or the internet settings that are specified in the node's network controller.

CLI Knowledge
All of this requires knowledge of Linux and being comfortable working with the Command Line. Installing a coin, synchronizing it, setting up the notary software, management of wallets, improving the node's connectivity to other nodes, cronjobs, monitoring; it's all part of a normal day in the life of a Notary Node Operator.

Helping Others
Although it is not necessary, it would be in a node's best interest to help the Komodo Platform and / or your fellow notaries as good as possible. Some examples of this are:

- Testing newly developed tech
- create tools that help the Komodo Platform forward
- write scripts for other notaries to use
- helping the devs to fix bugs

A notary can write their own tools, or use any of the tools that other notaries graciously made available. (see this repository)


*From Notary Node Operator team Komodo Pioneers*

The daily tasks and routine of a Notary Node Operator involves asking some odd questions.
- How long does listunspent take?
- How big is my wallet.dat file?
- Can I jump onto the console and work on fixing a problem for the next few hours?
- Do I have time to bug hunt?

The tasks range from:
- Ensuring that you’re not on a fork
- Checking you have UTXOs to spend (all funded by the network) for notarizations.
- Checking you have a responsive system
- Tuning your system so you are in agreeance with the rest of the network about which are the best performing nodes for this sequence
- Updating Komodo or any of the notarized chains when they have upgrades to their code base

The last point is the most important. Komodo’s Notary Node network is a secure functioning network of blockchains. Any weakness will be exploited.  Komodo cares about blockchain technology, whether it is from Komodo or from another project.

The usual sys admin tasks apply. Running several blockchain daemons and dozens of blockchains inevitably comes with some management tasks. It is a baptism of fire for the first 6 weeks, even if you’re already familiar with running full nodes.

Developing scripts to make managing your notary node easier is the primary goal in the first few months. There is a heterogenous method of maintenance amongst Notary Node Operators, with vanilla scripts that make some (but not all tasks) easy. 

When the scripts fail, what do you do? At that point, your node will not be participating in notarizations. It may not even be mining. The scripts may fail when you least expect it. If you've worked in a real-time telecommunications setting (audio or video), this is the type of troubleshooting that can be expected. Blocks sometimes don't arrive and the issue could lay anywhere in the 7-layers of tech or it could be some software bug.

The most important part is making sure your node is up. Has it mined a block in the last 100 blocks?  If yes, you probably have half a healthy node. If your node participated in a notarization in the last few minutes, you are 80% healthy. But are you performant?

The 80/20 rule certainly applies to the scoring system. The scoring goes on notarizations and notarizations are somewhat of a competition. If you have an 80% healthy node, you will likely be in the bottom 20% of the scoring for your region because there are a number of enthusiastic devops and sys admins in Komodo’s Notary Node network.

There will be some itch that needs scratching— constantly!  Will you itch, will you scratch?  How long will you itch before you scratch?  Some scratches will be multi-week, multi-failure attempts to optimize. This is the third season of notarizing. Not every itch has been scratched, and there will of course be new itches to scratch because we have Komodo, which is bleeding-edge technology. Komodo technology is not only for innovation, it's for performance.

The first season’s Notary Node Operators were different from second season’s.  In the second year, Komodo’s delayed proof of work (dPoW) security service was extended to non-Komodo blockchains. This means the second cohort of Notary Node Operators faced a new set of challenges that the first cohort didn’t need to deal with. 

The third season notaries are likely to need to manage resources better than second season notaries. As Komodo is innovating with cross-chain technology and clusters of chains, new maintenance tasks will need to be overcome to be a top-performing node.
