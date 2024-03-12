| Content | Description |
|---|---|
| Title               | Micro transactions and the underlining values |
| Author              | Phoenix Green |
| Featured text       | Why does it matter if a blockchain can process micro transactions, and will we ever need them? |
| CT link             | FIXME |
| Publish date        | YYYY-MM-DD FIXME |

| Social Media | Links |
|---|---|
| YouTube link        | FIXME |
| Podcast link        | FIXME |
| Bison Relay post    | Title |
| Reddit link         | FIXME |
| CT tweet            | FIXME |
| YouTube tweet       | FIXME |
| Twitter full video  | FIXME |
| Twitter clip 1      | FIXME |
| Twitter clip 2      | FIXME |
| Matrix post         | Promote your main tweet in "DCR Social Media" channel |


## Thesis statement

A global peer to peer digital currency network is a massive ledger of every transaction ever created from the genesis to the present day. For a network to remain peer to peer, solutions need to be found that reduce the burden of running the network and also allow for frictionless payments of the smallest qualities.

Outline:
* The factors that define a micro transaction
* What can micro transactions be used for
* How do platforms compare when processing these transactions?
	* Fees
	* Transaction size on-chain
	* Average time it takes to process, 100k transactions
	* Any other considerations?


## Pre-discussion, research and questions

What average fees do specific scaling blockchains charge?
What is the size of an average transaction on these chains?
Block times and block sizes of scaling blockchains?
What it takes to run these chains? Blockchain size, ram, processing power, storage.

Which chains should I compare?
I’m currently thinking of doing: Solana, Polygon, Dash, Nano, Litecoin, Bitcoin Cash and the Lightning Network.


---
--- ARTICLE GOES BELOW THIS POINT ---

---

## Micro transactions and the underlining values

A global peer to peer digital currency is a massive ledger of every transaction ever created from the genesis to the present day. For a network to remain peer to peer, solutions need to be found that reduce the burden of running the network and also allow for frictionless payments of the smallest quantities.

Most individuals can’t comprehend the amount of storage and computing power it takes to achieve the goal of producing 1000s of small transactions per second. The aim of this discussion is to shine a bright light on transaction scaling, with a specific focus on micro transactions.

## The factors that define a micro transaction
What is a micro transactions, and how can we identify a solution that achieves this goal at scale whilst remaining a peer to peer network? This can be categorised into six unique points, all of which need to produce optimally low values:

* Can the smallest unit available on a network be sent?
* Is the fee to send this transaction less than or equal to the smallest unit on the network?
* Can this transaction be confirmed instantly or under a few seconds?
* How many of these transactions can be sent per second?
* What is the weight of these transactions on-chain?
* How much computer and internet power is need to run and stay in sync with the network, if it’s producing hundreds of thousands of transactions per second?

In most cases, we can assume, if a network requires more than 300 GB of storage; 4 GB of RAM, and an internet bandwidth greater than 20 MB per second, the majority of users will not be able to or want to run the network. At this point, and in my opinion, a network no longer functions in a peer to peer capacity. 

Some would argue, this is nonsense, my phone has 1 TB of storage, 8 GB of RAM and 200 MB per second internet bandwidth. To which, I would suggest trying to run a network that functions at the above capacity. It won’t take too long for those same people to come to their senses, once their $1000 phone completely burns out after a few hours of running the chain.

## What can micro transactions be used for?

It turns out that blockchain technology is useful for more than just sending large amounts of money across the internet securely and permissionlessly. You can also facilitate all kinds of communication activities, including:
* Tipping users for content, participation, and engagement
* As a mechanism to reduce spam for communication services
* Buying low-cost items and services instantly with near zero fees

## How do platforms compare when scaling transaction volume?

Here is a chart of the basic information regarding popular platforms that are trying to achieve the scaling capacity of thousands of transactions per second. Of which, only two solutions enable you to send micro transactions of the smallest unit at a cost of a single unit or less. As you can see, those are Nano and the Lightning Network.

