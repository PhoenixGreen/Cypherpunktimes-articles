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

Pre-discussion, research and questions:
* What are the most popular LN wallets?
* How do these platforms open and close channels? Are there any restrictions or limitations?
* How do these platforms facilitate inbound liquidity?
* Who provides the liquidity and at what cost?
* What are the fees for opening and closing channels?
* What are the fees for transacting over LN on these platforms?

* Is the LN processing done client-side or server-side on these platforms?
* Are any of these platforms using Neutrino SPV?
* Are any of the platforms using Electrum lite-clients?
* If not Neutrino / Electrum, how is this service being provided? e.g. fully centralised server model.


# Non-custodial Lightning Network Solutions
Title: Why is Decred’s client-side SPV the perfect home for the Lightning Network?

The Lightning Network has achieved the monumental target of processing thousands of transactions per second at the cost of a single Atom/Satoshi per transaction. But would it be possible to have this functional in a non-custodial wallet?

The answer is yes, it’s already been built and is functioning as intended. Checkout Bison Relay to learn more.

But what about the anti-Lightning Network narratives? Popular voices in the crypto space are suggesting that the Lightning Network doesn’t work, can’t achieve its goals, and only has full functionality when used through centralised and custodial wallet providers. Is this false information?

Although, this is certainly the case with a lot of the popular wallet providers, especially those operating on the Bitcoin network. It doesn’t have to be this way. As said previously, Bison Relay is a good example of this.

## So how is Decred achieving a non-custodial Lightning Network?
The Lightning Network was principally designed to solve one problem. And that was, to be able to process thousands of transactions per second whilst minimising the demand for block space. As a side note. The Lightning Network performs best when it’s dealing with small or micro-transaction.

To facilitate the non-custodial, peer to peer nature of LN, Decred has made some very interesting technical design decisions that have made the Lightning Network a key piece of infrastructure on the platform. 

A lightning Network wallet needs to be non-custodial, lightweight, functional and have a high level of security. To enable all of these features, there’s no better solution than a Decred SPV wallet. Decred’s SPV mode has 100% full node support and processes the data required client-side, minimising the burden to full nodes running the network. Decred’s SPV model also has similar levels of security as a fully validating node, due to its “header commitments” upgrade. All of which means, Decred’s SPV model doesn’t require third-party validators or middle men to process the data required. 

Decred’s SPV wallets are the perfect solution for housing the Lightning Network and its applications. This is due to being lightweight, non-custodial in nature and being able to synchronise and communicate directly to the network.

## Lightning Network Payment Channels

With the wallet infrastructure in place, the next area to address are the LN payment channels. Opening and closing LN channels can be problematic on the Lightning Network due to the need for peers to be online at the same time and the preloaded liquidity aspect of these channels.

To make the process of opening and closing channels easier, whilst remaining non-custodial, Decred has the ability to use LN hubs.

The main benefits of using a Lightning Network hub:
* Setup 2 channels (outbound and inbound) — These channels can automatically connect to peers on the network, without setting up individual channels for each peer.
* Liquidity — When you set up your channels, you also set up the liquidity for each of these channels. Outbound is the amount you can send. Inbound is the amount you can receive.

As a side note, peers on the Lightning Network don’t have to route their payment channels through LN hubs, but it does greatly simplify the process of finding peers, channel setup and pre-populating channels with liquidity. 

The Lightning Network is in active development and constantly being refined to offer a streamline user experience. And when combined with Decred’s SPV mode, the aim of being fully non-custodial is still very much alive and well.
