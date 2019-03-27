---
date: 2017-01-14 14:45:05
title: Daily Duties & Responsibilities
description: Daily Duties & Responsibilities
type: Document
category: 1-about
---
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
