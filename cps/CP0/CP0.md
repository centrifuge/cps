---
cp: 0
title: CP-0: Centrifuge Proposal Framework
authors: Governance and Coordination Group (ImdioR, Orhan)
date proposed: 2022-10-18
status: passed
---
## Short Summary
Proposal for a new Governance process and defining proposal types and their templates.

## High-level objective
This proposal aims to bring more clarity and transparency to our Governance process. The Governance & Coordination Group (GCG) want to provide a clear framework and process for proposers, by defining different proposal types and their Governance processes.

The different proposal types are called CPs (Centrifuge Proposals) and they are each followed by a number, indicating their type.

## Background
In our proposal to become a core group in the Centrifuge DAO, and get a mandate to formalise, coordinate and facilitate Governance processes, we promised that one of our first tasks would be to propose a clearer Governance process.

## Description of activity

### Centrifuge Proposal Principles and Guidelines

- All proposals must be aligned to the Centrifuge Mission to unlock economic opportunity by connecting people to borrow and lend money transparently and cost-effectively
- All proposals must follow their respective Governance process
- A CP must be as clear and easy to understand as possible. Any member of the community without special knowledge should be able to understand the meaning and purpose of the proposal, even if not all details
- A CP must be thorough. Relevant information or categories must not be left undefined
- The proposer must select the relevant type CP (e.g. CP-1, CP-2 etc.) and provide the information mandated by their templates
- CPs must use the baseline timing of their Governance process but can use extensions if needed. If you want to use an extension make it clear in the RFC itself and outline why you think an extension is needed
- Using the principles, process, and CP framework, anyone can create a CP at any time

**Request For Comments (RFC)**

Creating an RFC is always the first step of a proposal and the off-chain governance. This is posted on the Forum and the purpose is to give the Community the opportunity to provide feedback and ask questions and gauge support for the proposal. If changes are made to the proposal, based on the feedback from the Community, they should be done in this step.

Some proposals may require longer time for discussion than others, but the minimum time an RFC should be running is 7 days. The proposer decides how long an RFC should run before moving on to a snapshot vote.

