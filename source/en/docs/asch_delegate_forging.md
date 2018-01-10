title:  Delegate and forging mechanism of Asch
---

Every account in Asch system can be registered as a  delegate (nedd to pay 100 XAS ).

A registered delegate can accept votes from any xas coin holders. When the received support rate is in top 101, this delegate can obtain the right to account(eg, the right of block production, which is equal to the miners in Bitcoin. ) and get xas coins as reward. The process of block production is called forging.

Forging does not need much computing power like Bitcoin mining. Even a ordinary computer can be used to verify the algorithm of accounting right, which combines the time slice verification, delegate random ranking, delegate signatures and pbft algorithm. For more details, refer to Asch consensus agreement. The delegates in top 101 can produce blocks in chronological order with a block interval of 10 seconds. When the delegate in turn can not produce blocks because of exceptions, the block will be postponed to next 10 seconds and produced by the next delegate.

Each 101 blocks are formed as a cycle, the forging order of the delegates will be random changed in each cycle.
When the last block is produced, the reward will be settled in this cycle and the ranking will be refreshed.
If the delegates can not produce blocks because of the downtime, network errors and other reasons, they can not get the rewards of this cycle, and the productivity will decrease. Productivity is an indicator of the stability of a delegate, and low productivity may lost the votes.

The delegates with normal block production share the rewards equally, including block rewards and transaction fees. The amount of the reward does not affected by the rank and the votes. The reward for every top 101 delegate is the same.

# 1 Block rewards

Block rewards will decrease over time, and the specific time will be decided on the height of block in the future.
The block rewards of Asch system start from the beginning of block 464500. The initial reward is 3.5 coins.
The reward will decrease every 3 million blocks and it lasts about 1 year.After 15464500 blocks, the reward will be fixed and the inflation rate every year is less than 1.5%.

The following are the various stages of the block reward

|reward|initial height|end height|
|-----|------|-------|
|3.5|464500|3464500|
|3|3464500|6464500|
|2.5|6464500|9464500|
|2|9464500|12464500|
|1|12464500|15464500|
|0.5|15464500|---|

# 2 transaction fee

In addition to the block rewards, the delegates can obtain the system transaction fees.
There are several kinds of transaction fees, including:


|type|fee|
|----|---|
|transaction|0.1|
|vote|0.1|
|the second password|5|
|delegate register|100|
|dapp register|100|
|dapp deposit|0.1|
|dapp withdraw|0.1|
|multiple signatures|(n+1)*0.5|
|small file storage (not yet online)|(size / 200 + 1) * 0.1|