| Blockchain | Decimal | Tr Fee | Tr size | Conf time | TPS | Blockchain size |
|---|---|---|---|---|---|---|
| Solana | 9 | 0.00002000 | 250 Bytes | Instant | 65,000 | Over 1 TB |
| Polygon | 17 | 0.00200000 | 250 Bytes | 20 mins | 65,000 | Over 1 TB |
| Decred LN | 8 | 0.00000001 | Near zero Bytes | Instant | 100,000+ | Majority off-chain |
| Litecoin | 8 | 0.00004400 | 250 Bytes | 2.5mins | 54 | Over 140 GB |
| Dash Instasend | 8 | 0.00002200 | 225 Bytes | 1–2 secs | 35 | Over 32 GB |
| Digibyte | 8 | 0.00004000 | 250 Bytes | 15 seconds | 1066 | Over 36 GB |
| Nano | 30 | 0.00000000 | 250 Bytes | Instant | 1000 | Over 113 GB |

(NOT FOR VIDEO) Statistics side note: These stats have been taken from platform-specific documentation and their representative block explorers during March 2024. Where possible, a low average has been calculated to represent the best efficiency of each platform.

All the platforms listed achieve the ability of sending lots of cheap and fast transactions per second. Which is a much-needed functionality, but these platforms would still get costly if you needed to send thousands of transactions per day. For example, If I send 10,000 transactions on Digibyte the cost would be (4000 × 10,000) 40,000,000 units or 0.4 DGB. Conducting these same transactions on LN would be 10,000 units or 0.00010000 DCR. And on Nano, the fees would be zero.

Another factor to consider is the amount of weight these transactions would add to the blockchain. Out of all of these solutions, only one optimises natively to reduce on-chain bloat, and that’s the Lightning Network. All other platforms produce approximately 250 Bytes per transaction, all of which, goes on-chain. Running the same example as above for 10,000 transactions on the Nano platform (10,000 × 250 B = 2.5 million Bytes), this would produce approximately 2.5 MB of on-chain data. On the Lightning Network, this same calculation of 10,000 transactions can be reduced to 2 on-chain transactions of 500 Bytes or 0.0005 MB. This is due to the off-chain nature of the Lightning Network and the need to only synchronise with the chain when opening and closing payment channels. 
Now let's look at the computer power needed to run a one of these networks when they are operating at scale. Fortunately, there are two platforms already considered to be at this level, which are Solana and Polygon.

## Solana’s Computing power

Solana is a highly scalable layer 1 Blockchain built for mass adoption. The requirements to run a validator node are generally unreachable for the typical user, and starts at needing:
* A high-speed internet connection
* A CPU with 12 cores / 24 threads, or more
* 256 GB of RAM or more, the recommendation is 512 GB of RAM
* 500 GB, or larger Disk space for accounts
* 1 TB or larger disk space for Ledger

As per Solana’s specifications, the specs listed here should be considered the bare minimum — https://docs.solanalabs.com/operations/requirements

Solana produces approximately 1 TB of data per day. To keep the ledge size manageable, the platform utilises pruning and sharding methods. 

Even with all this capacity, it’s still worth noting that on both Solana and Polygon, you can’t send a micro transaction of a single unit for a single unit fee.

## Decred’s LN Computing power 

In comparison, Decred’s Lightning Network is run using the platform's Lightweight SPV mode. Which requires less than 2 GB of storage, 1 GB of RAM and can operate seamlessly over an internet connection of approximately 2 MB per second.

Over the lightning Network, you can send a single unit at the cost of a single unit (0.00000001 DCR). Which is also the standard transaction fee for transactions of 1 KB of data or less.

The Lightning Network conducts the majority of its transactions off-chain. Only the opening and closing of payment channels are recorded on-chain. This allows for greater scalability at minimum cost in all six areas listed previously. Decred’s LN is also fully non-custodial and extremely secure.

The Lightning Network gets a lot of criticism in the crypto space. But as I continue to conduct my research, this seems more to do with envy and the fact that others can’t achieve the same levels of transaction volume, without considerable trade-offs. 

When implemented properly, as it is on the Decred blockchain, the Lightning Network is currently the only crypto platform capably of maintaining peer to peer payment functionality at a scale of 100,000 TPS. The Lightning Network is already capable of processing similar qualities of transactions per second to that of Visa’s payment network. Which is impressive when you consider this is still a relatively young technology.
