---
cp: 1
title: Centrifuge Proposal Framework
authors: Governance and Coordination Group (ImdioR, Orhan)
date-proposed: 2022-10-18
date-passed: 2022-11-12
date-modified: 2024-05-13
status: passed
---

# CP1 (Request for Mandate)

A mandate is when an entity (group or individual) asks for, and is given, the legitimacy by the DAO to pursue stated objectives in a specific domain area.

Typically those asking for mandates form ‘Groups’ and become the service provider for a particular type of work is necessary to the Centrifuge Ecosystem. By submitting a proposal for a mandate a group is asking for control over a DAO process.

An example is the mandated PEG - [Protocol Engineering Group](https://github.com/centrifuge/cps/blob/main/cps/CP32.md) - who provide feedback on technical feasibility of improvement proposals in the community, propose technical implementations, and propose a roadmap for CFG token holders to vote on.

Mandates do not need to be proposed for defined or very particular types of work. Mandates should be given to a group/individual where coordination and clear responsibilities are a clear efficiency gain for the DAO (as opposed to work that can happen ad hoc, by individuals). 

Work can be initiated and brought to the DAO without a mandate, but no individual or group may claim to be working on behalf of the DAO without a mandate. Mandated groups must have an objective, mandate related deliverables and a method for reporting on deliverables (such as quarterly reports on what the group has achieved and how funds are administered). The initial facilitator of the group should also be explicitly stated in the proposal.

A mandate indicates long term commitment (i.e. not a one time service, like creating a video for a specific purpose) and hence on-going funding. The maximum funding period is 6 months. This means that every 6 months, the group or individual would need to re-apply for funding by submitting a CP2.

Mandated groups are accountable to the DAO according to the details specified in the CP submitted to GitHub. Being accountable includes responding to other DAO members when inquired and communicating how personnel are recruited or admitted into the group.

See examples below for when a mandate is required.

|MANDATE NEEDED|MANDATE NOT NEEDED|
| --- | --- |
|Marketing content accredited to represent the brand|Research article, social promotion, educational content (youtube, twitter)|
|Official representation of Centrifuge|Running a node|
|Taking control of a process or vertical|Short-term engagements/one-time commitments|

## GOVERNANCE PROCESS

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|2| Create an RFC on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) (see template below for title, tags and content)|Minimum 7 days|
|3|Create a snapshot vote on [OpenSquare](https://voting.opensquare.io/space/centrifuge)|Minimum 7 days|

If the snapshot vote passes (majority of CFG votes in favor of giving the mandate and quorum met), the proposal has passed and the mandate has been obtained. 

## TEMPLATE
```
Title: CPXXX: [TITLE OF PROPOSAL]

Tags: cp1, rfc
```
### Body of the RFC must contain:
```
cp: [XXX]
title:
authors: [forum handles]
contributors: [forum handles]
uses-component: [cp1|cp2|cp3|cp4|cp5|cp32|cp63]
technical-proposal: [yes|no]
requires-onchain: [yes|no]
impacts/modifies:
status: [rfc|voting|passed|rejected]
date-proposed: [YYYY-MM-DD]
date-ended: [YYYY-MM-DD]

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
- Background of the member(s) of the group
- How do they meet and publish activity? 
- What are the roles (e.g. who is the Facilitator and how are they selected?), is there election or selection into this group - how does it work?

Delivery and Reporting
- A timeline of when the objective(s) will be delivered and how this will be reported
```
You can combine a Request for Mandate with a Request for Funding ([CP2](https://github.com/centrifuge/cps/blob/main/cps/CP2/CP2.md)) in the same proposal by using both a component CP1 and a CP2. Then you would need to add the following in the RFC post, compared to the template above:

```
uses-component: CP1, CP2

Budget
- What amount is requested and how is it calculated?
- How are the funds distributed within the group?
- What wallet address is used for the funding request?
```
and add the following step to the governance process:

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|4|Create an on-chain Treasury proposal|-|

**Important:** remember to update the Forum post (title + content) as the proposal progresses through the steps, as explained [here](https://github.com/centrifuge/cps/blob/main/cps/CP0/CP0.md).

# CP1.1 (Changing facilitator)

Groups that have received a mandate via governance voting have full autonomy over how they organise themselves and how their facilitator is selected. The faciliator and the selection process should be clarified in the RFC for the mandate request. The facilitator is the person accountable to the DAO.

Groups should self-select the initial facilitator with a requirement to disclose information such as expertise, experiences, and credentials.

If the facilitator needs to be changed, the group should select one or more candidates, communicating information about their expertise, experiences, and credentials in addition to their justification for why the candidate is fit for the role. Once selected, the GCG should submit an amendment to their CP (where the mandate was obtained) listing the new facilitator, keeping record of all past facilitators. If the group cannot produce any candidates within two weeks of the loss of their initial facilitator, then anyone can come and propose themselves. Essentially, the team uses the forum as a job listing to source candidates.

## GOVERNANCE PROCESS

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|2|Create a post on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) (see template below for title, tags and content) with an announcement of the change of facilitator|-| |-|

## TEMPLATE
```
Title: CPXX: [TITLE OF PROPOSAL]

Tags: cp1.1
```
### Body of the RFC must contain:

```
Uses component: CP1.1
Author(s): Forum handle(s) of author(s)
Impacts: [link to the CP where mandate was obtained]
Date proposed: yyyy-mm-dd

Short Summary 
- One sentence summary of the proposal

Background
- What is the background for changing the facilitator?

Description of Process
- Who is the new facilitator?
- How was the new faciliator selected?

```
The XXX in the title is from the pull request # from GitHub.

# CP1.2 (Removal of Mandate)

In order to revoke a mandate from a group, or individual in a group, a proposal using the CP1.2 component has to be created.

This can happen in two ways:

1) *The group/individual itself no longer wants its mandate within the DAO*
2) *The Community/DAO wants to revoke the mandate of a group/individual in a group*

The group itself has autonomy to include and remove members, but in the case that someone breaks the [Code of Conduct](https://github.com/centrifuge/cps/blob/main/cps/CP29/Appendices/FD4-CoC.md), the DAO can propose to remove a group member from the group. 

## GOVERNANCE PROCESS

1) *The group/individual itself no longer wants its mandate within the DAO*

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|2|Create a post on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) (see template below for title, tags and content) with an explanation of the revocation of the mandate|-| |-|

