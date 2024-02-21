| Author | Phoenix Green |
| :---- | :---- |
| Title | Non-custodial Lightning Network Solutions (Better Title needed) |
| Headline  | Why is Decred’s client-side SPV the perfect home for the Lightning Network |
| Cypherpunktimes | cypherpunktimes.com/...link |
| Publish Date | 00 Jan 20?? |

| Social Media | Link |
| :---- | :---- |
| Twitter | post link… |
| Twitter | thread link… |
| Twitter | poll link… |
| Reddit  | link… |
| Bison Relay | News feed title |
| Other platforms | Instagram and TikTok |

Thesis statement 

The Lightning Network has achieved the monumental target of processing thousands of micro-transactions per second at the cost of a single Atom/Satoshi. But is it possible to have this functional in a non-custodial wallet?


# Article - Non-custodial Lightning Network Solutions
Title: Why is Decred’s client-side SPV the perfect home for the Lightning Network? 

The Lightning Network (LN) has achieved the monumental target of processing thousands of transactions per second at the cost of a single atom per transaction (0.00000001 DCR). But is it to have this functionality in a lightweight non-custodial wallet? 

The answer is yes, it’s already been built and is functioning as intended. Checkout Bison Relay to learn more.

But what about the anti-Lightning Network narratives? Popular voices in the crypto space are suggesting that the Lightning Network doesn’t work, can’t achieve its goals, and only has full functionality when used through custodial wallet providers. Is this false information?

Although, this is certainly the case with a lot of popular wallet providers, it doesn’t have to be this way. As said previously, Bison Relay is a good example of this.

## So how is Decred achieving a non-custodial Lightning Network?

The Lightning Network was principally designed to solve one problem! And that was, to be able to process thousands of transactions per second whilst minimising the demand for block space. As a side note. The Lightning Network performs best when it’s dealing with small or micro-transaction, for example, individual transactions less than 0.01 DCR. Bigger transactions than this, should mostly be conducted on-chain for maximum security.

To facilitate the non-custodial, peer to peer nature of LN, Decred has made some very interesting technical decisions that have made the Lightning Network a key piece of infrastructure on the platform. For example, Decred’s SPV mode, Hash Time-Locked Contracts and all other relevant op-codes needed for the Lightning Network, have all been included in the protocol through consensus upgrades.

To facilitate the peer to peer nature of LN transactions, a lightning Network wallet needs to be non-custodial, lightweight, functional and have a high level of security. To enable all of these features, there’s no better solution than a Decred SPV wallet. Decred’s SPV mode has full network support and processes the data required client-side, minimising the burden to the nodes running the network. Decred’s SPV mode also has similar levels of security as a fully validating node, due to the “header commitments” consensus upgrade. All of which means, no third-party validators or middle men are required to process Lightning Network data, as this is fetched synchronised and communicated directly over the network.

## Lightning Network Payment Channels

With the non-custodial wallet infrastructure in place, the next area to address are the Lightning Network payment channels. Opening and closing LN channels can be problematic due to the need for peers to be online at the same time and the preloaded liquidity aspect of these channels. In a typical setup, individual peers will connect to each other, creating a route across the network. This can mean that an individual has many channels open to facilitate broad connectivity.

To make the process of opening and closing channels more user-friendly, Decred has utilities hubs. Hubs allow broader connectivity and only require two channels to be set up. This reduces the number of connections needed to communicate with all peers on the network. The hub is a more centralised component that offers valuable services, including opening and maintaining channels and adding receive liquidity. Hubs are incentivised to run these services through a fixed fee of 1 atom for every 1 KB of data sent and received, and a 1% commission for providing inbound liquidity.

Lightning Network hubs also help to make channel liquidity more deterministic. For instance, if you put 0.1 dcr into your outbound channel, you know you can send up to that limit to anyone on the network. The same applies for your inbound channel, if you load the inbound channel with 0.5 dcr, you know you can receive up to that limit from anyone on the network. Once these funds are exhausted, you’ll need to close the channels and open new ones. 

**Lightning Network costs and fees:**
Opening an outbound channel = 3640 atoms (0.00003640 DCR)
Opening an inbound channel = 3640 atoms (0.00003640 DCR)
Inbound channel liquidity fee = 1% (if you ask for 0.1 DCR in inbound liquidity, the fee will be 0.001 DCR)
Transaction fee = 1 atom for every 1 KB of data (0.00000001 DCR)

As a side note, peers on the Lightning Network don’t have to route their payment channels through LN hubs. But it does greatly improve the user experience and simplify the process of finding peers, setting up channels and pre-populating channel liquidity.

It should also be noted that LN hubs don’t have custody over the funds placed in the channels routed to them. Signing transactions, opening and closing channels require both the peer and the hub to be online to process these actions. 

The Lightning Network is in active development and constantly being refined to offer a streamline user experience. When combined with Decred’s SPV mode, the aim of being fully non-custodial is still very much alive and well.

