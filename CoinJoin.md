| Content | Description |
|---|---|
| Title               | Securing Bitcoin Transactions: The Importance and Impact of CoinJoin |
| Author              | João Paulo Sant'Anna da Silva |
| Featured text       | FIXME |
| CT link             | FIXME |
| Publish date        | YYYY-MM-DD FIXME |
| Ai checks (https://www.zerogpt.com) | Score must be lower than 25% or article is rejected for publication |

| Social Media | Links |
|---|---|
| Bison Relay post    | Title |
| Reddit link         | FIXME |
| Tweeter link        | FIXME |
| TwitterSpace link   | FIXME |
| Matrix post         | Promote your main tweet in "DCR Social Media" channel |

## Thesis statement: How does CoinJoin enhance user privacy in Bitcoin transactions, and what are its limitations?

This article will talk about the Coinjoin privacy protocol, going through:

-Brief history of the protocol

-Why it was created

-How it works

-Pros and Cons

-Could it work for Decred?

-Conclusion


## Pre-discussion, research and questions



--- ARTICLE GOES BELOW THIS POINT ---

---

# Article Title

Bitcoin is far more than a cryptocurrency, it symbolizes a revolutionary idea. Developed as a response to the 2008 global financial crisis, it presented a new type of transaction, eliminating the need for trusted institutions as intermediaries. This innovation has significantly altered the financial landscape, offering an alternative, and decentralized method for financial exchanges.

Bitcoin aimed for a high level of transparency, making it a great alternative to the shady way that the traditional financial system works. All Bitcoin transactions are public, traceable, and permanently stored in the network blockchain. 

Despite being initially private, the transaction history for Bitcoin addresses becomes public once they get used. Anyone can check an address balance ad record, making complete anonymity a difficult goal.

Noticing the privacy limitations of Bitcoin, cryptographer Gregory Maxwell developed a privacy protocol called CoinJoin in 2013, first posting the idea in a BitcoinTalk thread (https://bitcointalk.org/index.php?topic=279249.0). This model allows users to combine their BTC with other users utilizing a mixing process. Let's explore this privacy feature to understand its functionality, benefits, and potential drawbacks.

## Why CoinJoin was created

In common sense, Bitcoin is frequently seen as a tool for keeping financial matters private, but it is not as private as it seems. Each Bitcoin transaction is linked to a unique address that masks identities on the surface, but various techniques can unhide the individual behind the transaction. This can happen through methods like watching where payments come from and go to, checking IP addresses, and other online detective work. Once someone figures out your Bitcoin address belongs to you, getting your privacy back can be tough and sometimes expensive.

In comparison, regular banks keep your financial activities more private, at least for extern individuals. For example, your spending remains hidden from your family, so they can't see if you are buying things they do not support. Similarly, your employer won't have insight into the charities or causes you choose to support financially.

Even if Bitcoin users try to improve their privacy by changing their addresses more often, any past transactions can still potentially be traced back to them. This means their attempt at being more private has limited effectiveness.

Moreover, if you're careful with your privacy but trade with others who aren't (like using less secure methods), you can still end up losing privacy, affecting everyone involved. This lack of privacy can also lead to bigger problems for Bitcoin as a whole. If people can track which Bitcoins are "good" or "bad," it might lead to some Bitcoins being accepted and others not, which goes against the idea of Bitcoin where every unit is supposed to be equal. Sending and receiving Bitcoins leaves a fingerprint, and those traces are publicly registered in Bitcoin's blockchain. Anyone you send Bitcoin can look up your transactions and balance information.

## How CoinJoin works

CoinJoin aims primarily at improving the privacy and anonymity of Bitcoin transactions. Its concept is relatively straightforward: it combines multiple payments from several users into a single transaction, making it difficult to determine who paid whom. Here’s a look at how it operates:
Combining Transactions: CoinJoin combines several transactions into one, mixing the BTC being transacted. For example, if John wants to send 1 BTC, George wants to send 2 BTC, and Paul wants to send 3 BTC, a CoinJoin transaction would combine these into a single transaction. Bitcoins are mixed, and the transaction outputs distribute the mixed bitcoins to their right recipients.
Decentralization and Trust: What sets CoinJoin apart is its decentralized nature. Unlike traditional financial transactions that require a central authority or intermediary (like a bank), CoinJoin transactions are directly between users. 
Enhancing Privacy: By combining multiple payments, CoinJoin hides the trail of transactions. This process protects transaction histories from being easily accessible and linked to individual identities.
Participation and Execution: Users willing to create a CoinJoin transaction usually use a wallet or service that supports this feature. These services gather and match users who wish to mix their transactions. Once matched, the users agree on the transaction details and sign their part of the transaction, and the service combines these signatures to broadcast the complete, mixed transaction to the Bitcoin network.

Imagine a marketplace where everyone's shopping is out in the open. John starts the day with a heavy digital wallet containing 0.8 Bitcoin (BTC). He pays Paul for some goods, and just like getting a change back from a cashier, John gets 0.3 BTC back.

Nearby, George has 0.6 BTC and decides to buy something from Ringo that costs 0.5 BTC. After the purchase, George gets a little change too, ending up with 0.1 BTC.

Now, imagine there's a clever way to shop together to keep purchases private. It's like John and George put their BTC together and then split the cost of their items. This is what's known as a CoinJoin transaction.

In this smarter way of shopping, the BTC from John and George get mixed up, and they both pay out: Paul and Ringo each receive 0.5 BTC. After the deal, just like before, John gets their change of 0.3 BTC and George gets 0.1 BTC back.

The CoinJoin is like shopping with a group where everyone pitches in and then sorts out who bought what later, keeping the details away from prying eyes. It's a more private way to handle their marketplace business, where the trail of who bought what is hidden, making the day's trade a little less public.

## Benefits of CoinJoin
Increased Anonymity: CoinJoin provides an additional layer of anonymity to Bitcoin transactions, making it difficult for outside observers to track and link transactions to specific users.
Decentralization: It reinforces the decentralized nature of Bitcoin by eliminating the need for trust in centralized mixing services.
Prevention of Censorship and Blacklisting: By mixing coins, CoinJoin helps prevent the potential blacklisting of coins based on their transaction history, preserving the fungibility of Bitcoin.

While CoinJoin significantly increases privacy, there are still ways to narrow down the anonymity provided by this protocol. Let's go through some of the potential flaws/limitations of CoinJoin:

Traceability of Pre-Mixing and Post-Mixing Transactions: If an observer can link the pre-mix or post-mix addresses to a user or set of users, the effectiveness of CoinJoin in obscuring the transaction source is reduced.

Address Reuse: Users must adhere to the best practices for address generation. Those who keep reusing addresses may compromise their privacy.

Amount correlation: If a user mixes an amount that stands out or is less common in the mix, it could be more easily traced, especially if this same amount appears in the next transactions. User's behavioral patterns, such as consolidating funds after mixing, could also provide clues to their identity.

Non-Uniform adoption: The privacy and efficiency of CoinJoin also depend on how widely it is adopted. If only a small group of users are mixing transactions, it may be easier to identify those users identity.

## CoinJoin Wallets

CoinJoin is a Bitcoin-only protocol. The way the use of it differs depends on the wallet/mixer that you are using. Some of the most known privacy-focused Bitcoin wallets are Wasabi, Samourai, and Joinmarket. Let's go through some details concerning anonymity sets and fees for each one of them:

WabiSabi Wallet

The WabiSabi Wallet charges a coordinator fee of 0.3% for CoinJoin transactions of more than 0.01 BTC. The coordinator fee is charged to cover the service costs of coordinating the mix. For amounts of 0.01 BTC or below, no coordinator fee is charged.

An anonymity set is basically the pool of users participating in a specific transaction. The size of an ideal anonymity set in a WabiSabi can vary from 50 to 100 participants in a CoinJoin round. This means your transaction would be mixed with those 49 to 99 other users.

Samourai 

Samourai Wallet uses Whirlpool, a CoinJoin implementation created by its developer team. The service employs a fixed fee structure. Fees range from 5,000 satoshis for the smallest pool (100,000 satoshis) to 1,750,000 satoshis for the largest pool (50,000,000 satoshis). Each satoshi is equal to one hundred millionth of a Bitcoin (0.00000001 BTC), it is the smallest Bitcoin unit.

Whirlpool's anonymity sets vary based on real-time participation within each pool. Since the number fluctuates the user is encouraged to go through multiple mixing rounds to increase their transaction's anonymity. Samourai wallet model aims to provide a balance between costs and privacy.

Bitcoin mixers

There are also options for those wanting a fast and user-friendly Bitcoin mixer. Websites like Whir and Tumber.io let you mix your Bitcoin by entering the Bitcoin address where you want to receive the mixed BTC. After that you need to send the BTC to the address generated by the tool, they will be sent to a BTC pool, where your Bitcoin will be mixed, and after that sent to the address you entered in the first step.

Whir has a 1% fixed coordinator fee.
Tumber.io fees start at 0.4% and vary according to the amount mixed.

## Could it work for Decred?

As we said before, CoinJoin is a tool exclusive to Bitcoin. Other coin mixers have been developed by other projects, like the Stake Shuffle protocol from Decred.

StakeShuffle is a privacy protocol available at Decred Wallet Decrediton. It is a non-custodial process used to obfuscate ownership of DCR coins. If you use StakeShuffle your outputs are going to turn fully anonymized, and peers of the server won't be able to link outputs and inputs. This technology is based on a paper called " “P2P Mixing and Unlinkable Bitcoin Transactions” by Ruffing, Moreno-Sanchez, and Kate. This system uses a more efficient version known as DiceMix Light, making the process quicker. Although it successfully hides who is sending money to whom, the amounts being sent are still visible to everyone. For added privacy, each mixing transaction uses the same amount of money, known as a fixed denomination.

## Moving Forward

CoinJoin can be highlighted as one of the most used privacy protocols in the crypto market. It is a tool that complements and contrasts with the transparent nature of Bitcoin. For starters learning that Bitcoin is not really anonymous can be a shock, but CoinJoin was created to address this issue.

Have you ever used CoinJoin? Do you think this mixing is better provided by any wallet? Please share your opinion with us in the comments section!
