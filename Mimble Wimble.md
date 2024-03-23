| Content | Article about the privacy protocol MimbleWimble |
|---|---|
| Title               | MimbleWimble Explained: How It Works and Why It Matters |
| Author              | João Paulo Sant'Anna |
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

## Thesis statement: What role could MimbleWimble play in shaping the future of secure, private, and scalable digital currencies?

This article will talk about the MimbleWimble privacy protocol, going through:

-Brief history of the protocol

-Why it was created

-How it works 

-Pros and Cons

-Could it work for Decred?

-Conclusion

---
--- ARTICLE GOES BELOW THIS POINT ---

---

# Mimblewimble, the Enchantment of Anonymity

If you have read the Harry Potter books the name Mimblwimble may be familiar. It's the name of a spell that ties the target's tongue to keep them from spreading secrets or casting other spells. In the real world, this funny word was chosen by an anonymous developer who used the name Tom Elvis Jedusor, to name a privacy protocol. This protocol can be described as a cloak of invisibility for crypto transactions, ensuring that user information remains hidden.

The Mimblewimble protocol offers a new structure for blockchain technology that emphasizes scalability, fungibility, and especially privacy in transactions. Let's investigate this protocol to learn how it functions, and understand its advantages and potential drawbacks. 

## Why was MimbleWimble created?

On August 2nd, 2016, a person using the pseudonym Tom Elvis Jedusor, the French name for Voldemort, made a brief appearance on a Bitcoin research IRC channel. The person shared a document from a Tor hidden service, titled "Mimblewimble," before exiting the channel. This document proposed a novel blockchain architecture distinct from Bitcoin's, featuring transaction merging, confidential transactions, and the ability for full verification of the chain's current state without necessitating new users to review the entire coin history.

Mimblewimble was designed as a cryptocurrency protocol that focuses on enabling a compact and efficiently verifiable transaction history, using minimal computing resources. It also prioritizes user privacy through confidential transactions and an obscured transaction graph. The main objectives of the protocol are addressing scalability issues, and keeping transactions private.

Key characteristics of Mimblewimble include:

Direct value transfers between parties.

Confidential transactions that obscure the amount transferred.

Reduced data and processing requirements for new participants, scaling with the system's current state rather than its entire transaction history.


## How does MimbleWimble work?

MimbleWimble can be described as a tool for making efficient and private cryptocurrency transactions. Imagine you're sending secret messages that can only be opened by someone with a specific key. In MimbleWimble, when you send cryptocurrency, the amount you send is hidden using a secret code (called a "blinding factor"). This means only you and the person receiving the money know how much is sent.

Even though the amount is secret, everyone can still ensure the transaction is fair (no extra money out of thin air) by checking that what's sent equals what's received, without actually seeing the amounts. This is like knowing a box is full of apples without knowing how many apples are inside.

Transactions in MimbleWimble can be combined in a way that makes it hard for outsiders to figure out who sent money to whom. This is similar to mixing several messages so that no one can tell which message came from which sender. This mixing helps make transactions even more private.

However, MimbleWimble can't do some of the tricks that other protocols can, like creating special conditions for transactions or swapping currencies directly without a middleman. But it has a cool trick: as transactions are combined and old, unnecessary data is removed, stopping the history of transactions from growing too big. This keeps things running smoothly without needing a super-powerful computer.

(Animated video explaining Mimblewimble)
https://www.youtube.com/watch?v=aIh0XjhNgBc

## Elliptic Curve Cryptography (ECC)

Talking a little about the technical part, MimbleWimble uses a form of cryptography known as Elliptic Curve Cryptography (ECC). ECC enables the protocol to confirm the accuracy of transaction amounts and the identities of the sender and receiver, all while keeping this information private. The "discrete" aspect in logarithms, which ECC is based upon, refers to a mathematical field focused on distinct values, incorporating areas like probability and set theory, thereby enhancing the protocol's security.

With the use of the Elliptic Curve Cryptography, Mimblewimble can achieve 3 main goals for its users:

Privacy Protection: MimbleWimble ensures that the transaction details remain a secret between the sender and the receiver. Only they can know how much crypto was sent.

Transaction Legitimacy: It verifies that transactions are valid without the need for those to be signed publicly, maintaining user anonymity.

Enhanced Efficiency:  The protocol achieves greater efficiency and scalability by generating smaller blocks of data. This approach prevents the blockchain from becoming excessively large and difficult to manage over time, a challenge often faced by networks like Bitcoin.

Beyond ECC, MimbleWimble protocol integrates technology used by cryptographic protocols, such as:

Dandelion: This protocol obscures the identities of the sender and receiver, adding another layer of privacy.

CoinJoin: This technique complicates the task of tracking transaction paths. By amalgamating multiple payments from different senders into a single transaction, CoinJoin masks the public addresses involved. This not only enhances privacy but also streamlines blockchain data storage by reducing the need to retain extensive transactional information beyond the essential inputs and outputs.

## Could it work for Decred?

Decred utilizes Stakeshuffle as its privacy protocol. It is responsible for mixing multiple transactions, and hiding who sent coins to whom, without the need for third parties. If you want to learn more about Stakeshuffle click here (https://docs.decred.org/privacy/cspp/overview/?ref=cypherpunktimes.com)!

To understand more if Mimblewimble could be a good addition to the Decred blockchain I went through its implementation on Litecoin. Also highlighted some of its advantages and disadvantages.

Mimbleimble was implemented on Litecoin by the use of a feature called Extension Blocks. The implementation launched in May 2022, and made it possible for Litecoin holders to use the new privacy features by moving their Litecoin into these Extension Blocks. These blocks are responsible for hiding the transaction information.

To engage with this privacy feature, users perform a "pegging-in" transaction to move their Litecoin into an Extension Block, using a specific MimbleWimble Extension Block (MWEB) address. These transactions are facilitated by a special transaction known as the HogEx (Hogwarts Express), which processes both the pegging-in of funds to the Extension Block and the pegging-out back to the main, transparent blockchain. The HogEx also manages the Extension Block balance, adjusting it for incoming and outgoing transactions.

While the majority of Litecoin transactions continue to operate on the transparent main blockchain, the introduction of MimbleWimble via Extension Blocks provides a significant step forward in offering privacy options to users.

Implementing MimbleWimble on the Decred blockchain is theoretically possible. Decred governance model and adaptability could facilitate the consideration and potential implementation of MimbleWimble if there was enough community support.

The technical integration of MimbleWimble would require a lot of development effort and a thorough review process to ensure that it aligns with Decred’s security, privacy, and scalability goals. One of the main considerations would be how to integrate MimbleWimble's privacy features with Decred's existing features, such as its governance system, and the Stakeshuffle protocol.

There are also some Mimblewimble drawbacks that need to be taken into consideration: 

Slower Transactions: Networks that use Confidential Transactions, like MimbleWimble, can be slower than others such as Ripple (XRP) and proof-of-stake networks like Solana and Cardano. This is because the data for Confidential Transactions is larger, which can slow things down.

Quantum Computer Risk: MimbleWimble relies on digital signatures to work. This makes it potentially more at risk from future attacks by quantum computers, which might be able to break these digital signatures. Decred has overcome this problem with post-quantum secure mixing on stakeshuffle.

## Moving Forward

Is always interesting to learn about privacy protocols, especially one that is much commented like Mimblewimble. Do you think it could be a good addition to the Decred blockchain? Let your voice be heard in the comment section below!

Sources:

A Formal Analysis of the Mimblewimble Cryptocurrency Protocol 

Non-interactive Mimblewimble transactions revisited

Explaining MimbleWimble: the privacy upgrade to Litecoin

