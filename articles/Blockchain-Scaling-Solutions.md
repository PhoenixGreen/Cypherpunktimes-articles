| Content | Description |
|---|---|
| Title               | The Blockchain Scaling Solutions & Trade-offs |
| Author              | Phoenix Green |
| Featured text       | FIXME |
| CT link             | FIXME |
| Publish date        | YYYY-MM-DD FIXME |
| Ai checks (https://www.zerogpt.com) | Score = 0% |

| Social Media | Links |
|---|---|
| YouTube link        | FIXME |
| Podcast link        | FIXME |
| Reddit Link         | FIXME |
| Bison Relay Post    | TITLE |
| Twitter full video  | FIXME |

| CT tweet            | FIXME |
| YouTube tweet       | FIXME |
| Twitter clip 1      | FIXME |
| Twitter clip 2      | FIXME |


## Thesis statement

Blockchain technology is slow, inefficient and inconsistent. Many would argue, this is to preserve the highest levels of security whilst aiming to maintain a peer to peer decentralised network. But can this be improved to give users the best of both worlds, A fast, efficient blockchain that is also a secure, decentralised, peer to peer network?


## Pre-discussion, research and questions

* What problems are scaling solutions trying to solve? e.g. Volume, Speed & cost
* What are the trade-offs for these solutions?
* Why do these problems and trade-offs exist?
* What are some of the scaling solutions currently being explored?


---
--- ARTICLE GOES BELOW THIS POINT ---

---

# Blockchain Scaling Solutions & Trade-offs

It’s not uncommon, for a crypto user to come across a project that announces they have developed a solution that solves the blockchain transaction problem. Most of which will display a series of arguments as to why their solution is better than others. But more often than not, they fail to disclose the areas their solution fails short in.

Let’s explore blockchain scaling and the methods used to increase transaction volume and speed, whilst decreasing congestion and cost. We’ll also discuss what users should look out for when researching the latest, greatest blockchain solutions. Understand the long-term implications being produced by these methods and trade-offs will help evaluate the path a project is likely to follow. For example, whether it will end up being a centralised datacenter-driven blockchain or able to maintain a peer to peer decentralised infrastructure.

To my knowledge, the first time blockchain technology had to deal with the transaction scaling difficulty was during the 2017 block size wars, which introduced the “Bitcoin Cash” hard fork. The reason for this hard fork was to introduce larger blocks, so Bitcoin could process more transactions per second. This hard fork would have taken the original block size from 1 MB per block to 4 MB, with the likelihood of increasing this further in the future as needed. The opposition to this hard fork highlighted the blockchain bloating that would be caused by increasing the block size. Fast-forward to today, and we can see this effect playing out in many blockchain projects, including Ethereum and Solana. Bitcoin (BTC) also hasn’t completely avoided this issue.

## Transaction scaling — Volume, Speed & cost

The three desirable features blockchain projects try to include in their design as they build their next-gen transaction infrastructure can be categorised into three areas, volume, speed, and cost:

Transaction volume: 
The holy grail for blockchain volume is to match the 100,000 transactions per second currently being achieved by VISA

Transaction speed:
How fast transactions can fully settle. One of the major downsides of blockchain projects like Decred and Bitcoin is how long it takes for a transaction to fully settle. The aim in this area of development is to get all transactions to fully settle in under one second.

Transaction cost:
And finally, the transaction cost or fees associated with processing a transaction. As a blockchain increases in popularity, it will start to witness block congestion. This in term pushes transaction fees up as people increase the fees they are willing to pay to get their transaction in the next block. The aim in this area is to maintain a transaction fee that is less than a penny, but the current benchmark is a single Atom / Satoshi (0.00000001 DCR).

## The transaction scaling trade-offs

As solutions are introduced they typically run into one or more unavoidable trade-offs, these include, centralisation, security, blockchain bloat, efficiency, and reliability.

* Centralisation — Reduced decentralisation due to the majority of users not being able to run the validating software and hardware needed
* Security — Reduced security and the need for increased trust, which is introduced through the techniques used to circumvent on-chain consensus or other mechanisms used that secure the blockchain
* Blockchain bloat — Is mostly unavoidable when a project aims to place all transactions on-chain whilst aiming for the 100,000 TPS target
* Efficiency — Being efficient with the data that is put on-chain and being efficient with how transactions are being processed
* Reliability — The more transactions you process, the harder it becomes to synchronise a peer to peer network. The reliability factor is how hard is it for an individual to stay in sync with the chain whilst validating up-to-date transactions.

## Why do these problems and trade-offs exist?

There are many scenarios for why these trade-offs exist, but the first thing that needs to be identified is that everything that happens on-chain has a data weight and a physical storage and creation cost. To maintain a peer to peer network, the majority of the participants need to store this data and remain connected to the network. We must get it out of our heads that everything is free or somebody else is going to do this for us. There is always a price to pay, and blockchain is no different. At some point in the future, individuals who want to remain sovereign will need to burden these expenses.

Producing data for a blockchain creates a footprint that will live on-chain, sometimes in defiantly. For example, an empty block and its header has a data weight, as does each and every transaction. An empty block will generally be larger than 194 Bytes. And an individual transaction will typically be 215 Bytes or larger. 

Once you understand this, you should be able to make some simple calculations regarding things like blockchain bloat and its effects of centralisation.

For example: If a blockchain produces a new block every second and only produces empty blocks, this will produce approximately 5 GB of data per year, of which full node operators have to process, verify and store long into the future. 

Calculation: 
* 1 block per second (194 B) x 60 seconds = 11,640 B per minute
* 11,640 B × 60 minutes = 698,400 B per hour
* 698,400 × 24 hours = 16,761,600 per day
* = 16.7616 MB per day
* 16 × 365 = 5,840 MB per year
* = 5.84 GB per year

## Scaling solution

It’s actually very impressive how many projects have and are trying to solve the transaction scaling problem. Some of the most popular scaling solutions include:

* Block size and time 0n-chain scaling
* Pruning and sharding mechanisms for on-chain scaling
* Layer 2 and side-chain scaling solutions
* The Lightning Network
* Global and local scaling

Depending on your requirements, you’ll probably prefer certain solutions to others. I’m currently leaning towards the Lightning Network for my preferred scaling option, but it’s also fair to say that others have their merits, which we’ll explore through this series.
