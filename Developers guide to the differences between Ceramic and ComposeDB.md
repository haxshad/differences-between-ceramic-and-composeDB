## Ceramic (Composable Web3 data network): An Introduction

![Ceramic Overview](https://user-images.githubusercontent.com/100013084/202481575-5484ac77-d0be-4492-990f-66be71ebaa0e.jpg)

Ceramic is a **decentralised** data network that gives Web3 apps infinite data composability.
By allowing you to browse a marketplace of data models, plug them into your app, then save, update, and retrieve data from those models, Ceramic makes creating applications using composable Web3 data simple.

Data is inherently interoperable when the same data models are utilised by many applications. Ceramic enables data to be composable and reusable across all apps by decentralising application databases.

## Why do we need the Ceramic Protocol❔ 🤔

By using the ceramic protocol, we can achieve:

1. Identity that is **portable** and **self-sovereign**
2. Storage of user and application data that is **interoperable**
3. Without requiring any new logins or accounts, **open web services**
4. **Schemas**and **definitions** for shared data

_With these, Ceramic enables information interoperability across all platforms and services on the internet._

To better understand why we need ceramic, let's look at some ceramic `use cases`

- **Payment:** Ceramic enables online transactions without the usage of a third-party processor. This offers customers a more secure and effective way to conduct transactions by enabling them to make and receive money straight from their DIDs

- **KYC:** KYC for people and companies can be done using the Ceramic Protocol to confirm identity papers. For businesses that provide financial services and adhere to tight rules, this use case is particularly crucial.

- **Social media:** users may exchange data between platforms without making new accounts and log in to social media sites using their DIDs. Users can share only the data they want because they have complete control over their data sharing.

Whoa... You read this much? I appreciate you. You appear to be interested in learning more about ceramics, don't you? Let's look at an important framework, `Self.ID` SDK.

## Self. ID (A Builder's Bundle)

In layman's terms, `Self.ID` is a framework that makes it simple to create Web3 applications with user-centric, composable data storage and retrieval and Ethereum-based authentication.

`Self.ID` is a straightforward SDK that requires little configuration and gives users access to the entire Ceramic stack with support for well-liked environments like React and the web. `Self.ID` is simple to use and expandable. Ceramic doesn't require users to install new wallets or create new accounts because `Self.ID` works with Ethereum accounts and EVM-based wallet authentication.

Maybe I sparked your interest in learning more about yourself. If you want to get your hands dirty, I'm leaving the link to the official documentation. Go check it out.

☞ [Self.ID](https://developers.ceramic.network/reference/self-id/)

To complete the ceramic as a whole, we need ComposeDB. What does it mean? 🤔

## ComposeDB:

ComposeDB on Ceramic is a decentralized, composable graph database built on IPFS. A graph structure is made available by ComposeDB for interacting with data on the Ceramic network, that enables multi-player use cases, such as those required by social and DAO applications.

It offers many configurations (building blocks) that enable developers to construct applications on Ceramic quickly, including the capability to `find`, `create`, `exchange`, and `reuse` data models using `GraphQL`.

ComposeDB adds many features to the Ceramic network, which makes a difference between both. Let's see what it is. 👇

## Ceramic 🆚 ComposeDB

![differences between Ceramic and ComposeDB](https://user-images.githubusercontent.com/100013084/202481459-7859fb22-4c34-4e3f-a75e-d64173ba05f0.png)

**1. DataBase Type:**

**Ceramic:** This is very dissimilar to the key-value store that Ceramic currently works on.

**ComposeDB:** ComposeDB introduces a graph database type, which means that each node must now be supported by a **SQL database**, such as `SQLite` or `Postgres`, which will be used to **index** the data and build the database for the data models in your Composite.

**2. Indexing of data:**

**Ceramic:** Today's ceramic doesn't have any indexing method.

**ComposeDB:** ComposeDB, on the other hand, fills this indexing by each ceramic node.

**3.Storage streams:**

**Ceramic:** Ceramic uses TileDocument streams. The third document type offered by Ceramic, known as "tiles," is the most flexible and may be used to represent virtually any type of information.

But the prior data models module will be retired, and the use of TileDocument streams will be discouraged as we move toward Composites.

**ComposeDB:** CompositeDB uses model streams and MID streams.

Because, as we know, "the use of TileDocument streams will be discouraged as we move toward Composites.

**4.Query the data:**

**Ceramic:** In Ceramic we can query the data using many JS library method calls, but it is not convenient for many developers.

This is one of the reasons ComposeDB came into the picture.

**ComposeDB:** In order to get rid of this problem, developers need to use the GraphQL interface to Ceramic provided by the ComposeDB Client.

You can issue GraphQL queries and modify your Ceramic node once your ComposeDB Client has loaded it. ComposeDB will make developing directly with earlier developer packages on Ceramic more simpler and more efficient.

**5. Clients:**

**Ceramic:** Without clients, we cannot benefit from Cermaric or ComposeDB.
To deal with clients Ceramic uses `HTTP Client`, `ModelManager`, `DID DataStore`, `Self.ID SDK`.

**ComposeDB:** ComposeDB outperforms Ceramic in terms of client handling by utilising `HTTP Client` and `GraphQL Client`.

**6.Accessing the accounts:**

**Ceramic:**

Ceramic by default uses **3ID**. 3ID is basically, decentralized identities exist at the most basic level. A 3ID is the most popular method for creating **decentralised identities on Ceramic**.

Users can control and maintain their Ceramic accounts using several Web3 wallet accounts on various blockchains thanks to DIDs.

DID supports the 3ID approach, developed by Ceramic, which can simultaneously manage numerous keys and serves as an aggregator for many accounts.

**ComposeDB:**

ComposeDB by default uses **did:PKH**. The did:pkh DID method, which creates a persistent ID from the public key hash of a wallet address, is recommended by ComposeDB. For many Ethereum apps, this provides one-click sign-on with your wallet.

**7. Composability:**

**Ceramic:**

In Ceramic, developers must have had to manually contribute data models to the Github registry.

**ComposeDB:**

Data models are now automatically indexed in ComposeDB, making it simpler to find and reuse them. We'll closely follow with a UI, however in the initial release milestone, acquiring existing models is done through commands in the ComposeDB CLI.

**8. Authentication:**

**Ceramic:**

The Ceramic ecosystem requires users to write, sign, or decrypt data as part of authentication. The authentication procedure and the means for validating the addition of new data to a given stream are determined by the kind of stream.

**ComposeDB:**

DID is now supported by ComposeDB as one of its authentication methods. DIDs make it possible for documents to include public keys for encryption and signature verification.

**9. Developer Experience:**

ComposeDB mitigates the Ceramic's lagging sides very efficiently, and it makes the Ceramic more friendly to use than ever with it's rich advantages.

**10. User Experience:**

**Ceramic:**

Currently, Ceramic uses the sign-in popup method. Because of this, Ceramic didn't reach its full potential, and it dulls the user experience.

**ComposeDB:**

The "DID sessions" library will be used by ComposeDB to broaden the range of sign-in processes and data access patterns on Ceramic.
ComposeDB adds in this web3 wallet-native feature, which makes the user experience better than ever.

Reference: https://blog.ceramic.network/composedb-using-ceramic-as-a-graph-database/ 👇

![ceramic vs composeDB](https://user-images.githubusercontent.com/100013084/202481139-f68567e5-53f2-4de3-8891-54e73fb71591.png)

## Huh, now what's the summary?  🎉

Basically, **ComposeDB** is like add-on on **Ceramic network**. It adds various advantages to Ceramic to make it even better, which we saw in the differences between Ceramic and ComposeDB.

Just remember, using ComposeDB we can achieve our requirements more efficiently and easily. ComposeDB just increased the flow for a great `UX` and `DX` experience with great features.

With the combination of both, it will be great for `users`, `developers`, and the `whole ecosystem`.
