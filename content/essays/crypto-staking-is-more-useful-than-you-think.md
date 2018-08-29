---
title: "Crypto Staking is More Useful Than You Think"
date: 2018-06-28T22:32:33-04:00
---

[As published on Token Foundry's Medium](https://medium.com/tokenfoundry/crypto-staking-is-more-useful-than-you-think-8cb3cfe06587)

![Staking](https://www.dropbox.com/s/5mmsfbt3xb737si/Staking.png?raw=true "Staking")

Proof-of-Stake (PoS) consensus mechanisms are a highly controversial topic in the crypto ecosystem as Ethereum is implementing Casper and many consumer tokens rely on staking economic incentive structures. However, while staking may be a new and relatively untested blockchain consensus mechanism, it has been widely used as an economic mechanism for centuries. This article will examine such cases and explain what staking is, how it works, and why it’s a crucial tool in token design and incentive structures.

## What is crypto staking?

When it comes to blockchains, staking is the action of putting up a balance of tokens as a security deposit for the right to validate transactions in a PoS consensus protocol. Nodes that validate transactions correctly are rewarded with tx fees while those that break the protocol’s rules are penalized and have their stakes slashed, potentially losing small amounts for light infractions– or their entire stake for significant breaches. The more a node stakes, the more likely it is to be selected to validate the next block due to simple “skin in the game” principles as they have more to lose from breaking the rules and are therefore highly incentivized not to do so. Put in plain English…

> Staking is securing the right to perform a service for a network that meets quality assurance criteria.

## Staking - past and present

This abstract definition can be clearly illustrated by examining the NYC taxi ecosystem, its breakdown, and the medallion “staking” solution.

During the Great Depression in the 1930s, New York City had more than 30,000 cabs in operation. In these tough economic times, the drivers would compete fiercely for customers– often resorting to underhanded tactics like renting their back seats out to prostitutes. Fees were cut drastically, driver and passenger safety were compromised, and cleanliness standards plummeted. Taxis at this time were viewed as a menace to society and consumers pushed politicians to take action.

In 1937, NYC Mayor Fiorello LaGuardia introduced the Haas Act, establishing and mandating the taxi medallion system still in use today. It limited the amount of medallions (and therefore taxis) available which brought the supply of taxicabs closer to the level of service the public demanded while simultaneously establishing a quasi code of conduct to ensure a high level and quality of service*. Taxi drivers now had to purchase the medallion for an initial price of $10 and agree to follow established rules while performing the services. Failing to do so would result in fines, tickets, and even medallion confiscation.

Having skin in the game in prior times meant a financial and reputational investment that a central authority would have to control and monitor. Blockchain decentralizes this responsibility and enables anyone to invest in the network and utilize it.

Virtue Poker, a Token Foundry project, used a staking mechanism to solve a significant challenge that has plagued the online poker industry: ensuring game integrity while removing centralized counterparty risk (deposit misappropriation, stacked decks, etc.). They did so by creating the Justice Pool, a group of nodes that stake Virtue Player Points (VPP) and serve as impartial facilitators and arbiters in Virtue Poker games. They are compensated for these services (outlined below) through tx fees, but if a Justice is caught cheating, colluding, or misreporting hand results, that Justice’s stake is seized and is kicked out of the Justice Pool.

*Core functions of Justices explanation from the [Virtue Poker whitepaper](https://virtue.poker/public/Virtue-Poker-White-Paper-0.9.pdf)*:

> *4.2.2.1 Dispute Resolution*
In the rare instance two peers at a table disagree as to the state of the table at the end of a hand or a game, a Justice resolves the dispute in real-time and awards the pot to the winner.

> *4.2.2.2 Data Feed*
Each Justice submits each action of every hand to IPFS so hand histories can be stored. This is required by gaming regulatory bodies, and enables essential services such as collusion detection, bot detection and multi-accounting identification.

> *4.2.2.3 Partial Storage of Player Encryption Keys*
The “Dropped Player Problem” of Mental Poker occurs when a player drops out of a hand prior to its completion. This is problematic, as all players must share encryption keys for community cards to be revealed and for a hand to be completed. Using Shamir’s Secret Sharing, each player’s keys can be encrypted and split amongst all players plus the Justice. If the player drops out for any reason, the Justice can request the pieces from each player and decrypt the assembled pieces so that the hand can be completed.

## What's at stake

The challenge with centralized staking mechanisms (franchises, alcohol licenses, etc.) is that they have a long, broken behavioral feedback loop. A McDonald’s franchisee that has invested a significant sum to obtain the franchise, build the store, hire workers, and order supplies, can still fall far short of corporate performance standards. In order to rectify the situation, investigations have to be conducted, threats need to be made, surprise visits paid, and a lot of time and money invested. At the end of it all, incentives are misaligned because corporations makes more real, immediate income from keeping a problematic store open than the perceived potential future loss from diminishing customer preferences for McDonald’s after bad experiences.

Blockchain staking mechanisms solve for that problem because feedback in the forms of tx fee payouts or stake slashing always occur before the individual is able to access their money, but after they have provided the services. This review comes not from a centralized party, which is constrained by time and resources, but in real-time by every other participant in the network. In addition, whereas in centralized systems large services providers may try to bend the rules in their favor, they are disincentivized from doing so in decentralized systems due to the transparency afforded to all participants. Any discovered manipulation event will significantly decrease the overall value of the network, hurting the largest participants most.

There are additional reasons for why staking mechanisms make sense for many projects we come across.

## Why staking works

First, staking with a network-specific token (as opposed to ETH) enables the most accurate pricing to access the network because token prices factor in all public knowledge about a network’s true value in real time. Staking requirements can then be set based on proportion of network value instead of it’s fiat or ETH equivalent, which would need constant adjustment based on the network’s value. This equilibrium is not set by a centralized agency (e.g. government organization), but by the market.

Second, buying into most networks is impossible using Proof-of-Work because most tokens will not deserve or require their own ASIC’s and will just use coin-agnostic GPU’s. Whereas Bitcoin miners are truly invested in the protocol because there are few alternatives for their SHA-256 ASIC hash power, GPU miners are not invested in the protocol and can simply switch to another one at will. Staking forces individuals to contribute value into the network by buying tokens with highly liquid cryptocurrencies, making them truly vested co-owners.

Third, staking significantly diminishes the threat of a 51% attack for smaller networks. Whereas it is is almost impossible to amass enough hash power to attack Bitcoin, it is easy to buy or rent the computing power necessary to constitute a majority share of smaller Proof-of-Work tokens. Staking requires massive initial investment into the network to obtain 51% of the tokens, which is already difficult, but this challenge is further compounded by a lack of liquidity as a successful attacker attempts to convert his loot into more liquid cryptocurrencies.

Lastly, staking is the crucial monetary incentive mechanism that was missing in “goodwill” projects. Mesh networks, for example, long relied on individuals goodwill and were unable to effectively route network connections as gateway nodes could misrepresent their capabilities or go down unexpectedly with no penalties. Adding verifiable quality and price metrics to a Babel routing protocol puts money on the line and incentivizes good node behavior. We expect to see additional projects target similar areas of work, opening up a new field of innovation.

## Betting on the future

In conclusion, staking mechanisms are crucial tools to strengthen networks, build vested communities, and enable new business models. They are also especially useful in utility or consumer token models to resolve the medium of exchange velocity problem while providing true utility value.


### Note
*One can make the argument medallions may no longer be needed due to mechanisms such as Uber’s “attestations” (identity, rating system, etc.) which have alleviated the initial concerns that preempted medallions.*