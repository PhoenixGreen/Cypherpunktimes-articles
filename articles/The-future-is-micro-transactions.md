| Content | Description |
|---|---|
| Title               | The future is micro transactions |
| Author              | Phoenix Green |
| Featured text       | Blockchains that are not preparing for micro transactions have failed to understand what happens at scale. |
| CT link             | https://www.cypherpunktimes.com/the-future-is-micro-transactions-the-lightning-network/ |
| Publish date        | Feb 28, 2024 |

| Social Media | Links |
|---|---|
| YouTube link        | https://youtu.be/FY2lvgAllnA |
| Podcast link        | https://podcasters.spotify.com/pod/show/cypherpunktimes/episodes/The-future-is-micro-transactions---The-Lightning-Network-e2gcv8c/a-ab0tusr |
| Bison Relay post    | Title: The future is micro transactions |
| Reddit link         | https://www.reddit.com/r/decred/comments/1b29cnf/the_future_is_micro_transactions/ |
| CT tweet            | https://x.com/cypherpunktimes/status/1762867011657371932 |
| YouTube tweet       | https://x.com/DecredSociety/status/1762868086200308016 |
| Twitter full video  | FIXME |
| Twitter clip 1      | https://x.com/DecredSociety/status/1762901109616590857 |
| Twitter clip 2      | FIXME |
| Matrix post         | Promote your main tweet in "DCR Social Media" channel (DONE) |


## Thesis statement

Blockchains that are not preparing for micro transactions have failed to understand what happens at scale. What does a blockchain look like when it's processing tens of thousands of transactions per second?

* What are micro transactions, and why do they matter?
* When you take micro transactions to scale, what are things that need to be considered?
* How does the Lighting Network deal with these considerations?
* Why is the future of blockchains micro transactions?


---
--- ARTICLE GOES BELOW THIS POINT ---

---

## Title: The future is micro transactions

Excerpt: Blockchains that are not preparing for micro transactions have failed to understand what happens at scale. 

Part of the scaling debate is the knowledge that at some point in the near future, a large majority of all transactions conducted on blockchains will be micro transactions. These will likely be in the hundreds of thousands per second, this is in direct comparison to what is already being achieved by traditional banking services like Visa, and Mastercard. 

## What are micro transactions, and why do they matter?

A micro transaction is an amount that can be as low as a single unit, for instance, on Decred and Bitcoin this is a single atom or satoshi 0.00000001. 

When you consider that most on-chain transactions have a mining fee greater than 1000 units, this is extremely difficult to achieve. For instance, if I sent one unit on the Decred blockchain, it would cost me approximately 2000 units to process this transaction.

This fact alone makes on-chain micro transactions undesirable. Paying a 2000% markup for a single transaction is unacceptable. When you start to factor in other trade-offs including blockchain bloat, you’d be forgiven for thinking, this doesn’t work! 

But just incase this point hasn’t sunk in, let’s see what this looks like at scale.

## When you take micro transactions to scale, there are a few things that need to be considered:

Firstly, the aim is to be peer to peer. This means the blockchain has to be small and efficient, so the majority of users can run full nodes or SPV wallets. Secondly, you need to be able to process thousands of transactions per second at the cost of a single unit or less.

**Blockchain Bloat**
Tens of thousands of transactions per second will have an estimated minimum weight of approximately 1 TB per day. Data centres will be the only ones able to run the blockchain network, bringing an end to the peer to peer functionality.

**Cost**
On-chain micro transactions is prohibitively expensive, either through the rising congestion fees or due to the mining fees being greater than the amount being sent. If a blockchain goes down the route of larger blocks, mining fees will remain lower for longer. To maintain this, at the scale of one hundred thousand transactions per second, you’d need a minimum block size of approximately 6 GB.

Transaction weight Calculation:
* 1 transaction = approx 215 Bytes, 0.215 KB, 0.000215 MB
* 2000 transactions = 0.43 MB 
* 100,000 transactions = approx 21.5 MB per second
* 21.5 MB x 60 seconds = 1,290 MB, 1.29 GB per minute
* 1.29 × 5 minutes = 6.45 GB per 5-minute block
* 6.45 × 12 blocks = 77.4 GB per hour
* 77.4 GB x 24 = 1,857.6 GB, 1.857 TB per day

**Speed**
Most blockchains can’t process tens of thousands of transactions per second without either increasing the block size significantly or reducing the time between blocks drastically, some have opted to do both. Both of these actions combined will create an environment where tens of thousands of transactions can be achieved, but the cost is on-chain bloat in the realms of 1 TB per day. 

## How does the Lighting Network deal with these considerations

The lightning network is an off-chain scaling solution that starts and ends on-chain. The only data that hits the blockchain is the opening and closing of payments channels, all other transactions are conducted off-chain.

For example: On the Lightning Network I can open a channel at the cost of 2000 atoms, conduct 4000 transactions at the total cost of 4000 atoms. And then close the channel at a cost of 2000 atoms. The total cost, 8000 atoms and only the opening and closing of these channels ends up on-chain, resulting in almost no weight to the overall blockchain. 4002 total transactions reduced to 2 on-chain transactions is highly efficient.

To do this same process on-chain, I would conduct 4000 transactions at a cost of 2000 atoms each. The total cost would be 8,000,000 atoms or 0.08000000 DCR. The on-chain weight of these transactions would be approximately 1 MB or over 2 full blocks on the Decred blockchain. This is not efficient and gets expensive rapidly.

Calculation: 
* 215 Bytes x 4000 = 860,000 Bytes (0.860 MB)

In terms of not being able to open and close channels during times of congestion, this becomes less of an issue when the majority of smaller transactions are being processed off-chain. That being said, if blocks become consistently full, the cost of opening and closing channels would increase. Scaling the block size is still an option for reducing congestion, but this would still be minimal compared to the scaling needed of an on-chain solution.

## The future is micro transactions

As we move forward, the likelihood is that the bulk of all blockchains transactions will be micro transactions. Micro transactions will typically be lower than 10,000 units, all the way down to a single unit. If a blockchain protocol becomes popular, these transactions with be in the 100s of thousands per second. If all of these transactions are conducted on-chain, every blockchain currently available, will fail in at least one of the following areas:
* The Blockchain will become congested 
* Fees will get unreasonably high
* The blockchain will become bloated

As it currently stands, the majority of layer 1 and layer 2 blockchains are incapable of processing micro transactions at a fee of a single unit or less (0.00000001 BTC/DCR).

The Lightning Network is still in active development, but it’s already the most suitable solution for micro transactions. And the fact that it can be run on a peer to peer  lightweight SPV wallet makes it even more impressive.

