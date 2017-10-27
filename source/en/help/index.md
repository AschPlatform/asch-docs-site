title: Asch FAQ
---

# 1 The brief introduction of Asch

The original design purpose of Asch is to reduce the skill threshold for the developers.For example,it makes DAPP development and traditional web applications become rather similar  by adopting JavaScript as an application development language and supporting RDB (Relational Database) to store the transaction data,
These characteristics must be extremely attractive to developers and SMEs (Small and Medium-sized Enterprises). We believe the prosperousness of the ecosystem of the whole platform is highly dependent on the developers’ productivity. Asch is an open platform that is not limited to specific areas— such as finance, document storage, copyright proof—but also providing a series of underlying and abstract APIs. These APIs can be combined flexibly to implement different types of applications. In terms of consensus mechanism, Asch system inherits and enhances DPOS (Delegated Proof of Stake) algorithm to significantly reduce the probability of forking in blockchain and the risk of duplicate payments.
Most importantly, Asch’s sidechain-as-a-application (SaaA) mode alleviates the blockchain inflation issue, as well as makes dApp more adjustable and individualized. Asch is a prospective, low-cost, one-stop solution that will become the incubator of next generation decentralized application. The token of Asch is XAS, and the initial amount of XAS is 100 million. Please browse Asch official website for details.


# 2 How do we know Asch?