In the templates for each proposal type, there is a description of what the RFC should contain (e.g. title, content etc.) in the Forum post. All RFCs must be posted in the Centrifuge [Request for Comments section](https://gov.centrifuge.io/c/cfg-governance/request-for-comments/37) of the Forum.

**The Centrifuge Proposals Repository (PR)**

All proposals must be submitted to the Proposals Repository (PR) on Github which is used to log all proposals. The discussion (RFC) takes place on the Forum, and if there are any changes made to the proposal, it must happen via the PR during the RFC phase, i.e. before the proposal proceeds to a snapshot vote. 
This is to ensure that a proposal is not changed during a snapshot vote or after it has ended.
A proposal is only deemed valid, if it has been submitted to the PR.
After a proposal has been submitted, a pull request number (XXXX) will automatically be assigned - this number will be used to index the proposal and in the title of the Proposal post.

**Snapshot voting**

Snapshot voting has replaced our Forum polls and is always the next step in the off-chain governance after an RFC (except for CP-2, CP-3 and CP-3.1, that do not require it). Once there has been adequate discussion of a proposal (after a minimum of 7 days) - and the proposal has been submitted to the PR - a snapshot vote must be created on [OpenSquare](https://voting.opensquare.io/space/centrifuge).

If a proposal does not require an on-chain vote, the snapshot vote will be binding (i.e. if the snapshot vote passes, the proposal passes).

Otherwise, a snapshot vote acts as an indicator for whether there is support for a proposal to proceed to an on-chain proposal.
The minimum voting time for snapshots on OpenSquare is 7 days - but the proposer could increase this to any amount of days, if they deem it necessary. This information must be communicated to the Community in the Proposal post on the Forum.
Once a proposal has moved on to a snapshot vote, a new Forum post (the Proposal post) should be created (see below). 
The outcome of the snapshot vote should also be announced in this same post.

**Proposal post**

Once a proposal has moved on from the RFC (and changes made if necessary), submitted to the PR, and the snapshot vote has been created, a Proposal post must be created. The purpose of this post is to notify the community that the proposal is now final and ready to proceed.

The title of this post will be CPXXXX (YY): same title as RFC, where XXXX is the pull request number from Github and YY is the abbreviation for the proposal type, e.g. (MRF).

This post should be created in the [Proposals section](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) of the Forum.

**On-chain proposal**

If a snapshot vote passes, the next step is to create an on-chain proposal if it is required (see each proposal type for whether they require it or not).

This can be done either as a Democracy Proposal (any token holder can create this) or a Council Motion (only the council can create this).

Once an on-chain proposal has been submitted (Democracy or Council), a new Forum post must be created in the [Proposals section](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) of the Forum.

The title of this Forum post should be **Council Motion XX: [same title as the RFC]** or **Democracy Proposal XX: [same title as the RFC]**, depending on how the on-chain proposal was created and where XX is the number of the on-chain proposal.

The body of the post should contain the following info:

- A brief description of the proposal with a link to both the RFC and the Proposal post
- Link to the outcome of the snapshot vote
- The Governance process going forward
- Link to Council Motion/Democracy Proposal (on Subsquare)
- Pre-image hash

If the Council Motion/Democracy Proposal passes, link to the referendum (on Subsquare) afterwards as a reply to the post, so everyone can follow the progress of the proposal. You can see an example [here](https://gov.centrifuge.io/t/council-motion-47-accept-statemint-hrmp-channel-request/4738).

**Cooling-off period**

A cooling-off period is the time that must pass before a proposal can be re-submitted. 
If a proposal fails to pass a snapshot vote, the cooling-off period is 15 days (counting from when the snapshot vote was created) before a new RFC can be resubmitted.

The cooling-off period is important in order to take the feedback from the Community into account and make the necessary changes to the submitted proposal, and re-submit the RFC.


### **Proposal types**
We have defined the following proposal types (CPs) and assigned them each with a number.

|CP #|Proposal type|Short description|
| --- | --- | --- |
|CP-1|Request for Mandate with Funding|Seeking mandate as a group/individual within the Centrifuge DAO to enact a project/work stream|
|CP-1.1|Request for Mandate without Funding|Same as CP-1, just without initial funding|
|CP-1.2|Removal of Mandate|Removal of a group’s mandate to enact a project/work stream (CP-1)|
|CP-2|Request for Funding|Asking for funding from the Treasury|
|CP-3|Runtime Upgrades|Proposals for Runtime Upgrades|
|CP-3.1|Emergency Proposals|Emergency proposals in case of hacks, exploits, attacks, or network halt|
|CP-4|General Improvements|Any proposal type, that does not fit under any of the other CPs|
|CP-5|Centrifuge Pool Onboarding Proposal (POP)|Onboarding new pools on Centrifuge Chain|

In general, the Governance process can be divided into two parts; *off-chain* and *on-chain Governance*.

*Off-chain Governance:*
This refers to the part of the process that takes place on our Forum (Request For Comments) and OpenSquare (snapshot voting). The purpose of this is generally to get input from the Community on a proposal and gather support, before moving the proposal on-chain (if necessary - not all proposals need to be submitted on-chain in order to pass).

*On-chain Governance:*
This refers to the part of the process that takes places on the blockchain. First a proposal is created on-chain (can be done by either the public or the Council) and this is generally followed by an on-chain referendum where all token holders can vote Aye or Nay.

Some of these proposal types have different governance processes (see individual description of their processes below), but what they all  have in common is that they start with a post on the Forum and all CPs must be submitted to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) on Github.

It is very important that the CP is submitted correctly. In the event of an incorrect format of a proposal, the process will need to be repeated.

Please contact the Governance & Coordination Group on the Forum or Discord ([Rhano](https://gov.centrifuge.io/u/Rhano) or [ImdioR](https://gov.centrifuge.io/u/imdior)), if you have any doubts or questions, and they will assist you.

#### CP-1 (MRF) Mandate Request with Funding

A mandate can be interpreted as an entity (group or individual) being given the authority by the DAO to pursue the stated objectives. The entity takes on the responsibility of fulfilling the mandate and accepts accountability to the DAO over this. 

Work can be initiated and brought to the DAO without a mandate, but no individual or group may claim to be working on behalf of the DAO without a mandate. 

A mandate indicates long term commitment (i.e. not a one time service, like creating a video for a specific purpose) and hence on-going funding.The maximum funding period is 6 months. This means that every 6 months, the group or individual would need to re-apply for funding by submitting a CP-2.

**GOVERNANCE PROCESS:**

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create an RFC on the Forum (see template for title, content, where to post etc.)|Minimum 7 days|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|3|Create a snapshot vote on OpenSquare|Minimum 7 days|
|4|Create a Proposal post|-|

If the snapshot vote passes (majority of CFG votes in favor of giving the mandate), the proposal has passed and the mandate has been obtained. 

The next step is the funding process, which will be an on-chain Treasury Proposal, voted on by the Council.
|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|5|Create an on-chain Treasury proposal|-|

#### CP-1.1 (MR) Mandate Request without Funding

Same as CP-1, just without funding (i.e. no step 5).

A group can make a proposal for seeking a mandate for a specific project/work stream and then afterwards apply for funding using a CP-2.

#### CP-1.2 (REM) Removal of Mandate

In order to revoke a mandate from a group, or individual in a group, a CP-1.2 proposal has to be created.

This can happen in two ways:

1) *The group/individual itself no longer wants its mandate within the DAO*
2) *The Community/DAO wants to revoke the mandate of a group/individual in a group*

The group itself has autonomy to include and remove members, but in the case that someone breaks the Code of Conduct (forthcoming), the DAO can propose to remove a group member from the group. 

**GOVERNANCE PROCESS:**

1) *The group/individual itself no longer wants its mandate within the DAO*

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create a Proposal post (still a CP-1.2) on the Forum with an explanation of the revocation of the mandate|-|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github)|-|

