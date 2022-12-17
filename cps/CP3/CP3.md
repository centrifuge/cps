# CP-3 (RU) Runtime Upgrades 

CP-3 is used to propose Runtime Upgrades. Runtime Upgrades allow developers and community members to change the logic of the chain, or parameter for pallets, without the need for a hard fork.

Runtime Upgrades may contain previously passed CP-4s (General Improvements) - this will be specified in the Proposal post.

### GOVERNANCE PROCESS

|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Submit proposal to the Centrifuge Proposals Repository on [Github](https://github.com/centrifuge/cps/tree/main) to get a pull request # |-|
|2|Create a Proposal post on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) (see template below for title, tags and content) |-|
|3|Create a Council motion or public proposal|-|
|4|Public referendum|Exactly 7 days|

If the referendum vote passes, the Runtime Upgrade will be enacted. The Council can choose to fast track the referendum at their discretion.

### TEMPLATE
Note that this post is not an RFC, but a Proposal post. 

In the title of this post, the XXXX is the pull request number from Github and YY is the abbreviation for the proposal type, e.g. (MRF), (RU) etc.

```
Title (on Forum post): CP-XXXX (RU): [Runtime Upgrade YYYY]
Tags (on Forum post): CP-3, month, year
```
#### Body of the post must contain:
```
Proposal type: CP-3
Author(s): Forum handle(s) of author(s)
Member(s): Forum handle(s) of member(s)
Proposal on Proposal Repository (Github): INSERT LINK
Date proposed: yyyy-mm-dd

List of content of this Runtime Upgrade
- Added functionalities, changed parameters etc.
- If CP-4s are included, link to their Proposal post

Detailed description of each content 
- Describe the different content above in details
Governance process for this proposal
- Council Motion/Democracy Proposal
- Fast-track?
- Duration of referendum vote
```

#  CP-3.1 (EP) Emergency Proposals

CP-3.1 is used to propose emergency proposals in order to avoid or prevent hacks, exploits, attacks, or network halts.

In order to protect the protocol, some actions or changes may take place without prior notice (Council motions + referenda).

When/if the Council motion and referendum have passed, and the Runtime Upgrade has been successfully enacted, a post-mortem must be posted on the Forum with a full description of the issue(s) and the fix.

Given that a public disclosure of a bug, exploit, or hack may lead to (further) exploitation of this vulnerability, all changes should take place without premature public disclosure but should be made public later in a post-mortem.

These types of proposals will be fast-tracked and the voting window in the referendum **may be as short as 3 hours**.

### GOVERNANCE PROCESS
|STEP|DESCRIPTION|DURATION|
| --- | --- | :---: |
|1|Create a post-mortem on the [Forum](https://gov.centrifuge.io/c/cfg-governance/chain-governance/18) with a description of the issue, along with the fix for it  |-|

### TEMPLATE
This proposal type doesn’t require any template.
