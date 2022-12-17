# CP-4 (GI): General Improvements

This CP is used for proposals that don’t fit under any of the types. In other words, if it is not a CP-1, CP-2, CP-3 or CP-5 (or any of their derivatives), it is a CP-4. 

A CP-4 can therefore be a wide range of proposal types, to improve the protocol or expand the ecosystem, and that require input from the Community. A CP-4 can roughly be divided into two categories; technical and non-technical.

### Technical CP-4

These can be proposals for the roadmap and technical features and functionality of the Centrifuge protocol, such as adjustment of fees, burning of tokens, liquidity pairing with another protocol, opening HRMP channels between other parachains etc. If passed, these proposals will typically be part of a Runtime Upgrade (CP-3) afterwards, but not always.

### Non-technical CP-4
These are proposals that do not require a change on the blockchain, and hence do not require an on-chain vote. This could be co-marketing partnerships, changes to the Governance process, incentivising users with NFTs for participation in Governance, creating events etc.

### GOVERNANCE PROCESS

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create an RFC on the [Forum](https://gov.centrifuge.io/c/cfg-governance/request-for-comments/37) (see template below for title, tags and content)|Minimum 7 days|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|3|Create a Proposal post on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18)|-|
|4|Create a snapshot vote on [OpenSquare](https://voting.opensquare.io/space/centrifuge)|Exactly 7 days|

For **non-technical proposals**, the process ends here and if the snapshot vote passes (majority of CFG votes in favor of the proposal), the proposal passes. 

For **technical proposals**, if it is a standalone proposal - i.e. not part of a Runtime Upgrade (CP-3) - there will be two more steps. 

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|4|Create a [Council motion](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Ffullnode.parachain.centrifuge.io#/council) or [public proposal](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Ffullnode.parachain.centrifuge.io#/democracy) |-|
|5|Public referendum |Exactly 7 days|

Otherwise, the proposal will be in queue to be implemented in an upcoming Runtime Upgrade.

### TEMPLATE
```
Title: [TITLE OF PROPOSAL]
Tags: cp-4, month, year
```
#### Body of the RFC must contain:
```
Proposal type: CP-4
Author(s): Forum handle(s) of author(s)
Member(s): Forum handle(s) of member(s)
Date proposed: yyyy-mm-dd
Short Summary 
- One sentence summary of proposal
High level objective 
- A short description of the objective that this proposal will achieve
Background 
- What are the historical and contextual factors that make this proposal relevant and aligned with the mission?
Description of Activity 
- Gives details on proposal, describe the new process or feature and the problem it is solving
- Relevant data/calculations - provide all the necessary information (links to relevant pages, charts, calculations etc.) and make sure there is enough for the Community to make a qualified decision, based on it
- Technical specifications, i.e. link(s) Github l (if relevant)
Change or improvement 
- What is the change or improvement that this proposal will bring?
Responsible
- Who is responsible for the implementation
Alignment to the mission of Centrifuge DAO 
- Explain why this is important and aligned with the mission
```
