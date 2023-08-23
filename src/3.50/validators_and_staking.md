<h1> Validators and Staking </h1>

<h2> Table of Contents </h2>

- [Staking Propositions](#staking-propositions)
  - [Staking Proposition: Validator Staking Only](#staking-proposition-validator-staking-only)
    - [Validator Part](#validator-part)
    - [Node Staking and TFT as Collateral](#node-staking-and-tft-as-collateral)
  - [Staking Proposition: From the Ground Up](#staking-proposition-from-the-ground-up)
  - [Staking Proposition: Farm and Validator Altogether](#staking-proposition-farm-and-validator-altogether)

***

## Introduction

We want to roll out and improve our validator and staking strategy.
***
## Basics of Staking

Staking can happen on

* ThreeFold Guardian Validators
* ThreeFold Farms

Staking is important for the following reasons:

* You show your support for a farmer or a guardian, because you give them your vote of confidence.
* You show your support for the TFGrid by locking in value and receiving rewards for doing so.
***
## Staking Principles

* 9 to 33 validators are operated by ThreeFold Guardians. We call them Guardian Validators.
  * As block creators are elected based on staking, it is not possible to enforce a lower bound. These numbers (9 to 33) would need to be discussed and approved.
* Every TFT token holder can stake their tokens on Guardian Validator(s) or on the Farm(s) of their choice.
* The minimum number of TFT per validator is 2,000,000 TFT.
* The Guardians and Farmers get votes on the TFChain DAO in relation to the weight of the amount of staked tokens on their Validator or Farm.
* A form of punishment (e.g. slashing) should be implemented in the cases where the authority misbehaves. The incites validators to be constantly effective and will allow stakers to support trusted parties (e.g. validators with few or no failures)
  * Potential slashing events:
    * Failure to participate promptly in minting.
    * Normal PoS slashing events.

***

## Staking Rewards

The initial rewards for the staking tokens on a Guardian Validator are

* 10% of TFT that is used for utilization of the grid.
* A commission of 20% on above 10% goes to the Validator Operator = The Guardian.

The initial rewards for the staking tokens on a ThreeFold Farm are the following:

* 10% of TFT is used for utilization of the grid.
* A commission of 20% of the 10% (i.e. 2%) goes to the 3Nodes Operator, i.e. the Farmer.
This is only for the tokens that are staked, the farmer gets other rewards in relation to utilization.

***

## Previous Validator Registrations

* L0 and L2 validators will be able to delegate their TFTs to the new staking model
  * 2 millions tft for L2
  * 100 000 tft for L0
* delegated staking will be done at a later stage

Thus, we need to find the best staking program that would best suit the grid.

***
# Staking Propositions

## Staking Proposition: Validator Staking Only

### Validator Part

We propose a simplified staking model for the TFGrid 3.50. 

In this proposition, there would only be one kind of staking on the TFGrid: validator staking. In essence, node staking and farm staking would simply be delegated staking to the validator staking model. The 10% of staking revenue to validators and the 10% of staking revenue to farmers would thus be combined in one 20% and distriuted on the pro rata of the staking quantity.

We also propose that each 3Node on the grid would require a given amount of TFT collateral. This TFT collateral would be used as deletaged staking. In this scenario, farmers would have their collateral/staking TFTs delegated to validators. 

Furthermore, the weigth of a given DAO vote would be based on the current shares in validator staking. Since every farmer would have TFT collateral directed as delegated validator staking, every farmer would have a weight on DAO voting.

Since validators get revenues from utilization on the TFGrid, this overall staking model would give a great emphasis and importance on utilization. It would incite members of the whole ecosystem to increase grid utilization.

### Node Staking and TFT as Collateral

When it comes to node staking, we propose the following model with two node staking options: having TFT as collateral and liquid farming rewards, or having locked TFT (non-liquid) until you achive the collateral amount. 

Each 3Node requires a minimum amount of collateral based on their 3Node resources. 

If the farmer stakes the minimum TFT collateral amount for their 3Node, the TFT farming rewards are liquid and thus the amount of TFT they farm at everyone minting period is directly available to them.

If the farmer doesn't stake the minimum TFT collateral amount for their 3Node, the TFT farming rewards are non-liquid and thus the amount of TFT they farm at every minting period is locked until they stake the minimum collateral amount.

* Farming model with 2 options
  * (1) A farmer stakes the minimum TFT for their given 3Node as collateral
    * Monthly farming rewards become liquid (unlocked)
  * (2) A farmer doesn't stake the minimum TFT for their given 3Node as collateral
    * Monthly farming rewards are non-liquid (unlocked) and added to the validator staking pool
      * When the total staked TFT reaches the minimum TFT for their given 3Node as collateral
        * the additional TFT becomes liquid
        * In short, it goes back to option (1).

As a concrete example, say a farmer has a 3Node with XYZ resources and this 3Node requires 10 000 TFT of collateral. The farmer can decide to stake 10 000 TFT as delegated staking to a validator. This 10 000 TFT acts as a collateral for their 3Node. This way, after each minting period, the farmer receives unlocked TFT rewards.

If the farmer doesn't have any TFT or simply doesn't want to stake the 10 000 TFT as collateral, the TFT farming rewards they receive at each minting period would directly go to a delegated staking of a validator. The 3Node would then farm TFT at every minting period and when the 10 000 TFT are staked, any TFT minted after this point would be liquid and unlocked to the farmer.

## Staking Proposition: From the Ground Up

We propose to have a maximum TFT quantity to be used as staking.

For now, we have 

* 50 validators at 100 000 TFT
* 50 validators at 2 millions TFT
* This gives a total of 105 millions TFT staked

If we set a limit to 125 millions TFT staked, we would need 20 millions TFT staked from farming and nodes.

We set that for each ratio of 8GB of RAM/1vcore/512 GB of SSD, you need X TFT staked.

This TFT staked goes to the validator staking pools. Farmers thus do delegated staking to validators and get in return part of the rewards and voting weight.

For simplicity for now, say we have 2000 nodes and we have 20 millions TFT to stake with farming and nodes. Thus it means each 3Node would need to stake 1000 TFT. This would be their collateral. If a farmer doesn't want to put collateral, the TFT farmed is locked until it achieves the minimum collateral amount.

## Staking Proposition: Farm and Validator Altogether

We could also 

* what is the purpose of farm staking?
  * propositions
    * unlock additional revenue to the farmer
      * if you don't stake
        * this part goes to
          * burning
    * can vote