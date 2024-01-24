## How do SPV wallets find peers? (Better title???)

If you’ve ever used a multichain SPV wallet like DCRDEX, a few questions might pop to mind when comparing Decred against Bitcoin, Bitcoin Cash and Litecoin. Firstly, how does Decred’s SPV mode synchronise, so quickly when compared to the others? And secondly, why does Decred seem to have more available nodes to synchronise to? 

Let’s focus on the second point, “why does Decred have more available nodes to synchronise to?”. In many ways, this seems like an odd scenario, especially when you compare the number of full nodes running on those networks. For instance, Bitcoin has thousands of full nodes running the network, where Decred typically has less than 500. So why do these platforms encounter issues when trying to find full nodes to serve SPV wallets? 

The answer comes mostly down to support and the fact that not all nodes running on these networks are using the same, or even, the latest version of the software, or configured to serve SPV wallets. In the case of older nodes, there’s also a possibility that the SPV data required is not even available. 

In Decred’s case, there is only one type of SPV, and this has been integrated fully into the protocol. Meaning, the information an SPV wallet needs is a core part of a Decred full node. Another interesting thing about Decred’s protocol, is that all full nodes running the network are using the same version of the software. There are no ambiguities between versions that could cause a full node not to server an SPV wallet with the data required. 

Another comparison to be made with alternative methods of SPV is the burden they place on the network. In Decred’s case, there is practically zero reason for a full node not to serve SPV wallets. Decred’s SPV is designed in such a way that it’s not a burden on full nodes running the network. This is due to the majority of the bandwidth and processing being done in the SPV wallet.

Decred's compact filter (GCS) model has an extremely minimal impact on full nodes running the network and for this reason, support is accepted network wide. Older models of SPV which are based on server-side bloom filters are not so friendly to the full nodes running a network and require more bandwidth, resources and generally put a massive load on the full nodes serving them. 

## Neutrino client-side SPV (BIP157)
SPV modes requiring server-side bloom filters are gradually being phased out and replaced with client-side models. This is the case with Decred’s SPV model and Lightning Labs Neutrino model (BIP157), both of which are used for DCRDEX’s native wallets (including Bitcoin, Litecoin, and Bitcoin Cash).

The main difference between Decred’s implementation and Neutrino is the way the data is served and downloaded. 

**Serving SPV data:** In Decred’s case, pretty much 100% of the full nodes running the network can and will server SPV wallets. Whereas, as on most other networks (including Bitcoin, Litecoin, Bitcoin Cash) support is optional, which results in low uptake and not being available on older node software.

**Downloading SPV Data: **Decred had a consensus upgrade in 2020 that made the block filters and merkle proofs part of the block header. This greatly simplified the synchronisation process and makes the data needed for serving SPV wallets a required component that’s included in each block in the blockchain. On other blockchains, this data is at the discrepancy of the nodes running the network.

## The SPV synchronising process
As a quick comparison, here is a basic overview of the main types of SPV mode (server-side SPV, Neutrino, and Decred’s client-side SPV) and how they process the required data for SPV wallets.

** Server-side SPV (before BIP157) synchronising process: **
1. SPV wallet downloads all block headers from a full node
2. SPV wallet builds a bloom filter making a list of keys, addresses, and hashes it is interested in
3. SPV wallet sends the filter to a full node with the search parameters to look for data matches
4. Full node sends back matching data 
5. SPV wallet verifies and discards data. Then uses the correct data to update their UTXO set.
6. SPV wallets modifies the filter and repeats the process

** Neutrino’s (BIP157) Client-side SPV synchronising process:**
1. SPV wallet downloads all Block Headers from full nodes
2. SPV wallet downloads Compact Filter Headers and Verifications from full nodes
3. SPV wallet downloads Compact Filters and Verifications from full nodes
4. SPV wallet checks filters and verifications for possible data 
5. SPV wallet downloads the desired block from full nodes. Then uses the correct data to update their UTXO set. 
6. SPV wallet then repeats this process to stay in sync with the network.

**Decred Client-side SPV synchronising process:**
1. SPV wallet downloads all Block Headers + filters from full nodes
2. SPV wallet checks filters and verifications for possible data 
3. SPV wallet downloads the desired block. Then uses the correct data to update their UTXO set. 
4. SPV wallet then repeats this process to stay in sync with the network.

## Moving forward
Having full support for SPV mode on the Decred blockchain opens up a world of possibilities and activities whilst improving the reliability, privacy, and security of this lightweight solution.

With this technology, Decred has already begun building various unique user experiences, including:

DCRDEX — A non-custodial peer to peer, decentralised exchange
CryptoPower — A non-custodial multichain lightweight wallet
Bison Relay — A non-custodial lightweight Lightning Network wallet that facilitates a wealth of user experiences and activities, including news feeds, social media, messaging, content delivery and micro-transactions. 

All of this development is possible because Decred’s SPV is crazy fast, radically reliable, super secure, extremely lightweight, perfectly private and supported fully by the network.
