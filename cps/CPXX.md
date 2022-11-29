We, Governance and Coordination Group, would like to ask Centrifuge Community and CFG token holders for feedback regarding this proposal. Any feedback, comment, or suggestions from the Community are highly appreciated.

Author(s): Governance and Coordination Group (ImdioR, Orhan)
Advisor(s): Cassidy, Miguel
Technical/non-technical proposal: Technical
Date proposed: 2022-11-16

Short Summary
Implement a block reward to Centrifuge Parachain
Improvement of Collator Reward Cycle
High-level objective
This proposal is aimed to improve Collators management and implement a block reward to the Centrifuge Parachain and funding the Centrifuge Treasury, which will solve a number of issues.
Background
The standalone Centrifuge chain had a 3% block reward that was distributed to its validators and stakers.

Once Centrifuge became a parachain, the original staking pallet and block reward functionality could no longer be used. In this regard, the validators stopped securing the network, because Polkadot began to ensure the security of all parachains. It was expected that a new staking pallet would be developed and become available for parachains that had transitioned to using collators. However, such a pallet has yet to be developed to a state that Centrifuge can utilize it.

Though collators do not need the same incentives as validators did (given they do not require the same security guarantees or have as much at stake), there is still some desire to reward these collators for providing work to the chain. In addition, there is a desire to begin to fund the on-chain Centrifuge Treasury in order to fund community grants on-chain. The Treasury currently 1 has ~15.76 CFG because protocol fees have yet to be turned on.
