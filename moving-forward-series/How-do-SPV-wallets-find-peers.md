
| Author | Phoenix Green |
| :---- | :---- |
| Title | How do SPV wallets find peers |
| Headline  | Decred’s SPV has the full support of the network, is extremely fast, reliable, secure, private and lightweight. When you have this level of integration, the possibilities are limitless. |
| Cypherpunktimes | https://www.cypherpunktimes.com/how-do-spv-wallets-find-peers/ |
| Publish Date | 31 Jan 2024 |

| Social Media | Link |
| :---- | :---- |
| Youtube | https://youtu.be/4XrPALy9NpY |
| Podcast | https://podcasters.spotify.com/pod/show/cypherpunktimes/episodes/How-do-SPV-wallets-find-peers-e2f6091/a-aatlslt |
| Twitter Post | https://x.com/cypherpunktimes/status/1752644510327140522 |
| Twitter Full Video | link… |
| Twitter Clip 1 | https://x.com/DecredSociety/status/1752660030610960585?s=20 |
| Reddit  | https://www.reddit.com/r/decred/comments/1afmtse/how_do_spv_wallets_find_peers/ |
| Bison Relay | Title: How do SPV wallets find peers? |

# How do SPV wallets find peers

If you’ve ever used a multi-chain SPV (Simplified Payment Verification) wallet like DCRDEX, a few questions might pop to mind when comparing Decred against Bitcoin, Bitcoin Cash and Litecoin. Firstly, how does Decred’s SPV mode synchronise, so quickly when compared to the others? And secondly, why does Decred seem to have more available nodes to synchronise to? 

Let’s focus on the second point, “why does Decred have more available nodes to synchronise to?”. In many ways, this seems like an odd scenario, especially when you compare the number of full nodes running those networks. So why do these platforms encounter issues when trying to find full nodes to serve SPV wallets? 

The answer comes mostly down to support and the fact that not all full nodes running these networks are using the same, or even, the latest version of the software. In the case of older nodes, there’s also the possibility that the data required for SPV is not available. 

In Decred’s case, there is only one type of SPV, and this has been integrated fully into the protocol. Meaning, the information needed is a core part of a Decred full node. Another interesting thing about Decred’s protocol, is that all full nodes running the network are using the same version of the software. There are no ambiguities between versions that could cause an SPV wallet not to be served with the data required. 

Another reason older models, commonly referred to a server-side SPV, are not so readily supported is due to the burden they place on the network and the resources required by the nodes to process the data. Decred’s client-side SPV model is designed in such a way that it’s not a burden on the network. This is due to the majority of the bandwidth and processing being done in the SPV wallet itself.

## Neutrino client-side SPV (BIP157)

SPV modes requiring server-side bloom filters are gradually being phased out and replaced with client-side models. This is the case with Decred’s SPV model and Lightning Labs Neutrino model (BIP157), both of which are used for DCRDEX’s native wallets (including Bitcoin, Litecoin, and Bitcoin Cash).

The main difference between Decred’s implementation and Neutrino is the way the data is served and downloaded. 

**Serving SPV data:** In Decred’s case, pretty much 100% of the full nodes running the network can and will server SPV wallets. Whereas, on most other networks (including Bitcoin, Litecoin, Bitcoin Cash) support is optional, which results in low uptake.

**Downloading SPV Data: **Decred had a header commitments consensus upgrade in 2020 that made the block filters and merkle proofs part of the block header. This improves the security by making the data needed for serving SPV wallets a required component. On other blockchains, this data is at the discrepancy of the nodes running the network. For instance, nodes serving SPV clients have to maintain a parallel set of filter headers that essentially mirror the real blockchain headers but add the additional data required by Neutrino wallets to verify the filters.

## The SPV synchronising process

As a quick comparison, here is a basic overview of the main types of SPV mode (server-side SPV, Neutrino, and Decred’s client-side SPV) and how they process the required data for SPV wallets.

** Server-side SPV (before BIP157) synchronising process: **
1. The SPV wallet downloads all the block headers from block 1 to the most recent block
2. The SPV wallet builds a bloom filter making a list of keys, addresses, and hashes it is interested in
3. The SPV wallet sends the filter to a full node with the search parameters to look for data matches
4. The Full node processes this filter and sends back matching data 
5. The SPV wallet verifies and discards unwanted data. Then uses the correct data to update their wallet's state (e.g. balances, used addresses, etc)
6. The SPV wallet then modifies the filter and repeats the process

**Decred Client-side SPV synchronising process:**
1. The SPV wallet downloads all the block headers from block 1 to the most recent block and performs several verifications to help ensure they all link together properly and haven't been tampered with
2. The SPV wallet downloads potentially relevant compact filters and associated inclusion proofs and verifies them against the header commitments
3. The SPV wallet performs wallet-side checks to determine if the filter matches any related transactions
4. The SPV wallet fetches the block when there is a match and finds the related transaction in that block which it then uses to update the wallet's state (e.g. balances, used addresses, etc)

**Neutrino’s (BIP157) Client-side SPV synchronising process:**
Is very similar to that of Decred’s but without the header commitments upgrade which is very much unique to the Decred blockchain. Instead, a Neutrino wallet has to connect to specific full nodes that are maintaining a parallel set of filter headers with the additional data required to verify the filters.

## Moving forward

Having full support for SPV mode on the Decred blockchain opens up a world of possibilities and activities due to the improved participation, reliability, privacy, and security of this lightweight solution.

With this technology, Decred has already begun building various unique user experiences, including:

DCRDEX — A non-custodial, peer to peer, decentralised exchange
CryptoPower — A non-custodial, multi-chain lightweight wallet
Bison Relay — A non-custodial, lightweight Lightning Network wallet that facilitates a wealth of user experiences and activities, from social media, messaging, content delivery and micro-transactions. 

All of this development is possible because Decred’s SPV has the full support of the network, is extremely fast, reliable, secure, private and lightweight. When you have this level of integration, the possibilities are limitless.
