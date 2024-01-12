# Can a Crypto Wallet be Lightweight, Private, AND Secure? The SPV Model Leads the Way

People need mobile wallets that are fast to set up, easy to use and very secure. All too often, mobile wallets make extreme security sacrifices in order to slightly improve ease of use. Including, the provision for a centralised node to serve requests to the wallet software. This is a trust model that processes all wallet information, sent and received, through a single point of failure. SPV challenges this convention by providing a high level of security whilst improving the user experience. 

## Fast and Small

If you’re looking for a non-custodial mobile wallet, Simplified Payment Verification (SPV) is an ideal solution.  SPV is designed to be intentionally lightweight, as it interacts with the blockchain by only fetching and downloading the data, that is absolutely necessary. This includes block headers, block filters, and the full blocks that contain transaction data directly associated with the wallet. As you can imagine, this reduces the size, setup, and sync times considerably from hours to minutes. In Decred’s case, the required storage space of a fully validating node is approximately 12 GB while its SPV counterpart is approximately 0.2 GB.

## Compact Block Filters

One aspect that aids in this design and makes the method extremely compact is the use of filters. SPV relies on the ability to identify and retrieve relevant transactions from the blockchain. Filters act like a search mechanism to help an SPV wallet find transactions it should care about. Decred’s Compact filters allow SPV nodes to retrieve this information without having to reveal or leak information regarding coin ownership. For instance, SPV nodes can ask full node peers for blocks that contain matching data without revealing addresses, keys, or the transactions they are looking for. Decred's filtering process is completed in the wallet to enhance privacy. Older methods of filtering put the entire workload onto the full nodes running the network, which is bad for network efficiency and privacy.

## Decred’s Implementation of the SPV model

When Decred implemented the “Block Header Commitments” consensus upgrade in 2020 ([DCP: 0005 “Block Header Commitments”]) it focused on bring the SPV security level closer to that of a fully validating node. This was done through a combination of security features like committed fraud proofs, inclusion proofs, and filters. As long as there is at least one honest fully-validating node on the network, SPV wallets can rest easy knowing that their transactions are valid and they are not being tricked by malicious nodes. 

## Lite clients vs SPV

SPV and Fully validating nodes are my wallets of choice, as they offer the highest levels of security whilst verifying blockchain data independently. But, of course, there are other solutions, commonly referred to as lite clients. A large majority of multi-coin wallets or exchange wallets favour lite clients or fully custodial wallets. This is mainly due to improving the user experience and making the functionality more streamlined by bypassing the verification and blockchain download process.

A typical setup for a lite client wallet is to connect directly to a centralised server controlled, normally, by the wallet provider. Your wallet then uses the centralised server’s API to request information, like, what’s my balance, or what are my transactions. This means your wallet must trust the information provided by a centralized server and hope that the server isn't lying or providing inaccurate information.

There are a multitude of issues that could arise from this setup, including, what happens to your wallet and coins if a provider closes down? In essence, these wallet providers are the gateway to your funds, similar to that of a custodial service. Is it even possible to get your funds if the service is no longer available?

## Interchangeable SPV Wallets

Another interesting thing about Decred's implementation of the SPV model is it was built as part of the core software “dcrwallet CLI tool”, and as such, can be used on any wallet that correctly implements it. Current implementations include dcrwallet, Decrediton and CryptoPower. As an added bonus, Decred's SPV wallet is also interchangeable with the fully validating wallet if the need arises to increase your wallets security or add additional blockchain functionality.

## Benefits and drawbacks

To conclude, SPV and Lite clients manage risk and functionality in various ways. If you require the highest assurances, there is still no better option than running a fully validating wallet. But if you’re seeking a lightweight alternative to interact with the blockchain, SPV is a pretty solid option that has seen many improvements over the last few years to increase security and privacy. 

As it currently stands, the main drawbacks with using lite clients revolve around having to trust centralised third-party services instead of the decentralised network.

There is a need for lightweight wallets and currently Decred’s SPV is a shining example of how this can be achieved while still allowing users to be in full control of their coins, data, and privacy.
