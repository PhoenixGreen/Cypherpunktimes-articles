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

The Lightning Network (LN) has achieved the monumental target of processing thousands of transactions per second at the cost of a single Atom/Satoshi per transaction (0.00000001 DCR). But is it possible to have this functional in a non-custodial wallet?

The answer is yes, it’s already been built and is functioning as intended. Checkout Bison Relay to learn more.

But what about the anti-Lightning Network narratives? Popular voices in the crypto space are suggesting that the Lightning Network doesn’t work, can’t achieve its goals, and only has full functionality when used through centralised and custodial wallet providers. Is this false information?

Although, this is certainly the case with a lot of the popular wallet providers, it doesn’t have to be this way. As said previously, Bison Relay is a good example of this.

## So how is Decred achieving a non-custodial Lightning Network?
The Lightning Network was principally designed to solve one problem! And that was, to be able to process thousands of transactions per second whilst minimising the demand for block space. As a side note. The Lightning Network performs best when it’s dealing with small or micro-transaction e.g. individual transactions less than 0.1 DCR/BTC. Bigger transactions than this, should mostly be conducted on-chain for maximum security.

To facilitate the non-custodial, peer to peer nature of LN, Decred has made some very interesting technical design decisions that have made the Lightning Network a key piece of infrastructure on the platform. For example, SPV, Hash Time-Locked Contracts and the relevant op-codes needed for LN (including the SHA256, CSV) have been approved by stakeholders as consensus upgrades.

To facilitate peer to peer transactions, a lightning Network wallet needs to be non-custodial, lightweight, functional and have a high level of security. To enable all of these features, there’s no better solution than a Decred SPV wallet. Decred’s SPV mode has full network support and processes the data required client-side, minimising the burden to the nodes running the network. Decred’s SPV mode also has similar levels of security as a fully validating node, due to its “header commitments” upgrade. All of which means, Decred’s SPV mode doesn’t require third-party validators or middle men to process the data required for the Lightning Network. This is due to SPV wallets being able to synchronise and communicate directly with the network.

## Lightning Network Payment Channels

With the non-custodial wallet infrastructure in place, the next area to address are the Lightning Network payment channels. Opening and closing LN channels can be problematic due to the need for peers to be online at the same time and the preloaded liquidity aspect of these channels. In a typical setup, individual peers will connect to each other, creating a route across the network. This can mean that an individual can have many channels open to facilitate broad connectivity.

To make the process of opening and closing channels more user-friendly, one method Decred has employed is routing hubs. If a user wants to use one of these hubs, it’s now possible to set up just two channels, an outbound and an inbound channel, and have broader connectivity by routing these channels through the hub. This also reduces the number of connections needed to communicate with all peers on the network. 

Lightning Network routing hubs also help to make channel liquidity more deterministic. For instance, if you put 0.1 dcr into your outbound channel, you know you can send up to that limit to anyone in the network. The same applies for your inbound channel, if you load the channel with 0.5 dcr, you know you can receive up to that limit from anyone on the network. Once these funds are exhausted, you’ll need to close the channels and open new ones. The interesting thing here is this reduces the process from many channels to two channels, which simplifies the process massively.

Peers on the Lightning Network don’t have to route their payment channels through LN hubs, but it does greatly simplify the process of finding peers, setting up channels and pre-populating channel liquidity. 

It should also be noted that LN hubs don’t have full custody over the channels. Opening and closing channels requires both the peer and the hub to be online to process these actions. 

The Lightning Network is in active development and constantly being refined to offer a streamline user experience. When combined with Decred’s SPV mode, the aim of being fully non-custodial is still very much alive and well.
