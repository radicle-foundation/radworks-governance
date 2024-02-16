# Governance Manual [v0.2]

> ❗ This document describes the current governance processes of Radworks. It is version-controlled and can only updated via off-chain approval.

> 📝 For more on how this document is maintained please refer to contributing.md


# Overview

Radworks is governed by on-chain and off-chain governance processes. These together make up Radworks' **governance system** 

### On-chain

The Radworks Treasury is controlled by a tokenized governance mechanism ([Compound-Governor](https://wiki.tally.xyz/docs/compound-governor)) via the project’s native governance token ($RAD). As members of Radworks, $RAD holders participate in the decision-making around the treasury by voting and creating on-chain governance proposals composed of executable actions. 

Currently, these actions include:

- Treasury distributions of assets (e.g. RAD, ETH, and USDC)
- Upgrades to the on-chain governance system (Compound Governor)
- Changes to parameters of Treasury-governed contracts (e.g. Drips)

To learn more about token governance and how Radworks’ on-chain governance system works, [see here](https://wiki.tally.xyz/docs/compound-governor).

### Off-chain

In addition to the on-chain governance system, Radworks manages a set of off-chain processes and resources that define the rules for participating in the DAO. These processes and resources are maintained off-chain, but updates to these documents still require formal community approval via Snapshot vote. An off-chain review process is also required for all proposals before they can be submitted on-chain.

See _Proposal Process_ for more info.

## **Governance Toolkit**

The primary tools for Radworks governance are:

- **[Snapshot](https://snapshot.org/#/gov.radworks.eth)**: Off-chain voting platform for *Formal Reviews*
- **[Tally](https://www.tally.xyz/gov/radworks)**: Platform for delegation, on-chain voting, and proposal creation. 
- **[Discourse](https://community.radworks.org/):** Community forum for discussion about governance proposals and topics.
- **[Discord](https://discord.gg/radworks)**: For governance announcements and informal governance discussion.

## Proposal Process

| Discussion | Formal Review | Submission |
| --- | --- | --- |
| Forum post | Snapshot poll | On-chain vote |
| ≥ 7 days | 7 day | 3 days vote, 2 day timelock  |

RAD Governance Proposals (RGPs) must be formally labeled with the phase of the proposal, #, and title (e.g. [Discussion/Formal Review/Submission][RGP - #] - [PROPOSAL TITLE])

Before a RGP can be submitted on-chain, it must first complete **an off-chain review process**. Having a public off-chain review process allows for proposals to be reviewed, discussed, and improved by the Radworks community before reaching an on-chain vote. This process includes a *Discussion* and a *Formal Review*. These steps help provide on-chain voters with more context on community sentiment and proposal development which supports more informed and less contentious decisions. It also protects the Radworks community by ensuring that any proposal being submitted on-chain has been vetted and reviewed in a transparent manner.

**Discussion**

The ***Discussion*** phase is used to review the first draft of new proposals. This is the primary period for the community to review and provide feedback on proposals drafts. The more feedback provided during this phase allows for more detailed and refined proposals to vote on in later stages.

When preparing the proposal drafts for the _Discussion_ phase, proposal authors should:
- Use [these templates](https://github.com/radicle-foundation/radworks-governance/tree/main/templates) to create their proposals
- Try to include as much detail as possible in this first draft of their proposals
- Post their proposal drafts under [Proposal Drafts](https://community.radworks.org/c/governance/discussions/19) on the forum by the _second Monday_ of each cycle (see 'Proposal Cycles' for details).  

**Formal Review**

The _Formal Review_ phase serves as the final review step in the governance process before proposals are submitted on-chain. Proposals in this phase incorporate feedback from the _Discussion_ phase, and are accompanied by an off-chain Snapshot poll to gauge consensus for their advancement. All Snapshot polls must begin on **5:00pm GMT+2** the **third Monday of the month** and end at **5:00pm GMT+2** on the **following Monday**. Each Snapshot poll should have three voting options: `Yes` `No` and `Abstain`. 

During _Formal Review_, proposal authors are required to:
- Publish an new version of their proposal on the forum that incorporates feedback from the *Discussion* phase. Proposals in this stage should be posted under the [Active Proposals](https://community.radworks.org/c/governance/proposals/18) category on the forum. 
- If applicable, inlcude a draft of the executable proposal code for the community to review. 
- Publish a corresponding Snapshot poll to your proposal. To initiate a Snapshot poll for Formal Review, you must be added as an 'author' in our Snapshot space. This measure is in place to prevent spam proposals. Please reach out to Shelby (shelb_ee#9785 on Discord) with the Ethereum address of the party posting your proposal. Proposal authors should include a link to the Snapshot poll at the top of their proposal draft on the forum.

If a proposal does not pass _Formal Review_, it can be resubmitted in the next governance cycle. The new draft should take into account feedback from the community. Please include a note at the top of the resubmitted proposal explaining why it is being resubmitted and explitely list any changes that were made.

**Submission**

Submitting a proposal on-chain is the final step in the governance process. An RGP can be submitted to on-chain governance by anyone who has an amount of $RAD greater than or equal to **1% of the total $RAD supply** delegated to their address (i.e ≥ 1M $RAD). If a proposal author does not meet this requirement, they should reach out to the Governance Committee as soon as possible. 

For Submission, proposal authors are required to: 
- Post an updated version of their proposal on the forum that incorporates feedback from the _Discussion_ and _Formal Review_ phases.
- Inlcude links to both the *Discsussion* and the *Formal Review* versions of the proposal in the final Submission post.
- Include any executable on-chain code in the Submission post. Please add or update the corresponding proposal code in the [proposal code archive](https://github.com/radicle-foundation/radworks-governance/tree/main/proposals) using this template [INSERT LINK WHEN READY] if not done so already. This version of the proposal should also be posted under the [Active Proposals](https://community.radworks.org/c/governance/proposals/18) category on the forum.

If a proposal does not pass _Submission_, it can be resubmitted in the next governance cycle. The new draft should take into account feedback from the community. Please include a note at the top of the resubmitted proposal explaining why it is being resubmitted and explitely list any changes that were made.

### Proposal Types

All proposals are considered a RGP. There are three main categories of RGPs:

| Type | Description | Process |
| --- | --- | --- |
| Executable | On-chain actions such as treasury distributions, updates to contract parameters, and upgrades to governance system. | Discussion → Formal Review → Submission |
| Social | Changes that can not be enforced by the DAO on-chain (e.g. updates to Governance Manual) | Discussion → Formal Review  |
| Consensus | Ad-hoc changes that “should” have community approval, but aren’t classified by an Executable or Social proposal | Discussion → Formal Review |

Each proposal type has a designated [template](https://github.com/radicle-foundation/radworks-governance/tree/main/templates).

### Proposal Cycles

Radworks manages proposals in **monthly cycles** to sync voting periods and establish a manageable cadence for governance participants. 

| Monthly Schedule | Stage | Weekly Schedule | Action |
| --- | --- | --- | --- |
| Week 1 | Discussion | First Monday  | Start of the next proposal cycle |
| Week 2 | Discussion | Second Monday  | Deadline to post proposal to forum under [Proposal Discussions](https://community.radworks.org/c/governance/discussions/19) |
| Week 2 | Discussion | Second Wednesday | Join monthly Proposal Review call to present and discuss proposal with community |
| Week 3 | Formal Review | Third Monday |  Open proposal for Formal Review |
| Week 4 | Submission | Fourth Tuesday | Submit proposal on-chain |

**Proposals can be posted to the forum for Discussion at anytime throughout the monthly cycle, but require at least 7 days on the forum to be considered for that month’s voting cycle. If proposal are posted after the second Monday deadline of a proposal cycle, they will be included in the next cycle. New proposals should be posted in the [Proposal Discussions](https://community.radworks.org/c/governance/discussions/19) sub-category under the _Governance_ category on the forum.**

### Proposal Reviews
Proposal Reviews take place on the second Wednesday of each month. These calls are a time for proposal authors to discuss and answer questions on their active proposals that will be voted on this cycle. The calls will be recorded and archived for reference. _Proposal authors are expected to make an effort to attend these calls and should come prepared to answer questions and discuss their proposal with attendees._

## Voting

Voting requires $RAD tokens, which you can [obtain here](https://docs.radworks.org/community/obtaining-rad). One $RAD token is equal to one vote. Voting takes place both on- and off-chain:

- **Formal Reviews:** *Off-chain* consensus checks done with [Snapshot polls](https://snapshot.org/#/gov.radworks.eth).

- **Submissions:** *On-chain* voting for RGPs take place on [Boardroom](https://boardroom.io/radworks/proposals) or [Tally](https://www.tally.xyz/gov/radworks)

### Voting Thresholds

Once proposed, participants can vote for/against the proposal on-chain with their RAD. An RGP is **approved** if it satisfies the following minimum vote thresholds:

- **Quorum:** The minimum number of RAD votes required to be cast in support of a proposal in order for a quorum to be reached and for a vote to succeed. Quorum is currently measured as **a % of the total $RAD supply.** The required quorum to pass a proposal is **4% (4M $RAD) of total supply (100M $RAD)**
    
  *Formal Reviews* and *Submissions* are required to meet quorum requirements.
    
- **Approval Threshold:** If quorum is met, the proposal passes if a majority of the votes are “in-favor”.

**Proposals can be posted to the forum for Discussion at anytime throughout the monthly cycle, but requires at least 7 days on the forum to be considered for that month’s voting cycle*

**Submission triggers a 3-day voting period. If passed, the proposal is queued for 48hrs, then it can be executed.**

## Delegating

On-chain voting is enabled by delegating voting rights to the address (or addresses) of the token holder's choice:

- The owner’s own wallet, if they would like to vote on their own.
- Another user's wallet, if they would like the other user to vote on their behalf.
- No wallet, if they don't want to vote.

To participate in off-chain and on-chain voting, you have to first delegate the voting weight of your RAD. This can be done via various governance management platforms (e.g. [Tally](https://www.tally.xyz/gov/radworks) or [Boardroom](https://boardroom.io/radworks/proposals). After connecting your wallet to one of these platforms, you can choose to delegate the voting weight held in that wallet to either yourself or another address. Once delegation is completed, the voting weight of the RAD can be used to vote.

> Any delegation made on-chain will be mirrored to Snapshot for off-chain votes - i.e. any $RAD that is delegated to your wallet on-chain will be able to be able to be used to vote in off-chain Snapshot polls.

> In order to utilize delegated voting power in a vote, delegation needs to take place *before* the vote goes live. 

> Delegation only needs to be set up once. The only time you need to redelegate is to change or remove the address you are delegating to, otherwise delegation will continue to the asigned address.

> In addition to the Code of Conduct, Radworks Delegates are expected to adhere to our Delegate Standards, a set of requirements for ensuring healthy & safe community governance. Please review [the standards](https://govradicle.super.site/delegate-standards) before announcing yourself as a delegate 👇

### Never miss a vote! 🤳

The best way to get live governance updates is by following the Radworks Twitter ([@radworks_](https://twitter.com/radworks_)) or follow the [🏛️governance-updates](https://discord.gg/sUJ2vaxh) channel on Discord. These accounts act as governance “ticker” accounts and include all of the information and links needed to participate in voting. 

You can subscribe to our [community calendar](https://calendar.google.com/calendar/u/0?cid=Y19kMmY5YzQxYWE1OTgxMWI5OGMzNDNjNjM5M2U5OWYwZmM4MjdmMjBlNjNjMmNlODk0YTcxNzczZmNkNTc3OGY1QGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20) that includes reminders for Quarterly Community Calls, monthly Proposal Review calls and each week of the monthly governance cycle.