check [official website](https://www.asch.so/)
Read [Asch white paper](https://www.asch.so/asch-whitepaper.pdf)
Developers can view/check the source code of Asch from  [github](https://github.com/AschPlatform/asch) and discuss with each other through Asch official QQ groups

Asch official ecological community QQ group one：485979564
Asch official ecological community QQ group two：545183438
Asch developers QQ group：472708713
BIVIEWS: ASCH  Column
Micbolg: 北京阿希链科技有限公司
Official WeChat：
![wechat](./assets/wechat.png)

# 3 What is the Asch Wallet?

Old wallet address of Asch system were digitals, later it upgraded to letters. They are compatible except for certain exchanges. Thus, old users should use the new alphabetic adders when withdrawing XAS on exchanges if possible.

Online wallet: http://mainnet.asch.so/

How do we use wallet?

Beginners must see how to manipulate Asch account proficiently.
[Notes for wallet users](http://bbs.asch.so/topic/23/%E9%92%B1%E5%8C%85%E7%94%A8%E6%88%B7%E9%A1%BB%E7%9F%A5)

Local Wallet（Full-nodes Wallet）

If you want to install Local Wallet by yourself, please refer to the article  [Asch Node Installation Guide](https://github.com/AschPlatform/asch-docs/blob/master/asch_install.md).

Mobile Wallet

Mobile wallet only needs to enter a master password when logging on at the very first time. Once you login, you will be required to set a gesture password, which allows you to access the mobile wallet afterwards.

Wallet for Android
    ![android](./assets/android.png)
Wallet for IOS
    ![iphone](./assets/iphone.png)

# 4 What language is used to develop Asch?

Asch platform is developed in Node.js language. There are some underlying developed modules with C or C++ language. When encountering a bottleneck in performance, we could use C or C ++ to modularize it completely. Node.js is the necessary skill if you want to develop Asch platform. We will add more SDK (mainstream programming languages such as java, python, php, and Go.)

# 5 What frameworks does Asch use?

Asch itself is a framework that is convenient for users to develop blockchain dApps. Since it is developed in Node.js, certain existing modules, for instance, express, are used.

# 6 What features does Asch have?

1. Supporting side-chains (cross-chains). DApp data are stored in the side-chain, so the main chain data will not swell too fast.
2. The Advantages of Node.JS language.
3. Saving block data in relational database to reduce the difficulty of dApp development
4. The speed of block production is rapid. Producing one block per 10 seconds and confirming it fast.
5. There will be no forking issues.
6. Safe sandbox isolating mechanism

# 7 Why will Asch not fork?

Asch system uses consensus mechanism which is based on Delegated Proof of Stake(DPOS). However, on the bottom half of the algorithm, we use an optimized variant of PBFT algorithm. This algorithm can achieve the consistency of the loyal nodes by the message complexity of O(n ^ 2) and time complexity of O(1) at t<n/3 to prevent bifurcation. In the equation t represents the number of the Byzantine Failures nodes (any possible problems such as network latency, system crash, vicious attack), while n represents the number of all nodes.

# 8 Can Asch be mined?

Asch uses a non-Pow algorithm, so it can’t be mined. However, the benefits can be gained by running as delegators. Asch use AC1.0 consensus algorithm (an optimized dpos with pbft algorithm) to ensure the output of blocks through the delegate system.

Everyone can register to be a delegate; everyone can vote for any delegate, but only the top 101 delegates who get the most votes can forge blocks (accounting). Currently, a delegate can get 3.5 XAS as reward for forging one block, and each block takes 10 seconds to be forged.

# 9 How much is the initial circulation of Asch?

Asch’s initial circulation is 100 million.

# 10 How much is Asch delegates’ returns?

Gross profit per day: 24*60*60/10*3.5=30240 XAS

Each trustee’s gross profit per day: 30240/101=299.4 XAS

The block rewards will decrease over time.Please click [here](https://github.com/AschPlatform/asch-docs/blob/master/asch_delegate_forging.md) to see the details.

# 11 How do we issue our own assets by Asch?

[Click to see the publishing asset tutorial](http://bbs.asch.so/topic/115/asch%E5%8F%91%E8%A1%8C%E8%B5%84%E4%BA%A7%E4%BD%BF%E7%94%A8%E6%96%87%E6%A1%A3)

# 12 Which platform does Asch support?

Currently, Asch is fully supported by the Linux platform, while Windows can synchronize blocks but cannot produce blocks.
We are looking forward to being supported by more platforms in the future.

# 13 How does Asch differ from ETH and LISK?

Comparisons between Asch and ETH

|name|ASCH|ETH|
|-----|------|-------|
|Consensus Mechanism|DPOS and PBFT focuses more on decentration when comparing to Pow. Pow also has the problem of hushing power and centralization of mining. Compared to Pos, the right to keep accounts is transferred to the delegates. Nevertheless, the shareholders still have the decision-making power, which make the whole system more security and decentralization.|Pow+pos|
|Smart Contract Implementation|Side-chain. The data stores in the dApp.|Transaction scripts.  The data is all in the main chain, easily expanding.|
|Contract Language|Native JavaScript|Solidity is designed for developing smart contracts that run on the EVM. ETH lacks documents and has small audience and high threshold.|
|Expansibility|The application of side chain and side chain can be downloaded as users’ needs without causing the main chain expansion.|The surge of Dapp will pose risks to the whole blockchain.|
|Security|The side chain operates independently with no effects on the main chain.|The vulnerability of the dApp will affect the whole blockchain, for example, The DAO.|
|Confirmation Time of a Block|10s|15s|
|TPS|3000|20|

Comparisons between Asch and LISK

|Name|ASCH|LISK|
|-----|------|-------|
|Consensus Mechanism|DPOS+PBFT; the latter prevents forking and eliminate double payment by hijacking.|DPOS, which leads to forking and fixture blocks.|
|Sandbox|Real sandbox can limit side chain’s permissions.|ETH cannot restrict the side chain’s permission.|
|Non-critical Refinement & Optimization |1.Create and sign the transaction at the front and transfer the encrypted data to the back. 2.As long as the problem of front-end performance is solved, it will not cause dpos to system itself.3.As For data persistence, the savepoint and the rollback of database are widely adopted. It will not fix blocks and fork even in the poor network.|The user’s password is transmitted directly to the back-end, which Easy to record and access|
|TPS|3000|20|


# 14 Where to trade Asch?

Today
[chaoex]https://www.chaoex.com
[coolcoin]https://www.coolcoin.com
[coinegg]https://www.coinegg.com
[bit-z]https://www.bit-z.com
[asdbi]https://www.asdbi.com
[bcex]http://www.bcex.ca
[kucoin]http://www.kucoin.com

In the future
[BTC100](https://www.btc100.cn/)


# 15 What blockchain browsers does Asch have?
Chinese version：http://aschd.org/
English version：http://explorer.asch.pub/

# 16 What Api does Asch provide?
The form of Api for Asch is RESTful,Click the link below if you request  http://45.32.248.33:4096/api/transactions/get?id=08ce16c9cf6a0dd4636f8f17665146984293c2f2889124877ad7e4f3eea37eb2，Then return to the json data.。
There are three categories of Api : :
1. General external access Api
2. Internal communication Api
3、Dapp api

# 17 What is the Asch inflation rate?
The block bonus will decrease as time goes by; the specific time is based on the height of a block in the future. The block bonus system starts form 464,500, with an initial reward of 3.5 coins, and is reduced every 3 million blocks, approximately a year. After the 15,464,500 blocks, bonuses are no longer diminishing, with a slight inflation rate of less than 1.5% a year (relative to the initial amount of 100 million).
The inflation rate is as follow： (calculated from the 464,500 block, at the point of block rewards generation, around October 7, 2016)

|Years|Inflation rate relieve to last year|Current block bonus sum (In units of 10,000 XAS)|
|-----|------|-------|
|First year|10.5%|1050|
|Second year|7.5%|900|
|Third year|5.9%|750|
|Fourth year|4.5%|600|
|Fifth year|2.2%|300|
|Sixth year|1.1%|150|


Bellows are the blocks of rewards at all stages:

| Delegates Award (XAS)| Initial height | Final height  |
| ------ | ------ | ------ |
| 3.5 | 464500 | 3464500 |
| 3 | 3464500 | 6464500 |
| 2.5 | 6464500 | 9464500 |
| 2 | 9464500 | 12464500 |
| 1 | 12464500 | 15464500 |
| 0.5 | 15464500 | --|

# 18 What is the GPL of Asch code?

The MIT License (MIT)

# 19 What related algorithms does Asch use?

Consensus algorithm 0.5（AC0.5）
Consensus algorithm 1.0（AC1.0）
Password generation algorithm: BIP39 specification (Level 1 password)
Private key and public key generation algorithm: ed25519 encryption

# 20 Side-chain (cross-chain) Introduction

The side chain does not refer to the side chain that Asch made for other blockchain, but to the Asch’s own side chain, i.e. Dapp.

Currently, node.js is the only development programming language. If you want to use Java, python, PHP and other language, all you need is to make the corresponding SDK. Everyone should give it a try. The main purpose is to write the library of Asch-js in other languages.

Qingfeng has been optimizing the convenience of Dapp development. More details will be revealed when releasing the Asch2.0.

The existing documents are as follows:
The introduction of Asch Dapp: notes on side chain related technologies
Dapp development tutorial 1: Asch Dapp Hello World - this document will teach you how to create and publish a basic side chain applications, and introduce the source code structure of the side chain framework.
Dapp development tutorial 2: Asch, Dapp, Asset
Dapp development tutorial 3: Asch Dapp Mini DAO - this document teaches you how to create new transaction types or smart contracts, and provides a Mini Dao project that includes project management and voting functions as demonstrations
Dapp development tutorial 4: Asch Dapp Dice Game development tutorial- this
document teach you how to create more complex types of transactions or smart contracts, how to establish the connections between contracts, how to rely on historical transaction data when enforcing contracts, and the realization of a dice game as a demo.
Dapp development tutorial 5: Release Dapp Online - this document teaches you how to register on the online system (testnet, mainnet), and how to install and uninstall.

# 21 How do we transfer Asch?

Click : http://forum.asch.so/index.php?s=/forum/index/detail/id/95.html

# 22 Asch’s work focuses
There are two main directions: application development and bottom development:
1.Application development: Mainly for several typical applications, for example, for news aggregating, forecasting markets and exchanges.
2.Bottom development: Optimize TPS, smart contracts, anonymous transactions, Identification (ID) authentication, the Oracle, and the cross chains with BTC and ETH.
3.The community has already developed some supporting facilities, such as asset browser, USB wallet and Java SDK.

# 23 Asch’s history

01/01/2016 Asch program was initiated.
03/01/2016 The implementation of a predigest algorithm model based on PBFT (prototype of Asch consensus algorithms) to fixe bugs of DPOS algorithm after the bug was analyzed and a simple attacking way was simulated. https://github.com/sqfasd/dpos-pbft/
06/28/2016 4 am The first block of Asch was born.
06/2016 The implementation of a full version of dpos+pbft algorithm in formal products, and deployed 10 machines to test it. The tests results meet the expectations in security. The whole system will not fork (AC0.5) even under the
circumstances such as rebooting frequently, broadcasting blocks irregularly, cheating by a small number of delegates.
07/13/2016 Asch version 0.9.1 released. The open beta began and majority delegates started to participate in the beta test.
07/17/2016 Asch version 0.9.2 released.
08/02/2016 Asch version 0.9.3 released.
08/09/2016 Asch version 0.9.4 released, while the product tends to be stable.
08/09/2016 The system was upgraded to version 0.9.5 and optimized. In the testnet that combined by 49 nodes, the peak bandwidth was around 600kbps.
08/11/2016 Consensus Algorithm was upgraded to AC1.0.
08/16/2016 Asch Mainnet was launched officially.
09/01/2016 The source code of Asch product officially was published. The source code document: https://github.com/sqfasd/.
09/08/2016 Asch version 1.0.1 released. The Light Purse went live officially. In addition, unconfirmed transactions were fixed.
09/15/2016 Asch version 1.1.0 released.
Fixed bugs of multiple dapps running at the same time.
Added page display of the front-end dapp.
Added display of the block production status.
Added commands to start block production in Asch script.
Updated dapp types.
Fixed the crashing bugs for getdelegates in certain conditions.
Fixed bugs in dapp installation and uninstallation.
Added querying interface for top account.
Fixed reindex bugs during restarting which happened in great chance.
09/30/2016 Asch version 1.1.1 released.
Fixed the synchronized bugs in LAN environment.
Increased detections of version compatibility, and refused to accept incompatible connection of node for old version.
09/2016 The token of Asch Project, XAS, was listed on Jubi (www.jubi.com).
10/21/2016 Asch version 1.1.2 released
Supported i18n.
Dealt with synchronized main card issue caused by transaction rollback.
Fixed the cleaning issue of dapp database.
10/26/2016 Asch version 1.1.3 released.
Fixed trade ductility issues.
10/26/2016 Asch version 1.1.4 released.
Fixed the memory overflow problem caused by request@2.76.0
Used a specific version of the node module as Asch dependencies
10/2016 XAS was listed on BTCBOX.COM (the Japan International Exchange), quitted later
10/2016 Cooperated with Beijing Financial Cloud Laboratory, and conducted evidences storage business (customized version of Asch)
11/10/2016 Asch version 1.1.5 released.
Fixed the fixture block problem caused by backwards tick.
11/22/2016 Invited to technical trainings of corporate blockchain by Japanese Mengzhen Holdings.
11/25/2016 Shousong Zhang gave a speech about “Block Chain Application based on side chain technology” in WOT2016 Big Data Technology Summit.
12/20/2016 Green Paper of Asch-eco community was published. Within one week, the presidents and vice presidents of the Volunteers Association, the Delegates Association, the Developer Association were selected.
12/2016 Cooperated with Japanese Telecommunications Company and released digital asset.
01/18/2017 Asch version 1.2.1 released.
02/17/2017 Asch version 1.2.2 released.
02/26/2017 Asch version 1.2.3 released.
Added the simple storage function (customized by Zhongjinyun)
Added function of issuing asset for users (UIA)
02/26/2017 Asch version 1.2.4 released.
Activated address of base58check format after block 1,700,000.
03/01/2017 Asch version 1.2.6 released.
03/01/2017 Asch Mainnet Version 1.2 was activated officially.
Added storage interface.
Added issuing asset interface for users.
Adjusted (optimized) web graphic interface.
Changed the format of transaction number and block number to 32 hex bytes without the affection of the old data.
Coexisted the old and new data.
Changed the account address to base58check code, and coexisted the old and new account.
03/05/2017 Asch version 1.2.7 released.
Fixed the issues submitted by front-end transactions. Fixed the display issues of pop-up dialog box. The Light Purse allowed users to select the node themselves.
04/07/2017 Shoushan Zhang gave a keynote speech on “Asch 2.0 - Maintaining the status quo” in the Second China Financial Trading Technology Conference.
05/08/2017 Asch was first entered coinmarketcap.com, and was ranked top 100 in the Global Encryption Coin.
05/14/2017 Asch participated in the First China Block Chain Developing Competition.
06/05/2017 Asch Mobile Wallet for Android and Asch Mobile Wallet M version was officially released.
06/19/2017 Asch was ranked top 50 in the Global Encryption Coin.
06/20/2017 XAS was listed on two exchange platforms - coinvc.com and biduobao.com.
07/06/2017 Asch was traded in YUANBAO Exchange（yuanbao.com/trade/xas2ybc）
07/18/2017 Asch version 1.3.0 released.
07/25/2017 Qingfeng Shan, the founder of Asch, was invited to the Seminar on the Construction of Blockchain  industry ecological system in Guiyang, China
08/03/2017 Asch has joined Blockchain technical application association in Zhengjiang, becoming a full member of the association.
08/06/2017 Qingfeng Shan delivered a speech on “Side Chain Technology and the Version of Block Chain 2.5” during China Blockchain Geek Summit
08/07/2017 Asch community has issued the first DAPP demonstration application - CCTime and its white paper
08/10/2017 Asch officials have brought the donations to earthquake-stricken area of Sichuan

