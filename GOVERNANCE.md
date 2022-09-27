# Curve Governance

This document defines governance policies of the Curve project. It is meant to be followed by all projects under the Curve organization.

## Roles and Responsibilities

### PMC

PMC members demonstrate a strong commitment to the project with views in the interest of the broader Curve project.

Responsibilities include:

* Own the overall direction of the Curve project.
* Speaking on behalf of the project.
* Maintaining guidelines of the project.
* Nominating new committee members.

Membership of PMC is by invitation only and must be approved by a consensus of the PMC. A committee member is considered emeritus by their own declaration. An emeritus member may request reinstatement to the PMC, which will be sufficient to restore him or her to active committee member.

Membership of PMC can be revoked by a consensus vote of the PMC other than the member in question.

The current list of PMC members is as below, in alphabetical order on last name.

| Name                                     | Represents | GitHub                                             |
|------------------------------------------|-----|:---------------------------------------------------|
| Pan Wang <hzwangpan@corp.netease.com>       | NetEase | [Wangpan](https://github.com/Wangpan)              |
| Xiaocui Li <lixiaocui1@corp.netease.com>         | NetEase | [ilixiaocui](https://github.com/ilixiaocui)        |
| Yifeng Xu <yfxu@corp.netease.com>              | skypexu    | [BusyJay](https://github.com/skypexu)              |

### Teams

Teams are persistent open groups that focus on a part of the Curve project. A team has its reviewer, committer and maintainer, and owns one or more repositories. Team level decision making comes from its maintainers.

The current list of teams is under the [teams](teams/README.md) directory.

#### Reviewers

Reviewers are individuals who actively make contribution and are willing to participate in the code review of new contributions. We identify reviewers from active contributors. The committers should explicitly solicit reviews from reviewers. High-quality code reviews prevent technical debt for long-term and are crucial to the success of the project. A pull request to the project has to be reviewed by at least one reviewer in order to be merged.

Review access is by invitation only and must be approved by consensus of the maintainers. A reviewer is considered emeritus by their own declaration. An emeritus reviewer may request reinstatement of review access from the maintainers, which will be sufficient to restore him or her to active reviewer status.

Review access can be revoked by consensus by the maintainers (except the reviewer in question if they are also a maintainer).

#### Committers

Committers are individuals who are granted the write access to the repositories belong to the team. A committer is usually responsible for a certain area or several areas of the code where they oversee the code review process. The area of contribution can take all forms, including code contributions and code reviews, documents, education, and outreach. Committers are essential for a high quality and healthy project.

Commit access is by invitation only and must be approved by consensus of the maintainers. A committer is considered emeritus by their own declaration. An emeritus committer may request reinstatement of commit access from the maintainers, which will be sufficient to restore him or her to active committer status.

Commit access can be revoked by consensus by the maintainers (except the committer in question if they are also a maintainer).

#### Maintainers

The maintainers consist group of active committers that moderate the discussion, manage the project release, and proposes new committers or maintainers. Potential candidates are usually proposed via an internal discussion among maintainers, followed by a consensus approval, i.e. a concrete number of approvals, and no vetoes. Any veto must be accompanied by reasoning. Maintainers should serve the community by upholding the community practices and guidelines Curve a better community for everyone. Maintainers  should nominate new reviewer, committers and maintainers, and should also strive to only nominate new candidates outside of their own organization.

Membership of the maintainers is by invitation only and must be approved by a consensus of the maintainers. A maintainer is considered emeritus by their own declaration. An emeritus member may request reinstatement to the maintainers, which will be sufficient to restore him or her to active maintainers.

Membership of the maintainers can be revoked by a consensus vote of all the maintainers other than the member in question.

#### Contributor

Community contributors with one or more merged PRs in the Curve project related repo.

We encourage everyone to participate in the community through various forms such as project testing, document writing, and bug reporting. After becoming a Contributor, you can also get our commemorative mug, so contribute your first PR now!

## Decision Making

Within the Curve project, different types of decisions require different forms of approval. For example, the previous section describes several decisions which require 'consensus' approval. This section defines how voting is performed, the types of approvals, and which types of decision require which type of approval.

### Voting

Decisions regarding the project are made by votes on [the primary project community repository](https://github.com/opencurve/community). Votes are clearly indicated by a pull request adding an entry under [votes](votes/README.md) folder. Votes may contain multiple items for approval and these should be clearly separated. Voting is carried out by replying to the vote pull request. Voting may take three flavors

* **+1**: 'Yes,' 'Agree,' or 'the action should be performed.'
* **0**: Neutral about the proposed action (or mildly negative but not enough so to want to block it).
* **-1**: This is a negative vote. On issues where consensus is required, this vote counts as a veto. All vetoes must contain an explanation of why the veto is appropriate. Vetoes with no explanation are void. It may also be appropriate for a -1 vote to include an alternative course of action.

All participants in the Curve project are encouraged to show their agreement with or against a particular action by voting. For team decisions, only the votes of active team maintainers are binding. For project decisions, only the votes of active PMC members are binding. Non-binding votes are still useful for those with binding votes to understand the perception of an action in the wider Curve community.

Voting can also be applied to changes already made to the Curve codebase. These typically take the form of a veto (-1) in reply to the commit message sent when the commit is made. Note that this should be a rare occurrence. All efforts should be made to discuss issues when they are still patches before the code is committed.

Only active (i.e. non-emeritus) maintainers and PMC members have binding votes.

### Approvals

These are the types of approvals that can be sought. Different actions require different types of approvals.

* **Consensus**: Consensus requires 2 binding +1 votes and no binding vetoes.
* **Lazy Majority**: A lazy majority vote requires 2 binding +1 votes and more binding +1 votes than -1 votes.
* **2/3 Majority**: Some actions require a 2/3 majority to pass. Such actions typically affect the foundation of the project (e.g. adopting a new codebase). The higher threshold is designed to ensure such changes are strongly supported. To pass this vote requires at least 2/3 of binding vote holders to vote +1.

> In order to address the case of insufficient active binding voters to reach 2/3 majority, one can follow the process below to exclude a binding vote from the counting of this particular voting thread. 
> 
> 1. Wait until the minimum length of the voting passes.
> 2. Publicly reach out via mentioned to the remaining binding voters in the voting pull request for at least 2 attempts with at least 7 days between two attempts.
> 3. If the binding voter being contacted still failed to respond after all the attempts, the binding voter will be considered as inactive for the purpose of this particular voting.

### Vetoes

A valid, binding veto cannot be overruled. If a veto is cast, it must be accompanied by a valid reason explaining the reasons for the veto. The validity of a veto, if challenged, can be confirmed by anyone who has a binding vote. This does not necessarily signify agreement with the veto - merely that the veto is valid.

If you disagree with a valid veto, you must lobby the person casting the veto to withdraw their veto. If a veto is not withdrawn, the action that has been vetoed must be reversed in a timely manner.

### Actions

PMC is permitted to take over team level decision making from the team maintainers, e.g., new maintainer or maintainer removal by consensus. However, it is a safety valve and the committee should avoid actually doing that.

| Actions                  | Description                                                                                                                                                                                                                                         | Approval      | Binding Voters           | Minimum Length (days) |
| :----------------------- |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------| :------------ | :----------------------- | :-------------------- |
| New Reviewer             | When a new reviewer is proposed for the team.                                                                                                                                                                                                       | Lazy Majority | Active maintainers       | 3                     |
| New Committer            | When a new committer is proposed for the team.                                                                                                                                                                                                      | Consensus     | Active maintainers       | 6                     |
| New Maintainer           | When a new maintainer is proposed for the team.                                                                                                                                                                                                     | Consensus     | Active maintainers       | 6                     |
| New Infra Member         | When a new member of the infrastructure team is proposed.                                                                                                                                                                                           | Consensus     | Active committee members | 3                     |
| New Committee Member     | When a new member of the PMC is proposed. Note: such actions will also be referred to the CNCF by the PMC.                                                                                                                                          | Consensus     | Active committee members | 6                     |
| Reviewer Removal         | When removal of review privileges is sought.                                                                                                                                                                                                        | Consensus     | Active maintainers       | 6                     |
| Committer Removal        | When removal of commit privileges is sought.                                                                                                                                                                                                        | Consensus     | Active maintainers       | 6                     |
| Maintainer Removal       | When removal of maintain privileges is sought. Note: such actions will also be referred to the CNCF by the PMC.                                                                                                                                     | Consensus     | Active maintainers       | 6                     |
| Infra Member Removal     | When removal of the infrastructure team membership is sought.                                                                                                                                                                                       | Consensus     | Active committee members | 6                     |
| Committee Member Removal | When removal of committee membership is sought.                                                                                                                                                                                                     | Consensus     | Active committee members | 6                     |
| Adoption of New Codebase | Adoption of large existing external codebase. This refers to contributions big enough that potentially change the shape and direction of the project with massive restructuring and future maintenance commitment, or potentially build a new team. | 2/3 majority  | Active committee members | 6                     |
| Modifying Governance     | Modifying this document                                                                                                                                                                                                                             | 2/3 majority  | Active committee members | 6                     |
