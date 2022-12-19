---
cp: 6
title: Add a block reward and improve Collator cycle
authors: Governance and Coordination Group (ImdioR, Orhan)
advisors: Cassidy, Miguel
proposal-type: CP-4
date-proposed: 2022-11-16
status: polling
---
## Short Summary
Implement a block reward to Centrifuge Parachain
Improvement of Collator Reward Cycle
## High-level objective
This proposal is aimed to improve Collators management and implement a block reward to the Centrifuge Parachain and funding the Centrifuge Treasury, which will solve a number of issues.
## Background
The standalone Centrifuge chain had a 3% block reward that was distributed to its validators and stakers.

Once Centrifuge became a parachain, the original staking pallet and block reward functionality could no longer be used. In this regard, the validators stopped securing the network, because Polkadot began to ensure the security of all parachains. It was expected that a new staking pallet would be developed and become available for parachains that had transitioned to using collators. However, such a pallet has yet to be developed to a state that Centrifuge can utilize it.

Though collators do not need the same incentives as validators did (given they do not require the same security guarantees or have as much at stake), there is still some desire to reward these collators for providing work to the chain. In addition, there is a desire to begin to fund the on-chain Centrifuge Treasury in order to fund community grants on-chain. The Treasury currently 1 has ~15.76 CFG because protocol fees have yet to be turned on.

The Burn rate is currently set to 0, but this parameter could be reevaluated in the future once the Treasury begins to accumulate CFG.

Each month, 1000 CFG is paid out of the Treasury to each collator in accordance with the previously passed [Council Motion](https://gov.centrifuge.io/t/centrifuge-council-collator-selection-criteria/3684). At the moment, the treasury is empty, so payment to collators from the treasury is impossible and must be done manually.

Therefore it is proposed to implement a block reward that will both fund the Treasury in the short-term (before the protocol becomes self-sustaining and can rely solely on protocol fees) as well as to provide some reward to collators (which will replace the manual reward process currently used to compensate collators).

## Detailed description of the proposal:

The Treasury has primary importance in the development and future of any project.

Any activity or project that benefits Centrifuge can be funded by the Treasury. This could include, but is not limited to: infrastructure deployment and continued operation, сross-chain application development, network security operations, collaborations with chains/projects, marketing activities (advertising, paid features, collaborations, video content), community events and outreach, software development, research, education, etc.

We believe that on the way to decentralized management and successful development of the project and interaction with other projects, it is crucial to have a well-funded Treasury that entities can apply for funds from.

Based on [this proposal](https://gov.centrifuge.io/t/centrifuge-council-collator-selection-criteria/3684), the current amount of CFG tokens to be paid out to each collator is 1000 CFG per month. Out of the minted block reward, everything will go to the treasury, except the amount that will be distributed to the collators.

It is technically difficult and inefficient to implement this reward per block, therefore it is proposed to use an epoch mechanism to distribute the block reward to the treasury and to collators. The epoch period suggested is 12 hours. The collator set changes every 12 hours (2 sessions), so matching the epoch end to the collator cycles will minimize the situation where a collator that is removed from the set in the first half (for example) will not get any reward at the end of the epoch.

If the reward period for collators is reduced to 2x daily, then that amount would be 1000CFG / 30 days / 2 = 16.65 CFG/epoch

At each epoch close 16.65 CFG * number_of_collators will be distributed to collators and the remainder of the block reward will be minted into the Treasury.

This block reward is important for the future of the Centrifuge protocol and the Community and we would like to keep the same rewards rate as before, 3%. This parameter could be reevaluated by the Community in the future if needed.

### Calculation:
```
Block rewards = Annual Inflation/Total blocks produced in 1 year = (14670570 CFG/year)/(2628000 blocks/year) ≈ 5.5824 CFG/block

Inflation - 3% (14.67M CFG)
Total Supply - 489.019M CFG
Block production ≈ 12 sec/block,3600 blocks/12 hours, 7200 blocks/day, 2628000 blocks/year.
Every epoch 20,096 CFG is minted into the on-chain Treasury.

Calculation of block rewards:
The amount will be minted every epoch (12 hours):

1 epoch =( Block Rewards x 3600 blocks/12 hours)=(5.5824 CFG/block x 3600 blocks/12 hours)= 20,096 CFG

In this regard, and in connection with the foregoing, I propose:
```
## Change or improvement:

* Activate block rewards and mint 20096 CFG each epoch into the on-chain Treasury.
* Set daily collator rewards in line with epoch - 16.65CFG/epoch
* Set epoch period for rewards - 12 hours 
  
## Responsible to implement: 

k-factory

## Alignment to the mission of Centrifuge DAO:

>We believe that the Treasury should be funded in order to unlock new partnerships and new development, and improvement of the protocol.
With a funded Treasury, any individual or group following CP Framework could offer to provide service to the protocol and be paid.

>In its turn, сontinuous improvement of the protocol and new partnerships unlocks economic opportunity by connecting people to borrow and lend money transparently and cost-effectively.

Link to the RFC on the Forum: https://gov.centrifuge.io/t/rfc-add-a-block-reward-and-improve-collators-cycle/4766
Link to the Opensquare Snapshot: https://voting.opensquare.io/space/centrifuge/proposal/QmYh1uJmu4VgEa6H5CSirZ9juJTdbTAB77LazAK4tB9Gpv