2) *The Community/DAO wants to revoke the mandate of a group/individual in a group*

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create an RFC on the Forum (see template for title, content, where to post etc.)|Minimum 7 days|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github)|-|
|3|Create a snapshot vote on [OpenSquare](https://voting.opensquare.io/space/centrifuge)|Minimum 7 days|
|4|Create a Proposal post|-|

If the snapshot vote passes (majority of CFG votes to revoke the mandate), the group/individual will no longer have its mandate.

#### CP-2 (RF) Request for Funding

Any entity (group or individual) who seeks funding from the Treasury, would need to create a CP-2 proposal. There can be different scenarios for an entity applying for funding:

- The entity already created a CP-1 (that passed) and received funding and wants to re-apply
- The entity already created a CP-1.1 (that passed) and wants to apply for funding
- The entity doesn’t have a mandate but wants to apply for funding for a one time service

The Treasury is administered by the Council so only the Council will vote on the proposal - token holders will not vote on it. 

It is possible to make a Treasury proposal on behalf of someone else.

A Treasury proposal can only be made if there are adequate funds in it to cover the funding request.

When creating a request for funding, make sure to provide the calculations for the requested amount and how they will be distributed. You can see an example of how it can be done in [this post](https://gov.centrifuge.io/t/rfc-establishing-a-centrifuge-credit-group/3554).

**GOVERNANCE PROCESS:**

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create an RFC on the Forum (see template for title, content, where to post etc.)|Minimum 7 days|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|3|Create a snapshot vote on OpenSquare|Minimum 7 days|
|4|Create an on-chain Treasury proposal|-|

#### CP-3 (RU) Runtime Upgrades

CP-3 is used to propose Runtime Upgrades. Runtime Upgrades allow developers and community members to change the logic of the chain, or parameter for pallets, without the need for a hard fork.

Runtime Upgrades may contain previously passed CP-4s (General Improvements) - this will be specified in the Proposal post.

**GOVERNANCE PROCESS:**

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|2|Create a Proposal post|-|
|3|Create a Council motion or public proposal|-|
|4|Public referendum|Exactly 7 days|

#### CP-3.1 (EP) Emergency Proposals

CP-3.1 is used to propose emergency proposals in order to avoid or prevent hacks, exploits, attacks, or network halts.

In order to protect the protocol, some actions or changes may take place without prior notice (Council motions + referenda).

When/if the Council motion and referendum have passed, and the Runtime Upgrade has been successfully enacted, a post-mortem must be posted on the Forum with a full description of the issue(s) and the fix.

Given that a public disclosure of a bug, exploit, or hack may lead to (further) exploitation of this vulnerability, all changes should take place without premature public disclosure but should be made public later in a post-mortem.

These types of proposals will be fast-tracked and the voting window in the **referendum may be as short as 3 hours**.

**GOVERNANCE PROCESS:**

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create a post-mortem on the Forum with a description of the issue, along with the fix for it |-|

#### **CP-4 (GI) General Improvements**

This CP is used for proposals that don’t fit under any of the types. In other words, if it is not a CP-1, CP-2, CP-3 or CP-5 (or any of their derivatives), it is a CP-4. 

A CP-4 can therefore be a wide range of proposal types, to improve the protocol or expand the ecosystem, and that require input from the Community. A CP-4 can roughly be divided into two categories; **technical** and **non-technical**.

##### Technical CP-4
These can be proposals for the roadmap and technical features and functionality of the Centrifuge protocol, such as adjustment of fees, burning of tokens, liquidity pairing with another protocol, opening HRMP channels between other parachains etc. If passed, these proposals will typically be part of a Runtime Upgrade (CP-3) afterwards, but not always.

**Non-technical CP-4**
These are proposals that do not require a change on the blockchain, and hence do not require an on-chain vote. This could be co-marketing partnerships, changes to the Governance process, incentivising users with NFTs for participation in Governance, creating events etc.

**GOVERNANCE PROCESS:**

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create an RFC on the Forum (see template for title, content, where to post etc.)|Minimum 7 days|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|3|Create a Proposal post|-|
|4|Create a snapshot vote on [OpenSquare](https://voting.opensquare.io/space/centrifuge)|Minimum 7 days|

For **non-technical proposals**, the process ends here and if the snapshot vote passes (majority of CFG votes in favor of the proposal), the proposal passes. 

For **technical proposals**, if it is a standalone proposal - i.e. not part of a Runtime Upgrade (CP-3) - there will be two more steps. 


|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|5|Create a Council motion or public proposal|-|
|6|Public referendum|Exactly 7 days|

Otherwise, the proposal will be in queue to be implemented in an upcoming Runtime Upgrade.

#### CP-5 (POP) Pool Onboarding Proposal

To be announced.

## Change or improvement
We believe that this proposal will contribute to a more robust and decentralised Governance, where anyone is able to create a CP, by following the guidelines and processes.

Recently, we integrated Subsquare/OpenSquare Voting 1 in our Governance process and one the biggest changes was the introduction of snapshot voting which has replaced our Forum polls.

Another change that this proposal will bring is the introduction of the Centrifuge Proposal Repository (on Github), which will act as register where all CPs must be submitted to.

We are not expecting this to be the final version of our Governance process - this is an on-going process where we might see a few iterations over time. Therefore, it would be greatly appreciated to get input from the Community on this proposal so we collectively find a model that suits the need of our protocol and ecosystem.
