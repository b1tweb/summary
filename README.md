# BitWeb Summary

- [Multichain Overview](#multichain-overview)
    - [Network Structure](#network-structure)
    - [Governance Platform and Consensus](#governance-platform-and-consensus)
    - [Web Computer](#web-computer)
    - [Parachains and Bridges](#parachains-and-bridges)
        - [IQ](#iq)
        - [Orbit](#orbit)
        - [Torus](#torus)
        - [Tags](#tags)
        - [Bench](#bench)
        - [Route](#route)
        - [Inspire](#inspire)
- [DAO Overview](#dao-overview)
    - [DAO Purpose](#dao-purpose)
    - [The Number Of Token Holders](#the-number-of-token-holders)
    - [Token Holder Powers](#token-holder-powers)
    - [When Network Will Be Fully Operational and Decentralized](#when-network-will-be-fully-operational-and-decentralized)
    - [Network's Essential Functions and Operations](#essential-network-functions-and-operations)
    - [How Token Holders Make Decisions](#how-token-holders-make-decisions)
- [Application Overview](#application-overview)
    - [BitHost](#bithost)
        - [WebChip and BitBox](#webchip-and-bitbox)
        - [BitHost DAO](#bithost-dao)
        - [Future BitHost DAO Functions](#future-bithost-dao-functions)
        - [Purpose Of BitHost](#purpose-of-bithost)

### Multichain Overview

_**"My bias was always to build decentralization into the net. That way, it would be hard for one group to gain control. I didn't trust large central organizations. It was just in my nature to distrust them."**_ -  **Bob Taylor, ARPANET Chief Engineer**

BitWeb is a multi-chain that forms both a decentralized autonomous organization and a decentralized alternative to the World Wide Web. BitWeb combines decentralized and scalable computing, smart contracts, finance, DNS, edge networking, storage and tokenization into a single ecosystem that is globally elastic. BitWeb’s ecosystem is designed so that its users and contributors power its infrastructure, decide on how it grows and ultimately how it runs on a day-to-day. In addition, its development platform is designed for novice developers, so that the development process is greatly simplified. This allows any web developer to develop on top of a truly people-powered ecosystem, while ensuring their application(s) can scale across any web services, to as many users as possible. BitWeb is the fourth iteration of the World Wide Web and the most efficient and scalable to-date.


#### Network Structure

BitWeb is a multichain built on top of the Substrate framework, similar to how networks like Polkadot and Kusama are built using the Substrate framework. Like Polkadot, BitWeb is made up of a root “relay” chain that houses its governance platform, relay consensus mechanism, cross-chain communication protocols and sub-chain architecture, along with its native currency “B1T.”  The relay chain works alongside sub-chains, known as "parachains," that operate in parallel with the root chain, and "bridge chains," which ultimately help facilitate interoperable communications between wholly unrelated blockchain and multichain networks that exist outside of the BitWeb ecosystem. BitWeb's entire network is managed by its users, via a groundbreaking governance platform, essentially forming an entire Internet that functions as a decentralized organization - exactly what the Internet was designed to be from its very inception.

BitWeb's relay chain and its parachains, all solve the "blockchain trilemma" as coined by Vitalik Buterin. Buterin said that a blockchain looking to achieve security, scalability and decentralization, could only achieve two of the three. BitWeb has achieved all three, through [Proof-of-Archival Storage (PoAS) consensus](https://www.parity.io/blog/subspace-archiving-kusama-with-onfinality), [a secure randomness beacon](https://eprint.iacr.org/2017/573.pdf), [erasure-based distributed archival storage](https://faculty.math.illinois.edu/~duursma/CT/RS-1960.pdf), [Flow's decoupling of consensus and computation](https://arxiv.org/pdf/1909.05821.pdf), [Flow's verifiable computation](https://arxiv.org/pdf/1909.05821.pdf), [Buterin's verifiable fraud proofs](https://arxiv.org/pdf/1809.09044.pdf), [PoReps](https://filecoin.io/proof-of-replication.pdf), [high-throughput transaction processing for secure vertical scaling](https://arxiv.org/pdf/1810.08092.pdf), [data availability sampling](https://arxiv.org/abs/1905.09274), [super-light clients](https://eprint.iacr.org/2019/226), [Free2Shard's adaptive-adversary-resistant super sharding algorithm for flat horizontal scaling](https://arxiv.org/abs/2005.09610) and [Taiji's fast confirmation protocol](https://eprint.iacr.org/2020/1470). This essentially allows BitWeb's relay chain and each of its parachains, to scale to 2^16 shards (65,536 shards), where each shard is capable of processing nearly 7,380 transactions per-second (483,655,680 tps) BitWeb's relay chain and its parachains are what can only be referred to as "super sharded," putting academic proposals like Free2Shard, Taiji and Prism into practice, to securely and efficiently scale horizontally and vertically to what we estimate at minimum will be 400 million transactions per-second. 

Below is a summary regarding BitWeb's governance, consensus and infrastructure functionality.

#### Governance Platform and Consensus

BitWeb’s governance platform is meant to transform BitWeb into a decentralized autonomous organization (DAO) at launch, allowing the community to handle its day-to-day operations and future direction via on-chain proposals and its on-chain treasury. BitWeb utilizes the Nominated Proof-of-Stake consensus algorithm, where community nominators, an elected 13 member Governance Council and 297 validators collectively maintain and secure the network. Nominators operate individually or collectively via on-chain nominator pools to nominate Validators, as well as the on-chain Governance Council.

The elected Council initiate software updates, work orders, and other initiatives through on-chain referendums that either derive from community proposals or through referenda that are generated by Governance Council members. Any community member can create a proposal for just about anything. Examples of a proposal may be the hiring of developers to develop a new website, the hiring of a graphic designer to develop new branding or even the hiring of a lawyer to oversee an acquisition by the DAO. All of these proposals can be voted on by the community and advanced to a Governance Council vote. The Governance Council can also bring their own emergency referenda, that is not initially proposed by community members, for certain issues that are defined under emergencies in the network constitution. 

The multichain has the ability to connect and communicate with sub-chains that run in parallel with the relay chain known as parachains. Validators work together to achieve consensus on parachains, as well as the root relay chain. Parachain nodes utilize full-node participants known as “collators” who maintain the full state of the underlying parachains and run a full node of the relay chain as well. Collators are responsible for collecting transactions on their parachain, forming block candidates and producing state transition proofs, based on those blocks, via transaction execution, for relay-chain based validators to validate.  Parachains utilize a consensus protocol that is compatible with the relay chain’s validators, which makes this sort of functionality possible.

BitWeb, as well as its parachains, are totally compatible with wholly unrelated blockchain platforms like Bitcoin, or other Substrate-based blockchains like Polkadot, using Substrate’s XCM interchain messaging format. This is made possible via “bridge chains,” which are directly connected into the BitWeb ecosystem like a parachain, only they handle their own consensus and do not use the relay chain for security. Bridge chains and the native chain they’re related to utilize their own security policies and protocols. Bridge chains simply allow BitWeb’s relay and its parachains, to communicate directly with the blockchain that a particular Bridge chain is onboarding. This means that Bitcoin could theoretically be moved between Bitcoin’s native network and a parachain on BitWeb’s multichain network.

BitWeb’s goal is to reimagine the application layer of the Internet, by bringing together the best and scalable blockchain protocols, under a single roof, where these protocols and their growth are totally regulated by the community themselves and interoperable with one another.

#### Web Computer

We began looking at a decentralized web as simply a people-powered and people-regulated decentralized services layer that takes the place of the centralized services layer that exists as a sub-layer to the Internet’s application layer. While that's a mouth full, it's the only way one could even begin to vision a decentralize web itself, considering that Web 1.0 and Web 2.0 were giant applications in their own right, made up of many protocols and interoperable networks. While the Internet’s infrastructure backbone is certainly centralized, its protocols aren’t. Our realization that a majority of the Internet’s centralization takes place at the application layer, led us to reimagine this layer as a massive distributed computer, where different components of the computer, could provide a set of specific services, all in parallel, while also maintaining interoperability with one another. In reality, these services are nothing but protocols at the application layer, just as SMTP and other protocols are as well, only these protocols and the networks that surround them are completely interoperable and cannot possibly be centralized - the only providers of services can be the users themselves. The plug-and-play nature of parachains and bridges, means that any and all decentralized services that are needed by decentralized application developers can easily be created and onboarded in the future. Thanks to bridges, those services don't have to be native to the BitWeb ecosystem either.

While BitWeb will initially launch as a DAO with its relay chain, over time, parachains that provide specific decentralized web services will be launched and hopefully inserted as parachains. Specifically, Octal Labs, who is being funded by BitWeb’s foundation to create the BitWeb multichain, is also developing six Parachains and a single Bridge chain, all of which will eventually become interoperable with BitWeb’s relay. We look at these 6 sub-chains as core components, that will provide high-performance barebones services and infrastructure for Web3/4-based applications, while providing a definite performance enhancement, when compared to other competing services and infrastructure platforms. 

#### Parachains and Bridges 

Below, is a short explanation of BitWeb's integrated parachains and bridges.

##### **IQ**

IQ is a bridge chain, that is able to scale to 2^16 shards, like BitWeb's relay chain. It utilizes multiple participants to achieve consensus, verify computation and finalize transactions on-chain. IQ utilizes an EVM-based smart contract engine and PoAS consensus, where "farmers" (similar to Bitcoin or Ethereum miners) farm data and in-turn, are rewarded IQ tokens at each block. IQ tokens can only be rewarded for farming or computation efforts. In other words, IQ tokens are earned in return for network-based proofs-of-work. IQ has the capability of storing exabytes of on-chain data thanks to its erasure-based distributed storage network and the other features mentioned above. 

Any Solidity-based smart contract can be deployed on IQ, meaning, all smart contracts on networks like Ethereum, Polygon, Avalanche and others, can be moved to IQ's more performant network, in just a few steps. Since the network can store exabytes of data permanently and can process millions of smart contract-based transactions per-second, IQ is looked at as the computation and permanent storage component for the network.

##### **Orbit**

Orbit is a parachain that forms an on-chain marketplace for [Hypercore](https://hypercore-protocol.org/)-based data. Orbit will ensure that data from the world's most powerful distributed data network is always reachable, connecting developers who want to distribute data and resource providers who want to earn for storing and replicating data, over specific data epochs.

Orbit differs from competing storage networks like FileCoin and Sia, considering both are based around IPFS's file storage protocols. Hypercore, unlike IPFS, can handle much more than just files - it handles the distribution of pure binary data on a peer-to-peer basis. This allows Hypercore to handle files like IPFS, with a simple module like [Hyperdrive](https://hypercore-protocol.org/guides/modules/hyperdrive/), a real-time distributed file-system that is far more performant than IPFS, due to its barebones architecture. Hypercore has even been used to distribute multi-writer key-value databases like [Hyperbee](https://hypercore-protocol.org/guides/modules/hyperbee/) on a peer-to-peer basis, with over a trillion records. We believe its use-cases are endless.

Orbit allows for dApp developers to utilize Hypercore's network to distribute raw data, whether its a media file, a file system, a database or even the data related to a phone call, efficiently and redundantly, without worrying about uptime. We believe Orbit is the cache component of network, allowing dApps to store data for a specific period of time and retrieve said data, quickly and efficiently.

Orbit's ORB token will be distributed freely to all of BitWeb's users via an air drop.

##### **Torus**

Torus is a parachain that forms a peer-to-peer marketplace for cloud computing resources via Torus's resource providers. Network participants can easily provide their available computer resources to the network, which are containerized and provided to developers who wish to deploy containers for their applications. Resource providers utilize Torus's core node software which is based around Kubernetes, allowing resource providers to effortlessly provide cloud computing resources to those in need.

Torus ensures that Web2 applications like WordPress and other Web2-based centralized web applications, can still utilize Web2-like infrastructure, on a Web3 basis. Torus is comparable to Akash and Flux, with much better performance and scalability. Torus is viewed as the "legacy compute" arm of the network, allowing for the onboarding of legacy applications from previous iterations of the Web. 

Torus's "SERVER" token will be distributed freely to all of BitWeb's users via an air drop.

##### **Tags**

Tags is a parachain that forms a decentralized domain name system that utilizes an NFT-based domain minting mechanism, which allows for trustless domain ownership and the secure transfer of domain ownership. Tags features a peer-to-peer domain marketplace, where domains can be auctioned on a peer-to-peer secondary market, along with a dTLD (decentralized top-level domain) registration system allowing for anyone to create and issue dTLDs (domain suffixes) of their own and earn royalties in the process, each time their created dTLD is used for a domain registration.

Tags allows domain owners to easily manage their DNS records on-chain, using Web2-based Resource Record Types, as well as Web3-based Resource Record Types. 

Tags will operate as a DAO, where "TAGS" tokens can be purchased on-chain and used to purchase domain names on-chain. The proceeds from TAGS tokens will be stored within the TAGS treasury and managed by TAGS community. The proceeds that derive from the spending of TAGS tokens during the registration of domain names, will be split between the dTLD creator (royalties) and the on-chain treasury.

##### **Bench**

Bench is a parachain that forms a layer-1 smart contract platform that's Ethereum-compatible and optimized for DeFi. Bench's decentralized finance network is the home of bUSD, a decentralized, multi-collateralized stablecoin backed by cross-chain assets. Bench's goal is for bUSD to have value relative to the US Dollar and for it to become the de facto stablecoin of BitWeb. Bench's network is application-specific, powering liquidity, economic activity and stablecoin utility. 

The BitUSD (bUSD) protocol enables a decentralized, multichain stable currency that will serve as the native stablecoin of the BitWeb ecosystem. bUSD is minted from a variety of reserve assets, allowing these holders to earn, trade, spend, and access other products and services, without price volatility, while retaining ownership of the underlying reserve assets.

bUSD is pegged to the US Dollar, can be trustlessly integrated by any blockchain that's integrated with BitWeb (parachain and bridge chains), as well as applications deployed on those networks. Anyone can mint bUSD using reserve assets that are compatible with the Bench network, where each bUSD is backed by a excess value of those reserve assets, which act as collateral. These reserve assets are cross-chain and include BitWeb-native assets like B1T, ORB, TAGS, SERVER and others, including Bench's native token BEX. Bench also accepts the native assets of wholly unrelated blockchains like Bitcoin (BTC) and Ethereum (ETH).

Bench's network operates as a DAO, where a Governance and Technical council are elected to act out the wishes of the community, via community-voted proposals. 

The future goals for bUSD are as follows:

- Yield & Liquidity for Reserve Assets

Release liquidity from reserve assets to earn yield, while maintaining ownership. B1T, ORB, TAGS, SERVER and IQ, along with BTC, and ETH are reserve assets. While users maintain ownership of assets like B1T, they can collateralize to borrow bUSD to hedge volatility, pay for goods and services or access services without price exposure. For example, a Bench user could provide liquidity to a stablecoin pool, use a stablecoin savings product or purchase a Torus-based container.

- BitWeb's Default Routing Assets

If bUSD becomes the default routing asset for the BitWeb network, it will provide a universal trading pair, routing to all assets in the ecosystem.

- Trustless transferability 

dApp developers can easily integrate bUSD into their applications, without using insecure strategies like wrapping or bridging.

Bench's BEX token distribution has not been planned and will require further legal review.

##### **Route**

Route is a parachain that realizes the true free nature of Bitcoin (BTC) and decentralized finance, by allowing Bitcoin to move from Bitcoin's network, to BitWeb's ecosystem and wholly unrelated blockchains that are compatible with BitWeb's messaging protocols, like Ethereum, Cosmos and others.

Route utilizes participants that run what are called "Vaults," so that BTC is secured, allowing for Route's rBTC to be minted and used cross-chain.

The routing of Bitcoin from the Bitcoin network to other networks is simple:

1. A user can lock their BTC in a network participant's vault, or their own vault. BTC is secure and backed by Vault-based collateral.
2. rBTC is minted at a 1:1 ratio to the locked BTC.
3. Minters can earn interest on their BTC by using rBTC as collateral for lending, yield farming or other DeFi methods on any blockchain network.
4. Redeem rBTC for actual BTC on Bitcoin's network any time you want or spend rBTC on other networks that are rBTC compatible. 

Route onboards the most valuable crypto asset into the BitWeb ecosystem, while also enabling top 10 assets like DOT, ETH and others to be onboarded in the future.

##### **Inspire**

Inspire is a generic assets parachain, allowing developers to deploy and transfer fungible and non-fungible assets (tokens). The native token of Inspire is B1T. 

A few facts about Inspire:
1. Deposit transfer fees are 1/10th the value seen at the relay chain level (i.e. the Initial Deposit Fee (IDF) for an Inspire account is 0.100 B1T, while the relay chain's IDF is 1 B1T).

***NOTE:*** BitWeb's relay chain utilizes an IDF to ensure that empty accounts are removed from the chain, so that the network's state isn't bloated with empty, useless accounts. Accounts are required to maintain a minimum balance, in order to be active on the network.

2. Assets held on Inspire can be classified as follows:
    - Assets without any backing.
    - Assets backed by an on-chain protocol's utility.
    - Assets with off-chain backing.

Inspire is commonly used for transferring non-native tokens and creating NFTs. It is the token highway between native and non-native chains. It is also frequently used for minting NFTs and for utilizing its lower IDF.

Inspire is the asset component of the network, allowing anything to be tokenized, while also allowing for assets to move between networks effortlessly.

---

### DAO Overview

As mentioned above, BitWeb's root relay chain forms a democracy where users of the network are able to push forward proposals regarding network updates, network improvements, network-based investments and other areas that the community believes will create growth and improvements for the network at-large. The Internet in its earliest days utilized Requests For Comment (RFCs) to push forward proposals for improving the Internet with various protocols and technologies. The submission and approval process for RFCs was intended to be decentralized but has been anything but. The BitWeb looks to bring the Internet's decentralized vision for RFCs to life, while also giving the network's members the ability to collectively invest in various DAOs and projects that look to integrate with BitWeb's ecosystem, like parachains, to ensure network and treasury growth over time. Below, is a quick explanation of how the DAO works at the network-level and for token holders.

#### DAO Purpose

The DAO is looking to achieve the following:

- The streamlining and decentralization of the Internet's RFC process, allowing community members, developers, engineers and scientists to submit improvement proposals to the network for vote, allowing for the organic improvement of the decentralized web.
- Allow for community members to submit proposals involving the marketing, branding and identity-related to the network itself, along with day-to-day business operations. The community should be able to vote on improvements in these areas, allow for sub-contractors who can provide these services to apply to perform the related services required by the proposal, a way to vote on sub-contractors if the proposal passes and a way to fund contractors upon the community's approval of provider(s), according to a payment schedule defined via the proposal.
- Allow for community members to submit proposals regarding network updates and vote on these upgrades. Due to BitWeb's fork-less upgrade system, BitWeb can be updated via proposal rather easily, without any network interruption. 
- Allow for community members to issue proposals on future investments into other DAOs or integrated projects. The community should be able to issue a proposal regarding investment, describing the project, how investments will be disbursed and to whom, and the mechanisms by which the network itself will be able to reap benefits from the investment in an autonomous fashion. 

#### The Number Of Token Holders

Ideally, BitWeb would start off with a small group of private funders who join the DAO through private investment. That number has not been determined yet and will require further legal review.

#### Token Holder Powers

- Token holders can utilize their token holdings to vote on any proposal on the network, vote on a Validator or vote for a Council member. Each holder can vote once per proposal, can vote for up to 16 validator candidates and can vote for 16 council members (even though there are only 13 seats). 
- Token holders have the ability to spend their assets any way they want, wherever they want.

#### When Network Will Be Fully Operational and Decentralized

After the private sale of B1T, the initial contributors to the DAO (purchasers of B1T) will become the network's initial validators and the initial Council will derive from this deployment via the organic voting process. From the day the network launches, proposals will be published for token holders to vote on, including the following:

- Core Software Development - token holders will vote on the hiring of a development lab to continue the development that was initially donated by Octal Labs. Octal Labs will be the leading candidate for the job.
- Network Marketing - token holders will vote on the hiring of a marketing firm to market the BitWeb ecosystem globally.
- Autonomous ICO - token holders will vote on whether or not the network itself should perform an autonomous ICO, through the minting of B1T with the end goal of bolstering the treasury.

#### Essential Network Functions and Operations

Token holders must vote on Validators and Council members for the network to function. In order for the network to grow and compete with other networks, token holders must create proposals, vote on proposals and fund proposals that successfully create growth for the network.

#### How Token Holders Make Decisions

Token holders make decisions by voting on proposals issued by other token holders.

---

### Application Overview

Before the launch of BitWeb, we will launch a decentralized application/DAO known as BitHost that is integrated with each of its components (parachains and bridges), along with other infrastructure components from other blockchains like Akash, Flux, FileCoin, Sia, Cosmos, Subspace, Polkadot, Polygon, Avalanche and others. While BitHost will exist prior to the BitWeb network's launch, it will be integrated with other infrastructure services, allowing for BitHost to perfect its platform while BitWeb's development team finalizing the Alpha-launch of its initial testnet. It will also become a key marketing tool for BitWeb's actual mainnet launch. Below is a brief description of BitHost.

#### BitHost

BitHost is a decentralized web services platform, bringing together the best of Web3/4 infrastructure services, including those powered via BitWeb's future ecosystem. BitHost streamlines all of these infrastructure tools into a single user-interface, allowing developers to deploy decentralized applications across many Web3/4 service providers effortlessly. BitHost could be compared to a decentralized version of AWS, facilitating the deployment of modern and decentralized web services and infrastructure.

##### **WebChip and BitBox**

BitHost works alongside a companion hardware device known as BitBox that utilizes a custom designed Single Board Computer known as the WebChip. Like BitWeb's multichain software, WebChip's printed circuit board is also designed and developed by Octal Labs. The initial BitBox X will be powered by WebChip's 1776a model, which features an octacore CPU, 16GB of RAM and a 512 GB NVMe SSD. BitBox is powered by BitOS, an operating system that is specifically designed the run multiple blockchain and off-chain daemons, so that BitBox users can earn money for providing resources to various networks, including BitWeb. BitBox resource providers simply plug their BitBox into Ethernet, download the BitHost application to their mobile device, register their device over Bluetooth and can begin activating their BitBox to provide resources on various networks. By default, BitBox will function across all of its integrated networks, including the networks mentioned above.

##### **BitHost DAO**

The goal of BitHost is to function as a DAO from the start, without any private funding. The day of BitHost's launch, the community will vote on the following proposals that will be issued by BitHost's initial token holders:

1. A development agency who can handle BitHost dApp development, including its DAO-based smart contract - the leading candidate will probably be Octal Labs since they developed the initial platform. NOTE: Octal Labs agreed to develop the initial platform in exchange for HOST tokens.
2. A development agency who can handle future designs for BitBox and WebChip - the leading candidate will probably be Octal Labs since they developed the initial BitBox X and WebChip's initial 1776a model for free, in exchange for HOST tokens.
3. An administrative company who can handle the domain name for BitHost, application submission to app stores and legal issues.
4. A marketing firm who can handle digital marketing and ad placement for BitHost
5. A manufacturing company who can handle the manufacturing of WebChip and BitBox, along with logistical tasks related to getting BitBox and WebChip to distribution companies. The leading candidate will be \[HARRY COMPANY HERE\], who has initially handled manufacturing and logistics through their own partners for the initial production of BitBox and WebChip.
6. A lawyer or law firm to handle legal issues on behalf of the administrative company mentioned in (3).
7. A distribution company to handle the distribution of BitBox to retailers.

##### **Future BitHost DAO Functions**

- Investing in infrastructure-based DAOs that are integrated with the BitHost platform
- Acquiring dying data centers and converting them into Web3-based infrastructure providers, bringing major profits to the DAO, along with a substantial amount of resources to BitHost's integrated Web3 networks.

##### **Purpose Of BitHost**

BitHost is an important element of BitWeb's eventual launch. BitHost integrates with a majority of the major blockchain platforms out there that provide key Web3/4-based infrastructure, while simplifying the usability of these networks via a unified experience. We are already seeing a great amount of interest from major blockchain platforms who provide these sort of infrastructure services, considering the development experience they offer is highly complex and unfriendly, to say the least. The addition of the BitBox hardware and our goal of onboarding resource providers to these networks, means that a majority of their network participants will want to join the BitHost DAO due to the value it brings to their home networks.

While BitHost builds up a large developer base, the fees developers pay to use the BitHost platform will go towards the BitHost treasury and will help fund BitHost projects, integrations, investments, marketing and more. Likewise, the day BitWeb's network is launched and subsequently integrated with BitHost, it will provide a better and more performant alternative for developers to integrate within their applications, considering it will encompass all of the collective areas BitHost's other integration partners cover. Even if developers don't choose to move their applications right away, a large amount of developers will be introduced to the BitWeb platform the moment it launches, allowing BitWeb to grow faster than other blockchains or multichains have in the past. BitHost launching a multichain to developers, could be compared to an exchange launching its own coin to its users. BitHost is BitWeb's secret tool for securing a large number of developers, over a small period of time. This brings true intrinsic value to the network and is clearly a great marketing strategy for the network at-large.
