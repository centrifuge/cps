---
cp: 2
title: Centrifuge Proposal Framework
authors: Governance and Coordination Group (ImdioR, Orhan)
date-proposed: 2022-10-18
date-passed: 2022-11-12
date-modified: 2024-05-13
status: passed
---

# CP2 (Request for Funding)

Any entity (group or individual) who seeks funding from the Treasury, would need to create a proposal, using the CP2 component. There can be different scenarios for an entity applying for funding:

- The entity already created a proposal using both the CP1 and CP2 component (that passed), 
received funding and wants to re-apply
- The entity already created a proposal using the CP1 component (that passed) and wants to apply for funding
- The entity doesn’t have a mandate but wants to apply for funding for a one time service

The Treasury is administered by the Council so only the Council will vote on the proposal - token holders will not vote on it. 

It is possible to make a Treasury proposal on behalf of someone else.

A Treasury proposal can only be made if there are adequate funds in it to cover the funding request.

When creating a request for funding, make sure to provide the calculations for the requested amount and how they will be distributed. You can see an example of how it can be done in [this post](https://gov.centrifuge.io/t/rfc-establishing-a-centrifuge-credit-group/3554).

## GOVERNANCE PROCESS

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|2|Create an RFC on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) (see template below for title, tags and content)|Minimum 7 days|
|3|Create an on-chain [Treasury proposal](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Ffullnode.parachain.centrifuge.io#/treasury)|-|

## TEMPLATE
```
Title: CPXXX: [TITLE OF PROPOSAL]

Tags: cp2, rfc
```
### Body of the RFC must contain:
```
cp: [XXX]
title:
authors: [forum handles]
contributors: [forum handles]
beneficiary: [name]
wallet: [wallet address]
uses-component: [cp1|cp2|cp3|cp4|cp5|cp32|cp63]
technical-proposal: [yes|no]
requires-onchain: [yes|no]
impacts/modifies:
status: [rfc|voting|passed|rejected]
date-proposed: [YYYY-MM-DD]
date-ended: [YYYY-MM-DD]

Short Summary 
- One sentence summary of the funding sought

High level objective 
- A short description of the objective that this proposal will achieve

Background 
- What are the historical and contextual factors that make this proposal relevant and aligned with the mission?

Description of Activity 
- Give details on the activity and the problem it is solving

Change or improvement 
- What is the change or improvement that this mandate will bring?

Alignment to the mission of Centrifuge DAO
- Explain why this is important and aligned with the mission

Description of Individual/Group seeking funding
- Background of the member(s) of the group seeking funding

Budget
- What amount is requested and how is it calculated?
- How are the funds distributed within the group?

Delivery and Reporting
- A timeline of when the objective(s) will be delivered and how this will be reported
```
**Important:** remember to update the Forum post (tags, link to vote and outcome of the proposal) as the proposal progresses through the stages.