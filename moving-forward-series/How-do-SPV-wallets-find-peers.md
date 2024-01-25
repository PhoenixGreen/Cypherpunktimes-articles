## How do SPV wallets find peers?

If you’ve ever used a multichain Simplified Payment Verification (SPV) wallet like DCRDEX, a few questions might pop to mind when comparing Decred against Bitcoin, Bitcoin Cash and Litecoin. Firstly, how does Decred’s SPV mode synchronise, so quickly when compared to the others? And secondly, why does Decred seem to have more available nodes to synchronise to? 

Let’s focus on the second point, “why does Decred have more available nodes to synchronise to?”. In many ways, this seems like an odd scenario, especially when you compare the number of full nodes running those networks. So why do these platforms encounter issues when trying to find full nodes to serve SPV wallets? 

The answer comes mostly down to support and the fact that not all full nodes running these networks are using the same, or even, the latest version of the software. These nodes could also not be configured to support SPV wallets. In the case of older nodes, there’s also the possibility that the data required for SPV is not available. 

In Decred’s case, there is only one type of SPV, and this has been integrated fully into the protocol. Meaning, the information an SPV wallet needs is a core part of a Decred full node. Another interesting thing about Decred’s protocol, is that all full nodes running the network are using the same version of the software. There are no ambiguities between versions that could cause a full node not to server an SPV wallet with the data required. 

Another comparison to be made with alternative methods of SPV is the burden they place on the network. In Decred’s case, there is practically no reason for a full node not to serve an SPV wallet. Decred’s SPV is designed in such a way that it’s not a burden on full nodes running the network. This is due to the majority of the bandwidth and processing being done in the SPV wallet.

Decred's compact filter (GCS) model has an extremely minimal impact on full nodes and for this reason, support is accepted network wide. Older models of SPV which are based on server-side bloom filters are not so friendly to the full nodes running a network and require more bandwidth, resources and generally put a massive load on the full nodes serving them. 

## Neutrino client-side SPV (BIP157)

SPV modes requiring server-side bloom filters are gradually being phased out and replaced with client-side models. This is the case with Decred’s SPV model and Lightning Labs Neutrino model (BIP157), both of which are used for DCRDEX’s native wallets (including Bitcoin, Litecoin, and Bitcoin Cash).

The main difference between Decred’s implementation and Neutrino is the way the data is served and downloaded. 

**Serving SPV data:** In Decred’s case, pretty much 100% of the full nodes running the network can and will server SPV wallets. Whereas, on most other networks (including Bitcoin, Litecoin, Bitcoin Cash) support is optional, which results in low uptake and not being available on older node software.

**Downloading SPV Data: **Decred had a header commitments consensus upgrade in 2020 that made the block filters and merkle proofs part of the block header. This improves the security by making the data needed for serving SPV wallets a required component that’s included in each block in the blockchain. On other blockchains, this data is at the discrepancy of the nodes running the network. For instance, a parallel set of filter headers are maintained that essentially mirror the real blockchain headers but add the additional data required by Neutrino wallets to verify the filters.

## The SPV synchronising process

As a quick comparison, here is a basic overview of the main types of SPV mode (server-side SPV, Neutrino, and Decred’s client-side SPV) and how they process the required data for SPV wallets.

** Server-side SPV (before BIP157) synchronising process: **
1. SPV wallet downloads all the headers from block 1 to the most recent block
2. SPV wallet builds a bloom filter making a list of keys, addresses, and hashes it is interested in
3. SPV wallet sends the filter to a full node with the search parameters to look for data matches
4. Full node processes this filter and sends back matching data 
5. SPV wallet verifies and discards unwanted data. Then uses the correct data to update their wallet's state (e.g. balances, used addresses, etc)
6. SPV wallet modifies the filter and repeats the process

**Decred Client-side SPV synchronising process:**
1. SPV wallet downloads all the headers from block 1 to the most recent block and performs several verifications to help ensure they all link together properly and haven't been tampered with
2. SPV wallet downloads potentially relevant compact filters and associated inclusion proofs and verifies them against the header commitments
3. SPV wallet performs wallet-side checks to determine if the filter matches any related transactions
4. SPV wallet fetches the block when there is a match and finds the related transaction in that block which it then uses to update the wallet's state (e.g. balances, used addresses, etc)

**Neutrino’s (BIP157) Client-side SPV synchronising process:**
Neutrino’s Client-side SPV synchronising process is very similar to that of Decred’s but without the header commitments upgrade which is very much unique to the Decred blockchain. Instead, a Neutrino node has to connect to specific full nodes that are maintaining a parallel set of filter headers with the additional data required by Neutrino wallets to verify the filters.

## Moving forward

Having full support for SPV mode on the Decred blockchain opens up a world of possibilities and activities due to the improved participation, reliability, privacy, and security of this lightweight solution.

With this technology, Decred has already begun building various unique user experiences, including:

DCRDEX — A non-custodial peer to peer, decentralised exchange
CryptoPower — A non-custodial multichain lightweight wallet
Bison Relay — A non-custodial lightweight Lightning Network wallet that facilitates a wealth of user experiences and activities, from social media, messaging, content delivery and micro-transactions. 

All of this development is possible because Decred’s SPV has the full support of the network, is extremely fast, reliable, secure, private and lightweight. When you have this level of integration, the possibilities are limitless.
