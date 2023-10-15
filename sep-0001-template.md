---
SEP: 1
Title: SocialDB Enhancement Proposal Purpose and Guidelines
Authors: Charles G. <charles@near.org>
Status: Pending
DiscussionsTo: https://github.com/nearsocial/SEPs/pull/1
Version: 1.0.0
Created: 2023-10-10
Last Updated: 2023-10-10
---


## Summary

A SocialDB Enhancement Proposal (SEP) is a design document that specifies a request to evolve the Near socialDB standard accompanied by an end-to-end prototype which demonstrates the use of the proposed enhancement.

SEPs are the primary mechanism for evolving NearSocial DB standards in a community-driven way. SEPs provide a concise technical specification, a rationale for the feature, and a prototype implementation. The SEP author is responsible for building consensus within the community and documenting dissenting opinions. The typical primary audience for SEPs are the developers of Near 2.0 Gateways and decentralized application developers.

SEPs are stored as text files in a versioned repository, allowing for easy historical tracking. A list of SEPs is available on [GitHub](https://github.com/nearsocial/SEPs).

## Motivation

The purpose of the SEP process is to ensure a coordinated evolution of the NEARSocial standards and to empower the community to contribute to its development. Given the complexity and number of participants involved across the ecosystem, a well-defined process helps ensure transparency, security, and stability.


## Submit a NEP

### Start with ideation

Everyone in the community is welcome to propose, discuss, and review ideas to improve the NEAR SocialDB standards. The SEP process begins with a [new idea](https://www.neardevgov.org/blog/how-to-ideate-in-the-near-developer-governance) for the NEAR Social ecosystem. A single SEP should contain a single key proposal or new idea.

Each SEP must have an author: Someone who writes the SEP using the style and format described below. The author, or another champion, shepherds the discussions in the appropriate forums and attempts to build community consensus around the idea to help it progress toward completion.

Before submitting a SEP, the author should first attempt to ascertain whether the idea is SEP-able. Vetting an idea publicly before writing a SEP saves the potential author time. Asking the NEAR community first if the idea is original helps prevent effort on something guaranteed to be rejected based on prior discussions. It also helps ensure the idea applies to the entire community. Just because an idea sounds good to the author does not mean it will work for most people in most use cases.

In general, the process for socializing an idea is:

- **Check prior proposals:** Many ideas for changing NEAR Social come up frequently. Please search the [Dev Gov Gigs Board](https://devgovgigs.near.social), the [NEAR Forums](https://gov.near.org), and SEPs in this repo before proposing something new.
- **Share the idea:** Submit your [idea](https://www.neardevgov.org/blog/how-to-ideate-in-the-near-developer-governance) on the [Dev Gov Gigs Board](https://devgovgigs.near.social).
- **Get feedback:** The [Dev Gov Gigs Board](https://devgovgigs.near.social) has comment threading which allows the community to ideate, ask questions, wrestle with approaches, etc. If more immediate responses are desired, consider bringing the conversation to the appropriate [Community Group](https://gov.near.org/c/dev/community-groups/103).


### Submit a SEP Draft

Following the above initial discussions, the author should submit a SEP draft into the GitHub SEP repository. The draft SEP must follow the [SEP-0000 template](https://github.com/nearsocial/SEPs/blob/master/sep-0000-template.md), or else it will fail the review immediately.

To submit a SEP draft as a pull request, the SEP author should:

1. Fork the [SEPs repository](https://github.com/nearsocial/SEPs).
2. Copy `sep-0000-template.md` to `seps/sep-0000-my-feature.md` (where “my-feature” is descriptive; don’t assign a SEP number yet).
3. Fill in the SEP following the SEP template guidelines. For the Header Preamble, make sure to set the status as “Draft.”
4. Push this to your GitHub fork and submit a pull request.
5. Now that your SEP has an open pull request, use the pull request number to update your `0000` prefix. For example, if the PR is 305, the SEP should be `seps/sep-0305-my-feature.md`.
6. Push this to your GitHub fork and submit a pull request. Mention the @nearsocial/sep-moderators in the comment and turn the PR into a "Ready for Review" state once you believe the SEP is ready for review.


### NEP Stages

- **Draft:** The first formally tracked stage of a new SEP. This process begins once an author submits a draft proposal and an SEP moderator merges it into the SEP repo when properly formatted.
- **Review:** A SEP moderator marks a SEP as ready for Subject Matter Experts Review. If the SEP is not approved within two months, it is automatically rejected. During this review time, the accompanying prototype(s) should be fully implemented and made available to the reviewers, and the corresponding PR(s) into nearsocial/standards should be submitted.
- **Voting:** This is the final voting period for a SEP. The working group will vote on whether to accept or reject the SEP. This period is limited to two weeks. If during this period necessary normative changes are required, the SEP will revert to Review.

Moderator, when moving a SEP to review stage, submit a Pull Request to update the SEP's status to `Review`


### SEP Outcomes

- **Approved:** If the working group votes to approve, they will move the SEP to Approved. Once approved, Standards SEPs exist in a state of finality and should only be updated to correct errata and add non-normative clarifications.
- **Rejected:** If the working group votes to reject, they will move the SEP to Rejected.


### SEP Roles and Responsibilities

![author](https://user-images.githubusercontent.com/110252255/181816534-2f92b073-79e2-4e8d-b5b9-b10824958acd.png)
**Author**<br />
_Anyone can participate_

The SEP author is responsible for creating a SEP draft that follows the guidelines. They drive the SEP forward by actively participating in discussions and incorporating feedback. During the voting stage, they may present the SEP to the working group and community, and provide a prototype implementation with thorough testing and documentation during the review stage.

![Moderator](https://user-images.githubusercontent.com/110252255/181816650-b1610c0e-6d32-4d2a-a34e-877c702139bd.png)
**Moderator**<br />
_Assigned by the working group_

The moderator is responsible for facilitating the process and validating that the SEP follows the guidelines. They do not assess the technical feasibility or write any part of the proposal. They provide comments if revisions are necessary and ensure that all roles are working together to progress the SEP forward. They also schedule and facilitate public voting calls.

![Reviewer](https://user-images.githubusercontent.com/110252255/181816664-a9485ea6-e774-4999-b11d-dc8be6b08f87.png)
**SEP Reviewer** (Subject Matter Experts)<br />
_Assigned by the working group_

The reviewer is responsible for reviewing the technical feasibility of a SEP and giving feedback to the author. While they do not have voting power, they play a critical role in providing their voting recommendations along with a summary of the benefits and concerns that were raised in the discussion. Their inputs help everyone involved make a transparent and informed decision.

![Approver](https://user-images.githubusercontent.com/110252255/181816752-521dd147-f56f-4c5c-84de-567b109f21d6.png)
**Approver** (Working Groups)<br />
_Selected by the Dev Gov DAO in the bootstrapping phase_

The working group is a selected committee of 3-7 recognized experts who are responsible for coordinating the public review and making decisions on a SEP in a fair and timely manner. There are multiple working groups, each one focusing on a specific ecosystem area, such as the [Near Social](https://gov.near.org/t/near-social-community-group/31179) or Wallet Standards communitites. They assign reviewers to proposals, provide feedback to the author, and attend public calls to vote to approve or reject the SEP. Learn more about the various working groups at [neardevgov.org](http://neardevgov.org/).


## SEP Maintenance

Generally, SEPs are not modifiable after reaching their final state. However, there are occasions when updating a SEP is necessary, such as when discovering a security vulnerability or identifying misalignment with a widely-used implementation. In such cases, an author may submit a SEP extension in a pull request with the proposed changes to an existing SEP document.

A SEP extension has a higher chance of approval if it introduces clear benefits to existing implementors and does not introduce breaking changes.

If an author believes that a new extension meets the criteria for its own separate SEP, it is better to submit a new SEP than to modify an existing one. Just make sure to specify any dependencies on certain NEPs.


## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
