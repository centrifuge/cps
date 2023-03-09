---
cp: 1
title: Centrifuge Proposal Framework
authors: Governance and Coordination Group (ImdioR, Orhan)
date proposed: 2022-10-18
date passed: 2022-11-12
status: passed
---

# CP1 (MRF): Request for Mandate with Funding

A mandate can be interpreted as an entity (group or individual) being given the authority by the DAO to pursue the stated objectives. The entity takes on the responsibility of fulfilling the mandate and accepts accountability to the DAO over this. 

Work can be initiated and brought to the DAO without a mandate, but no individual or group may claim to be working on behalf of the DAO without a mandate. 

A mandate indicates long term commitment (i.e. not a one time service, like creating a video for a specific purpose) and hence on-going funding. The maximum funding period is 6 months. This means that every 6 months, the group or individual would need to re-apply for funding by submitting a CP2.

### GOVERNANCE PROCESS

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create an RFC on the [Forum](https://gov.centrifuge.io/c/cfg-governance/request-for-comments/37) (see template below for title, tags and content)|Minimum 7 days|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|3|Create a snapshot vote on [OpenSquare](https://voting.opensquare.io/space/centrifuge)|Minimum 7 days|
|4|Create a Proposal post on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18)|-|

If the snapshot vote passes (majority of CFG votes in favor of giving the mandate), the proposal has passed and the mandate has been obtained. 

The next step is the funding process, which will be an on-chain Treasury Proposal, voted on by the Council.
|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|5|Create an on-chain Treasury proposal|-|

### TEMPLATE
```
Title: RFC: [TITLE OF PROPOSAL]

Tags: cp-1, month, year
```
#### Body of the RFC must contain:
```
Proposal type: CP1
Author(s): Forum handle(s) of author(s)
Member(s): Forum handle(s) of member(s)
Date proposed: yyyy-mm-dd

Short Summary 
- One sentence summary of the mandate sought

High level objective 
- A short description of the objective that this proposal will achieve

Background 
- What are the historical and contextual factors that make this proposal relevant and aligned with the mission?

Description of Activity 
- Give details on the activity, describes the new process or feature and the problem it is solving

Change or improvement 
- What is the change or improvement that this mandate will bring?

Alignment to the mission of Centrifuge DAO
- Explain why this is important and aligned with the mission

Description of Group
- Background of the member(s) of the group seeking funding
- How do they meet and publish activity? 
- What are the roles, is there election or selection into this group - how does it work?

Budget
- What amount is requested and how is it calculated?
- How are the funds distributed within the group?
- What wallet address is used for the funding request?

Delivery and Reporting
- A timeline of when the objective(s) will be delivered and how this will be reported
```

# CP1.1 (MR) Mandate Request without Funding

Same as CP1, just without funding (i.e. no step 5 and Budget does not need to be specified in the RFC).

A group can make a proposal for seeking a mandate for a specific project/work stream and then afterwards apply for funding using a CP2.

# CP1.2 (REM) Removal of Mandate

In order to revoke a mandate from a group, or individual in a group, a CP1.2 proposal has to be created.

This can happen in two ways:

1) *The group/individual itself no longer wants its mandate within the DAO*
2) *The Community/DAO wants to revoke the mandate of a group/individual in a group*

The group itself has autonomy to include and remove members, but in the case that someone breaks the [Code of Conduct](https://github.com/centrifuge/cps/blob/main/cps/CP29/Appendices/FD4-CoC.md), the DAO can propose to remove a group member from the group. 

### GOVERNANCE PROCESS

1) *The group/individual itself no longer wants its mandate within the DAO*

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create a Proposal post (still a CP1.2) on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) with an explanation of the revocation of the mandate|-|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github)|-|

Once the announcement has been made, and the proposal has been submitted to the Centrifuge Proposals Repository, the group has automatically been revoked of its mandate. 

2) *The Community/DAO wants to revoke the mandate of a group/individual in a group*

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create an RFC on the [Forum](https://gov.centrifuge.io/c/cfg-governance/request-for-comments/37) (see template below for title, tags and content)|Minimum 7 days|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github)|-|
|3|Create a snapshot vote on [OpenSquare](https://voting.opensquare.io/space/centrifuge)|Minimum 7 days|
|4|Create a Proposal post on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18)|-|

If the snapshot vote passes (majority of CFG votes to revoke the mandate), the group/individual will no longer have its mandate.

### TEMPLATE
```
Title: RFC: [TITLE OF PROPOSAL]

Tags: cp-1.2, month, year
```
#### Body of the RFC must contain:
```
Proposal type: CP1.2
Author(s): Forum handle(s) of author(s)
Related to: link to the CP1 or CP1.1 where mandate was obtained
Date proposed: yyyy-mm-dd

Short Summary 
- One sentence summary of the proposal

Background
- What is the background for wanting to remove the mandate of the group/individual?
```
