## How do SPV wallets find peers?

Article in discussion...


## SPV synchronising process

**Neutron synchronising process:**
1. Headers-first synchronisation (downloads all headers from block 1?)
2. Compact Filter Headers Download and Verification (downloads all filters from block 1 or other position?)
3. Compact Filters Download and Verification (what happens here?)
4. Wallet-side checks (unpacks filter to see if there’s a related transaction?)
5. Fetch desired block

**Decred SPV synchronising process:**
1. Headers + filters downloaded and synchronised
2. Wallet-side checks (unpacks filter to see if there’s a related transaction?)
3. Fetch desired blocks 


