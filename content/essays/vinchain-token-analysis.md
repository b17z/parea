---
title: "Vinchain Token Analysis"
date: 2018-05-15T22:32:33-04:00
---

[As published on Medium](https://medium.com/pareagroup/vinchain-token-analysis-1182764465e1)

![Vinchain](https://www.dropbox.com/s/vmd4xyzw3vh7u9u/Vinchain.jpeg?raw=true "Vinchain")

VinChain, an ERC20 token whose ICO ended on April 15th, 2018, promises to deliver a “100% trustworthy vehicle history on the blockchain” along with a spate of other non-blockchain features such as an app, vehicle performance analysis, more relevant advertisements, and, of course, a concoction of big data, machine learning, and artificial intelligence. It raised more than 12.5K ETH, equivalent to ~$9m at today’s ETH valuation.

One of blockchain’s use cases is to serve as an immutable golden source of truth, which is especially useful when there are strong incentives to obscure, delete, or alter history for financial gain. Almost any use case that tackles this challenge is a good one if it actually tackles the root cause of the problem — the contribution, storage, reliability, and availability of information.

## Analysis 

Building on blockchain is a terrible use case for this project because the service they are providing does not revolve around addressing the root cause of data issues and information asymmetry; it revolves around making payments in the same way that payments are made today. They are inserting themselves as middlemen by making a worse Carfax, but on the blockchain.

Most vehicle history data sits dormant for years before being used, beginning another multi-year revenue drought until the next revenue generating event (e.g., sale, insurance request, etc.). Building a sustainable business on this premise can only be accomplished by keeping the cost of acquiring and, more importantly, storing data extremely low. For example, Carfax, the industry leader in car history reporting, has more than 100,000 data sources and over 17 billion records, and charges only $39 for a full vehicle report.

Putting an equivalent or greater number of records (documents/data/images/etc.) on any blockchain is currently impossible (barring exorbitant fees), so on page 37 of the whitepaper, they claim that all records are hashed and the hashes are added to the blockchain, making them immutable. However, no one from VinChain checks the validity of these records nor that all records were actually added in the first place. All this would mean is that you could check that a provided document was not altered, but not whether it’s true, relevant, or any other details that actually matter to a consumer.

Their plan for extensibility is to abandon Ethereum and build out their own graphene blockchain. At the close of their ICO, their [Github](https://github.com/VinChain/VINchain-blockchain) was populated with ERC20 templates and BitShare’s graphene code libraries which they haven’t bothered renaming. But, supposing they accomplish everything they set out to do, their primary need for scale revolves around handling a greater amount of payments and document hashing.


However, there is no use case and no incentive to hash files from information providers onto the blockchain. This is for several reasons:

1. It is illegal for information providers to alter vehicle data
2. Even if it wasn’t illegal, there is little incentive for information providers to alter vehicle data
3. The only way to make money off of altered reports is to take a cut from a sale that was made which would not have happened if accurate information was provided. However, most reports do not result in sales, the report is the same price no matter how positive or negative it is, and the providers are agnostic to which car is sold.
4. If they did take a cut, it would have to be done on a very large scale to make it worth their while, highly increasing their odds of being caught.
5. The best way to commit fraud in this market is to have data originators (e.g., police departments) provide altered data, because they supply it to many information providers so no matter which one provided the vehicle history to the consumer, the lie would be consistent. You can see why this would be difficult, but without this, it would be very easy to catch cheating information providers through data inconsistencies.

They claim to increase interoperability through API’s, but these will not be interfacing with their blockchain solution. They will actually be interfacing with the information provider’s databases and then checking the provided documentation against the hashed record to ensure there were no alterations. This is useless.

Therefore their only primary need for scale is to handle a greater amount of payments. However, given their extremely limited blockchain development expertise, it is inadvisable for them to make their own.

Their token has four primary uses: (1) payment to users each time the driving and vehicle data they contributed via the VinChain app is used, (2) purchasing vehicle reports, (3) paying for API access, and (4) white labeling.

This token is primarily used to purchase vehicle history data from private, centralized databases. Per page 20 (WP), a user is able to register an account via the VinChain website, have the registration approved by the VinChain team, and then request information for a VIN (unique car identifier). VinChain then queries their information provider databases on the backend through their API’s, provides a short, free report to the user, and then gives the user an option to purchase the full report for full price. There is absolutely no need for the token for this use case as it can all be done with FIAT in the exact same fashion. The same can be said of paying for API access and white labeling. Users are entered into what equates to a loyalty program where, just like in existing programs, the platform most benefits from tokens that have been accumulated, but not used, in users’ accounts. This effectively decreases the token supply, making them appreciate in value, which benefits information providers and other vendors, but not the users themselves.

It is important to address the incentive structure for user-generated data gathered via the app. Users are not paid for generating the data itself, they are paid when it is used on this platform. This is an important distinction because the data they will be generating is not currently provided/sold in the primary purpose of this project — purchasing vehicle histories. It will only be used for all other non-blockchain add-on services, such as offering car maintenance discounts, suggesting spare parts, and other offerings which primarily benefit the vendors.

All accumulated data will sit in information provider databases, not on the blockchain. Therefore, it bears notice that while individuals are incentivized to provide their data to get paid if it gets used through the platform, nothing is preventing the information providers from selling that data off-platform to maximize their returns since it is already in their databases. And because, once on the platform, the user no longer owns their data, there is no recourse for individuals if their de-anonymized driving data is sold to their car insurance providers and adversely impacts their premiums.

Lastly, this project suffers from adverse selection. The paper mentions that VinChain will replace outdated and expensive reports from incumbents like Carfax. However, VinChain’s ability to provide car buyers with complete information will rely on them leveraging established data sources from these incumbents. Carfax has no incentive to share its data with VinChain, which is charging car buyers a premium for this data (+10%) and is trying to disrupt/disintermediate Carfax. Additionally, Carfax doesn’t need the additional distribution from VinChain, as Carfax already has brand recognition and established channel partners to distribute its data effectively.

As a result, VinChain will only be able to attract secondary or tertiary information providers that are relying on VinChain for additional distribution and likely have inferior or incomplete data relative to established incumbents like Carfax. This will make the product less compelling for car buyers, who would likely rather pay a slight premium for data directly from a trusted source like Carfax as an insurance policy that saves them from making a huge investment in a car that doesn’t satisfy their needs.

The impact of this can be seen in their token compensation structure to information providers. When a user exchanges a token for information on a vehicle, all active information providers in the network are compensated with part of the token. Initially, token allocation will primarily be linked to events (e.g., change of ownership and accidents). This incentivizes the production of more information, not better information, because there is now value in redundancy. Information providers use many common data sources (e.g., police and fire departments, DMV’s, etc.), but the best information providers are differentiated through the rarer, harder to get, or more expensive pieces of data. The VinChain information providers are then disincentivized from acquiring that data because it would require a large investment for a marginal increase in returns due to the structure of the payout mechanism (as opposed to charging a higher fee for premium data).

However, VinChain has an opportunity to significantly improve its service offering by having information providers differentiate the types of data they collect. Currently, they are all in competition, so they need to gather many of the same basic sources of data before branching out into the expensive or difficult ones. However, if the following two conditions are met, they may be able to provide much more consumer value.

1. Lock in information providers into multi-year contracts

2. Pay out more for expensive or difficult to acquire data

These conditions incentivize existing data providers and new entrants to skip many of the traditional data sources that are already being provided by others and instead specialize in niche categories. The lock in period diminishes risk because while this strategy works in this model, it would fail in an open market. By specializing, they will be able to lower their cost of acquiring this data while simultaneously increasing the value offering of the VinChain service, thereby further increasing their profitability.

## Conclusion

Overall, this project needs a significant overhaul in its business model, token economics, and incentivization structure. The project does not use blockchain to address the true pain point, the token economics harm the users, and the adoption incentive structure is geared towards low performers to provide an inferior product compared to market leaders. User ownership of user-generated driving and vehicle data was a potential saving grace, but actually relinquished ownership to information providers by storing on their databases, thereby incentivizing improper behavior.

### Credit

[Ben Rodriguez](mailto:ben@parea.io)

[Lisa Cuesta](mailto:lisa@nextgenvp.com)

## Errata

We are only human and we make mistakes. We will include any types of revisions or lapses in logic when found or brought up to us in a dedicated section at the end of each of our essays. In addition, if you have any suggestions for future essays such as formatting, or topics you’d like to see written about discussed, drop us an email at hello@parea.io or leave a comment.