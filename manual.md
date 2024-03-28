# Governance Manual [v0.2]

> ❗ This document describes the current governance processes of Radworks. For more on how this document is maintained please refer to [contributing.md](/contributing.md)


# Overview

Radworks is governed by on-chain and off-chain governance processes. These processes together make up Radworks' **governance system**. Holders of Radworks' native governance token ($RAD) can participate in governance by creating, discussing and voting on RAD Governance Proposals (RGPs).

### On-chain

The Radworks Treasury is controlled by a tokenized governance mechanism ([Compound-Governor](https://wiki.tally.xyz/docs/compound-governor)) via the project’s native governance token ($RAD). As members of Radworks, $RAD holders participate in the decision-making around the treasury by voting and creating on-chain governance proposals composed of executable actions. 

Currently, these actions include:

- Treasury distributions of assets (e.g. RAD, ETH, and USDC)
- Upgrades to the on-chain governance system (e.g. Quorum, Timelock)
- Changes to parameters of Treasury-governed protocols (e.g. Drips)

To learn more about token governance and how Radworks’ on-chain governance system works, [see here](https://wiki.tally.xyz/docs/compound-governor).

### Off-chain

In addition to the on-chain governance system, Radworks manages a set of off-chain processes and resources that define the rules for participating in governance. These processes and resources are maintained off-chain, but updates to these documents still require formal community approval via Snapshot vote. An off-chain review process (see [Formal Review](#formal-review) is also required for all proposals before they can be submitted on-chain.

See _[Proposal Process](#proposal-process)_ for more info.

# **Governance Toolkit**

The primary tools for Radworks governance are:

- **[Snapshot](https://snapshot.org/#/gov.radworks.eth)**: Off-chain voting platform for *Formal Review*
- **[Tally](https://www.tally.xyz/gov/radworks)**: Platform for on-chain delegation, voting, and proposal creation. 
- **[Discourse](https://community.radworks.org/):** Community forum for discussion about governance proposals and topics.
- **[Discord](https://discord.gg/radworks)**: For governance announcements and informal community discussion.

# Proposal Types

All proposals are considered a RGP. There are three main categories of RGPs:

| Type | Description | Process |
| --- | --- | --- |
| Executable | On-chain actions such as treasury distributions, updates to contract parameters, and upgrades to governance system. | Request for Comments → Formal Review → Submission |
| Social | Off-chain changes that can not be enforced by governance on-chain but should have community approval (e.g. updates to the governance process) | Request for Comments → Formal Review  |

Each proposal type has a designated [template](/templates/).

# Proposal Process

The Radworks governance process is defined by three separate phases: _Request for Comments (RFC)_, _Formal Review_, and _Submission_. Before a RGP can be submitted on-chain, it must first complete **an off-chain review process**. Having a public off-chain review process allows for proposals to be reviewed, discussed, and improved by the Radworks community before initiating an on-chain vote. This review process includes publishing a *Request for Comments (RFC)* and  passing a *Formal Review*. These steps help provide on-chain voters with more context on community sentiment and proposal development which supports more informed and less contentious decisions. It also protects the Radworks community by ensuring that any proposal being submitted on-chain has been vetted and reviewed in a transparent manner.

Each phase has specific timelines and requirements:

| Request for Comments (RFC) | Formal Review | Submission |
| --- | --- | --- |
| Forum post | Snapshot poll | On-chain vote |
| 14 days | 7 day | 3 days vote, 2 day timelock  |

RAD Governance Proposals (RGPs) must be formally labeled with the phase of the proposal, #, and title (e.g. [RFC/Formal Review/Submission][RGP - #] - [PROPOSAL TITLE])

## **Request for Comments**

The _Request for Comments (RFC)_ phase is used to actively review proposal drafts that are being submitted to be considered in a proposal cycle. While drafts of proposals can be posted on the forum _at any time_, this stage represents the official period for the community to review and provide feedback on proposals that will be voted on in a given cylce. The feedback provided during this phase allows authors to refine and improve their proposals with community feedback.

In order for a draft proposal to be formally included in a [proposal cycle](#proposal-cycles), it must be labeled with [RFC] and formatted using the templates linked below. 

> 💡 For more complex proposals, it is encouraged to post early drafts in advance of the intended proposal cycle to allow for ample discussion and debate. These early drafts should be posted under [Proposal Drafts](https://community.radworks.org/c/governance/proposal-archive/46) on the forum. Authors are encouraged to specify the expected or tentative proposal cycle for their submission.

When preparing the proposal drafts for the _RFC_ phase, proposal authors should:
- Use [these templates](https://github.com/radicle-foundation/radworks-governance/tree/main/templates) to create their proposals. Please see the 'Proposal Types' section below to determine which template to use. 
- Include as much context and detail as possible to help the community to review what is being proposed. 
- Post their proposal under [Active Proposals](https://community.radworks.org/c/governance/proposals/18) on the forum by the _first Monday_ of each cycle (see 'Proposal Cycles' for details).  

## **Formal Review**

The _Formal Review_ phase serves as the final review step in the governance process before proposals are submitted on-chain. Proposals in this phase incorporate feedback from the _RFC_ phase, and are accompanied by an off-chain Snapshot poll to gauge consensus. All Snapshot polls must begin on **5:00pm GMT+2** the **third Monday of the month** and end at **5:00pm GMT+2** on the **following Monday**. Each Snapshot poll should have three voting options: `Yes` `No` and `Abstain`. 

During _Formal Review_, proposal authors are required to:
- Publish a new version of their proposal on the forum that incorporates feedback from the *RFC* phase. Please use [this template](/templates/05-Formal-Review-forum-post-header) as a guide. Proposals in this stage should be posted under the [Active Proposals](https://community.radworks.org/c/governance/proposals/18) category on the forum.
- If applicable, include a draft of the executable proposal code. Use [this template](/templates/07-proposal-code-template.md) to draft the proposal code. 
- Publish a corresponding Snapshot poll on the [Radworks Snapshot page]([url](https://snapshot.org/#/gov.radworks.eth)). To publish a Snapshot poll for Formal Review, you must be added as an 'author' in the Radworks Snapshot space. This measure is in place to prevent spam proposals. Please reach out to Shelby (shelb_ee#9785 on Discord) with the Ethereum address of the party posting your proposal.
- Please use [this template](/templates/08-snapshot-poll-template) to prepare the Snapshot poll. 

A Governance Facilitator will link the Snapshot poll to your Formal Review post once ready. 

> 💡 If a proposal does not pass _Formal Review_, it can be resubmitted in the next governance cycle. The new draft should take into account feedback from the community. Please include a note at the top of the resubmitted proposal explaining why it is being resubmitted and explitely list any changes that were made.

## **Submission**

Submitting a proposal on-chain is the final step in the governance process. An RGP can be submitted to on-chain governance by anyone who has an amount of $RAD greater than or equal to **1% of the total $RAD supply** delegated to their address (i.e. ≥ 1M $RAD). If a proposal author does not meet this requirement, they should reach out to the Governance Committee as soon as possible. 

For Submission, proposal authors are required to: 

- Post an updated version of their proposal on the forum that incorporats feedback from the _RFC_ and _Formal Review_ phases. Please use [this template](https://github.com/radicle-foundation/radworks-governance/blob/main/templates/06-Submission-forum-post-header) as a guide. Proposals in this stage should be posted under the [Active Proposals](https://community.radworks.org/c/governance/proposals/18) category on the forum.
- Include or update the executable on-chain code in the Submission post using [this template]([url](https://github.com/radicle-foundation/radworks-governance/blob/main/templates/07-proposal-code-template.md)). Please always double check the addresses!
- Create an on-chain proposal using [Tally](https://docs.tally.xyz/knowledge-base/proposals/creating-proposals).
- The forum post and on-chain proposal should be submitted no later than the fourth Tuesday of the proposal cycle (see [Proposaal Cycles](###ProposalCycles)). 

If a proposal does not pass _Submission_, it can be resubmitted in the next governance cycle. The new draft should take into account feedback from the community. Please include a note at the top of the resubmitted proposal explaining why it is being resubmitted and explitely list any changes that were made.

# Proposal Cycles

Proposals are reviewed in **monthly cycles** to sync voting periods and establish a manageable cadence for governance participants. 

| Monthly Schedule | Stage | Weekly Schedule | Action |
| --- | --- | --- | --- |
| Week 1 | Request for Comments | First Monday | Start of the next proposal cycle and deadline to post proposal to forum under [Active Proposals](https://community.radworks.org/c/governance/proposals/18) |
| Week 2 | Request for Comments | Second Monday | Join monthly Proposal Review call to present and discuss proposal with community |
| Week 3 | Formal Review | Third Monday |  Open proposal for Formal Review |
| Week 4 | Submission | Fourth Tuesday | Submit proposal on-chain |

**Proposals can be posted on the forum for discussion at anytime throughout the monthly cycle, but if a proposal is posted after the first Monday deadline, they must be included in the next cycle. Proposal drafts & ideas should be posted in the [Proposal Drafts](https://community.radworks.org/c/governance/proposal-archive/46) category on the forum.**

### Proposal Review Calls
Proposal Reviews are monthly calls take place on the second Wednesday of each month. These calls are a time for proposal authors to discuss their active proposals and answer questions from the community. The calls will be recorded and [archived](https://www.youtube.com/playlist?list=PLUUjDC9sOrpktWjO7jNFwsisK0vi5d_Tx) for reference. _Proposal authors are expected to make an effort to attend these calls and should come prepared to answer questions and discuss their proposal with attendees._


# Voting

Voting requires $RAD tokens, which can be [obtained here](https://docs.radworks.org/community/obtaining-rad). One $RAD token is equal to one vote. Voting takes place both on- and off-chain:

- **Formal Reviews:** *Off-chain* consensus checks done with [Snapshot polls](https://snapshot.org/#/gov.radworks.eth).

- **Submissions:** *On-chain* voting for RGPs take place on [Tally](https://www.tally.xyz/gov/radworks)

## Voting Thresholds

Once proposed, participants can vote for/against the proposal on-chain with their RAD. An RGP is **approved** if it satisfies the following minimum vote thresholds:

- **Quorum:** The minimum number of RAD votes required to be cast in support of a proposal in order for a quorum to be reached and for a vote to succeed. Quorum is currently measured as **a % of the total $RAD supply.** The required quorum to pass a proposal is **4% (4M $RAD) of total supply (100M $RAD)**
    
- **Approval Threshold:** If quorum is met, the proposal passes if a majority of the votes are “in-favor”.

> *Formal Reviews* and *Submissions* are required to meet quorum requirements.

**Submission triggers a 3-day voting period. If passed, the proposal is queued for 48hrs, then it can be executed.**


# Delegating

To participate in off-chain and on-chain voting, $RAD must be delegated to the address that will be used to vote. Delegation can be executed via various governance management platforms (e.g. [Tally](https://www.tally.xyz/gov/radworks)). After connecting a wallet to one of these platforms, the token holder can choose to delegate the voting weight held in that wallet to the address (or addresses) of their choice:

- The owner’s own wallet, if they would like to vote on their own.
- Another user's wallet, if they would like the other user to vote on their behalf.

Once delegation is completed, the voting weight of the RAD can be used to vote. See this [FAQ](https://docs.radworks.org/community/faq) for further information about delegation and voting.

> Any delegation made on-chain will be mirrored to Snapshot for off-chain votes - i.e. any $RAD that is delegated to your wallet on-chain will be able to be able to be used to vote in off-chain Snapshot polls.

> In order to utilize delegated voting power in a vote, delegation needs to take place *before* the vote goes live. 

> Delegation only needs to be set up once. The only time you need to redelegate is to change or remove the address you are delegating to, otherwise delegation will continue to the asigned address.

> In addition to the Code of Conduct, Radworks Delegates are expected to adhere to our Delegate Standards, a set of requirements for ensuring healthy & safe community governance. Please review [the standards](https://govradicle.super.site/delegate-standards) before announcing yourself as a delegate 👇

## Never miss a vote! 🤳

The best way to get live governance updates is by following the Radworks Twitter ([@radworks_](https://twitter.com/radworks_)) or follow the [📢 announcements](https://discord.gg/xaHa6XEQ) channel on the Radworks Discord server. 

You can subscribe to our [community calendar](https://calendar.google.com/calendar/u/0?cid=Y19kMmY5YzQxYWE1OTgxMWI5OGMzNDNjNjM5M2U5OWYwZmM4MjdmMjBlNjNjMmNlODk0YTcxNzczZmNkNTc3OGY1QGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20) that includes reminders for Quarterly Community Calls, monthly Proposal Review calls and each week of the monthly governance cycle.