Once the announcement has been made, and the proposal has been submitted to the Centrifuge Proposals Repository, the group has automatically been revoked of its mandate. 

## TEMPLATE
```
Title: CPXXX: [TITLE OF PROPOSAL]

Tags: cp1.2
```
### Body of the RFC must contain:
```
Uses component: CP1.2
Author(s): Forum handle(s) of author(s)
Impacts: [link to the CP where mandate was obtained]
Date proposed: yyyy-mm-dd

Short Summary 
- One sentence summary of the proposal

Background
- What is the background for wanting to remove the mandate of the group/individual?
```
The XXX in the title is from the pull request # from GitHub.

2) *The Community/DAO wants to revoke the mandate of a group/individual in a group*

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create an RFC on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) (see template below for title, tags and content)|Minimum 7 days|
|2|Submit proposal to the [Centrifuge Proposals Repository](https://github.com/centrifuge/cps) (on Github) to get a pull request #|-|
|3|Create a snapshot vote on [OpenSquare](https://voting.opensquare.io/space/centrifuge)|Minimum 7 days|


If the snapshot vote passes (majority of CFG votes to revoke the mandate and quorum is met), the group/individual will no longer have its mandate.

## TEMPLATE
```
Title: RFC: [TITLE OF PROPOSAL]

Tags: cp1.2
```
### Body of the RFC must contain:
```
Uses component: CP1.2
Author(s): Forum handle(s) of author(s)
Impacts: [link to the CP where mandate was obtained]
Date proposed: yyyy-mm-dd

Short Summary 
- One sentence summary of the proposal

Background
- What is the background for wanting to remove the mandate of the group/individual?
```
**Important:** remember to update the Forum post (tags, link to vote and outcome of the proposal) as the proposal progresses through the stages.