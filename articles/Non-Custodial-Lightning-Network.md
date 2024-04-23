| Content | Description |
|---|---|
| Title               | Non-Custodial Lightning Network |
| Author              | Phoenix Green |
| Featured text       | Is Decred's Lightning Network non-custodial? Addressing the misconceptions and misinformation surrounding the non-custodial nature of the Lightning Network. |
| CT link             | https://www.cypherpunktimes.com/is-decreds-lightning-network-non-custodial/ |
| Publish date        | Apr 23, 2024 |
| Ai checks (https://www.zerogpt.com) | Score = 0% |

| Social Media | Links |
|---|---|
| YouTube link        | https://youtu.be/48muAQplR_4 |
| Podcast link        | https://podcasters.spotify.com/pod/show/cypherpunktimes/episodes/Is-Decreds-Lightning-Network-non-custodial-e2ip4rd |
| Reddit Link         | https://www.reddit.com/r/decred/comments/1cbe7zn/is_decreds_lightning_network_noncustodial |
| Bison Relay Post    | Is Decred's Lightning Network non-custodial |
| Twitter full video  | https://x.com/decredproject/status/1782855308273987801 |

| CT tweet            | https://x.com/cypherpunktimes/status/1782811798145519947 |
| YouTube tweet       | https://x.com/DecredSociety/status/1782810828254666973 |
| Twitter clip 1      | FIXME |
| Twitter clip 2      | FIXME |


## Thesis statement

Is Decred's Lightning Network non-custodial? The aim of this discussion is to highlight and find answers to the misconceptions and misinformation surrounding the non-custodial nature of the Lightning Network.

## Pre-discussion, research and questions

* Do peers need to run an always on LN node to use the Lightning Network in a non-custodial nature?
* Do peers need to be on-line at the same time to transact over the Lightning Network?
* Do peers need to give up custody of funds to use the Lightning Network?
* Do peers need to trust centralised middleman / servers to use the Lightning Network?


---
--- ARTICLE GOES BELOW THIS POINT ---

---

# Is Decred's Lightning Network non-custodial?

Is Decred's Lightning Network non-custodial? This question comes up frequently. The short answer is “yes”, but to be more specific we’ll need to look into some general misconceptions, which are plenty. For this discussion, we’ll focus on how Bison Relay has implemented the Lightning Network.

## Do peers need to run an always-on LN node to use the Lightning Network in a non-custodial nature?

The Lightning Network node or LND is a core part of Bison Relay, as is DCRD. When you open Bison Relay, you instantly start connecting and synchronising with the Decred blockchain and communicating with the Lightning Network. No third-party tool or connection is needed to achieve this, it’s all packaged in Bison Relay.

This process is also kept lightweight and efficient through the use of Decred’s Simplified Payment Verification (SPV) integration. Which allows Bison Relay users to download a much smaller version of the blockchain, whilst still verifying transactions and synchronising with the blockchain independently.

Although the Bison Relay doesn’t need to be always-on, e.g. 24 hours a day 7 days a week, it should remain active whilst you’re processing transactions or opening and closing channels. In most instances, a Lightning Network transaction will complete in under a second, so the commitment here is generally very minimal. 

If you are someone, like a merchant, who is aiming to receive many spontaneous transactions. It’s best to remain connected for longer periods of time, with the recommendation being an always-on version of Bison Relay. But for the average user, this isn’t a necessity.

## Do peers need to be online at the same time to transact over the Lightning Network?

In most cases, yes. For instance, if you are buying an item from an online shop or a user, the transaction won’t go through if they are not online. It’s for this reason, the recommendation for merchants or users expecting spontaneous payments should run an alway-on version of Bison Relay. This way, when a user buys something from them, the transaction will complete without delay.

In terms of messaging users on Bison Relay, it’s not a requirement for both users to be online at the same time. Bison Relay uses routing nodes to relay messages, these nodes will hold messages for up to 30 days or until the user or users come back online.

Routing nodes are a more centralised mechanism of Bison Relay’s Lightning Network that allows for more seamless communications between peers. It’s important to note that these services never take custody of your funds and don’t have access to the messages they are routing.

## Do peers need to give up custody of funds to use the Lightning Network?

No. On Bison Relay, the user is in full control of their funds at all times. The platform is fully non-custodial and trustless. Not all Lightning Network platforms have been built this way. Some LN platforms have been known to insert themselves as custodians of users' funds to help with the user experience or to extract fees for transactions and interactions. Some LN providers have prioritised user experience over non-custodial, peer to peer technology. 

Decred has a core mission to provide non-custodial peer to peer technology. The Lightning Network and SPV mode have been tightly integrated into the Decred blockchain, making for an extremely lightweight, efficient and secure experience.  

## Do peers need to trust centralised middleman / servers to use the Lightning Network?

There are some tradeoffs here, but generally the answer is no. All areas of the platform can be run by the individual, and there is no need to include a middleman to communicate and make payments over the Lightning Network. But to improve the user experience, there are some services available to make the process a lot more streamlined and user-friendly.

The two main services are “Bison Relay Hubs” and “Lightning Network Liquidity Providers”.

Connecting to a “Bison Relay Hub” allows you to connect to pretty much everyone on the LN network and reduce the hops needed from many to one. The fee for this service is 1 atom (0.00000001 DCR) per 1 KB of data sent or received. This is a standardised fee which helps the network remain consistent with ultra-low fees and is a mechanism to help prevent spam and DOS attacks. It’s important to note that “Bison Relay Hubs” never take custody of your funds and if you’d prefer not to use this service you are not required to do so.

The second service available, “Lightning Network Liquidity Providers” helps to streamline the ability to receive funds from other users, by allowing inbound liquidity to your LN channels. The fee for borrowing liquidity from a provider is 1% of the amount borrowed. This inbound liquidity can be left open for long periods of time or closed once the liquidity has been used. As a side note, it’s best to only borrow the amount you’ll realistically need, e.g. if you are expecting to receive 0.1 DCR over the next 30 days, set up your liquidity at 0.11 DCR. Setting up larger amounts than required will likely lead to unnecessarily expenses.

Once again, this service never gains access to your funds and there is no requirement to use it if you’d prefer not to. 

Hopefully, this answers a lot of the misconceptions surrounding the Lightning Network and how Decred’s Bison Relay has implemented it. Decred’s Lightning Network has been built as a core piece of infrastructure. It’s not an add-on or after thought. Many years have gone into building it from the ground up and making sure it works as intended and as part of the blockchain. Decred has proven, when it’s done correctly, the Lightning Network is leaps and bounds ahead of the majority of other scaling blockchains and layer 2 options.
