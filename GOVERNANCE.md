# Telco Global API Alliance Community Organization Guidelines (Governance Structure)

This document describes the rules and governance of the project. It is meant to be followed by all the contributors and developers of the project and the Telco Global API community. Common terminology used in this governance document is defined below:

- **The Telco Global API Project:** The sum of all activities and sub-projects performed under the governance protocol defined in this document.
- **Team members:** Members of the private Telco Global API Project GitHub Repository named in the file [Participants](./PARTICIPANTS.MD).
- **Maintainers:** Leaders of an individual sub-project or part thereof (MAINTAINERS.MD of the respective sub-project).
- **Sub-projects:** A single sub directory in the Telco Global API Project led by a voluntary group, open to anyone to participate.

Telco Global API Project is an independent open-source project, not controlled by any single company or organization. To emphasize this and clarify the governance structure (community organization guidelines), the Telco Global API Project will be conducted in the [Cloud Native Computing Foundation](https://www.cncf.io/), which all contributors are members of.

For specific guidance on the practical steps for contributing to any API sub-project please see our [Contribution Guidelines](./CONTRIBUTING.md).

## Principles

The Telco Global API community adheres to the following principles:

- Open: Telco Global API Project is open source.
- Welcoming and respectful: As a CNCF member project, we abide by the CNCF [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
- Transparent and accessible: Changes to the Telco Global API Project organization, Telco Global API Project code repositories, and CNCF related activities (e.g. level, involvement, etc.) are done in public. A primary reason that the Telco Global API Project exists is as a forum for collaboration. The work in the project should be done in the open. Community members and contributors must communicate in the open, ensure other community members and contributors can find notes of meetings, discussions, designs, and decisions, and periodically communicate a high-level summary of their contribution work to the community. Exception to this is committee work, this may be done in private if discretion is necessary.
- Merit: Ideas and contributions are accepted according to their technical merit and alignment with project objectives, scope, and design principles.

## Telco Global API Project

A global partnership could address much of the challenges in scaling API services across heterogenous operator architectures.

The development of open, global, and interoperable API solutions could benefit customers and developer ecosystems by giving access to operator capabilities in whatever network customers are in and therefore allow applications to run consistently between telco networks and countries. A new form of collaboration between various players (telcos, ISVs, device manufacturers, hyperscalers, etc.) could address much of the challenges in scaling API services across heterogenous operator architectures as well as advance the connectivity industry towards a more robust and faster core network, encourage the faster adoption of capabilities and as a result create value for the entire tech industry.

* Accelerate technology development
    * Build sustainable ecosystems around collaborative projects across industries.
    * Drive industry alignment by facilitating industry discussions with telcos, ISVs, device manufacturers, hyperscalers, etc.
* Standardization of APIs
    * Standardize and convert APIs to a user understandable format called “Service APIs”.
    * Achieve standardization through working code vs. documents.
    * Implementation experience should guide standardization process.
    * Enable interoperability (e.g. effortless portability of applications between different operators), compatibility (applicability to different network technologies) and interconnectivity (to enable interoperator collaboration).
* Education and promotion
    * Actively promote Service APIs via various forums, events, conferences, training programs, ecosystems and social media.
    * Promote best practices by aggregating and publishing lessons learned.
* Accelerate commercial adoption
    * Create awareness around use cases and services.
    * Minimize implementation effort though easy-to-consume standard Service APIs.
    * Foster the development of distribution channels to increase customer reach.
    * Integrate the APIs in relevant developer’s environments and ecosystems.
    * Provide customer service and support.

APIs grouped by services and bundled up into “Service APIs” could reduce the complexity of accessing operator capabilities for developers and enterprises.
Telco Global API Project is an independent open-source project and not controlled by any single company.

## Governance

**Steering Committee**

The highest deciding committee is the Steering Committee of the Telco Global API Project. It consists of _Tbd_.

**Committees**

Some topics, such as Security or Code of Conduct, require discretion. Whereas sub-projects are led by voluntary groups which operate in the open and anyone can join, Committees do not have open membership and do not always operate in the open. The steering committee can form committees as needed, for a bounded or unbounded duration. Membership of a committee is decided by the steering committee, however, all committee members must be community members of the Telco Global API Project. A committee has a charter and a chair, and will report to the steering committee periodically, and to the community as defined by the committee’s charter.

## Project Structure

**Sub-projects**

The Telco Global API Project is organized primarily into sub-projects. Each sub-project is comprised of members from multiple companies and organizations, with a common purpose of advancing the project with respect to a specific Service API topic, for example ‘streaming’ or ‘localization’. Our goal is to enable distributed decision making and code ownership. This will be done by providing focused forums for getting work done, making decisions, and onboarding new contributors.

Areas covered by sub-projects may be vertically focused on particular Service API components or functions, cross-cutting/horizontal or spanning many/all functional areas of Service APIs. Some examples of each type are:

- Vertical: Quality on Demand, Localization, Identification
- Horizontal: Scalability, Architecture, Lifecycle, Service

Sub-projects are documented in the respective sub directory of the APIs directory.

Each sub-project must have a MAINTAINERS.md file. A sub-project should have at least one maintainer. Ideally a sub-project is managed by two or more maintainers, depending on the size and scope of the sub-project. Here, the responsibilities must be clearly agreed upon between all of the maintainers. This includes coordinating who is responsible for which issues and pull requests. Each maintainer should also be listed in the [Participants](./PARTICIPANTS.MD) file in the root directory.

Some sub-projects may have distinct (although sometimes overlapping) sets of contributors and maintainers, who act as the sub-project’s technical leaders, organizers and facilitators.

Where a sub-project has a release process, access and documentation should be such that more than one person can perform a release. Releases should be announced on the Telco Global API Project mailing list. Any new sub-projects should be first proposed on Telco Global API Project mailing list following the voting procedures listed below.

**Working Groups**

Community rallying points are used to facilitate discussions/work regarding topics that are short-lived or that span multiple sub-projects.

Working groups are primarily used to facilitate topics of discussion that are in scope for the Telco Global API Project but that cross sub-project lines. If a subset of community members wants to get together and discuss a topic, they can do so with forming a Working Group.

See “working group governance” _Tbd_ for more details about forming and disbanding Working Groups.

Working groups are documented in _Tbd_.

## Roles, Responsibilities and Requirements

**Team members**

Team member status may be given to those who have made ongoing contributions to the Telco Global API Project for at least 3 months. This is usually in the form of code submissions and improvements and/or notable work on documentation but may also include other contributions such as organizing events or user support.

The current team members are listed in PARTICITPANTS.MD.

Please note that Telco Global API had received significant contributions from a number of unlisted individuals before this governance document was written, and thus formal team membership, was created.

**Maintainers**

Maintainers are first and foremost contributors that have shown they are committed to the long-term success of a sub-project. Contributors wanting to become maintainers are expected to be deeply involved in contributing code, pull request review, and triaging issues in the project for a minimum of three months and perform an ongoing contribution.

Requirements

The following requirements must be met by an individual wishing to become a maintainer for a sub-project: 

- Deep understanding of the technical goals and direction of the sub-project
- Deep understanding of the technical domain of the sub-project
- Sustained contributions to the design and direction of the sub-project, demonstrated by performing all of the following:
  - Authoring and reviewing proposals
  - Initiating, contributing and resolving discussions (emails, GitHub issues, meetings)
  - Identifying subtle or complex issues in designs and implementation PRs
- Direct contributions to the subproject through implementation and / or review

Responsibilities

Maintainers lead one or more sub-project(s) or parts thereof and serve as a point of conflict resolution amongst the contributors and are the technical authority for a subproject (responsible for vision and direction and overall design, choose/approve change proposal (KEP) approvers, field technical escalations, etc.). They *MUST* have demonstrated both good judgement and responsibility towards the health of that sub-project. Sub-project Maintainers *MUST* set technical direction and make or approve design decisions for their sub-project - either directly, or through delegation of these responsibilities.

Maintainers are also intended to be organizers and facilitators, responsible for the continued operation and progress of the sub-project and for communication and co-ordination with the other sub-projects, the Steering Committee, and the broader community. Maintainers are granted commit rights to their sub-projects.

Defined by: entry in sub-project MAINTAINERS.MD file.

Maintainers should actively participate in Pull Request reviews and are expected to respond to assigned Pull Requests in a *reasonable* time frame, either providing insights, or assign the Pull Requests to other maintainers.

The following responsibilities must be met by the maintainer for a sub-project:

- Make and approve technical design decisions for the sub-project.
- Set the technical direction and priorities for the sub-project.
- Define milestones and releases.
- Mentor and guide approvers, reviewers, and contributors to the sub-project.
- Ensure continued health of sub-project
  - Adequate test coverage to confidently release
  - Tests are passing reliably (i.e. not flaky) and are fixed when they fail
- Ensure a healthy process for discussion and decision making is in place and is followed by the sub-project’s members.
- Work with other sub-project owners to maintain the project's overall health and success holistically.

Types of maintainers

There are different types of maintainers (Reviewers and Committers) with different responsibilities, but all maintainers have 3 things in common:

1. They share responsibility in the project's success.
1. They have made a long-term, recurring time investment to improve the project.
1. They spend that time doing whatever needs to be done, not necessarily what is the most interesting or fun.

Reviewers

- A reviewer is a maintainer within the project. They share in reviewing issues and pull requests and their LGTM counts towards the required LGTM count to merge a code change into the project.
- Reviewers are part of the organization but do not have write access. Becoming a reviewer is a core aspect in the journey to becoming a committer.

Committers

- A committer is a core maintainer who is responsible for the overall quality and stewardship of the project. They share the same reviewing responsibilities as reviewers but are also responsible for upholding the project bylaws as well as participating in project level votes.
- Committers are part of the organization with write access to all repositories. Committers are expected to remain actively involved in the project and participate in voting and discussing of proposed project level changes.

**Security Advisors**

- A security advisor is an advisory role in the project responsible for helping classify and advise on embargoed security disclosures. Security advisors are part of the organization without write access, but with read access to security disclosures and advisories before becoming public. Security advisors help maintain the integrity of the security review process and encourage responsible disclosure.
- Security advisors are individuals trusted by maintainers and representing significant users of the project. A reviewer may also be a security advisor, however, committers do not need this role as it is part of their regular duties. The security advisor duties are not part of the duties of being a reviewer. There is no expectation of advisors to become reviewers or participate in issue triage and code review.

## Decision Making

**Voting Principles**

The Telco Global API project usually runs by informal consensus, however sometimes a formal decision must be made (reasons for this see below).

Depending on the subject matter, different methods of voting are used as laid out below.

For all votes, voting must be open for at least one week. The end date should be clearly stated in the call to vote. A vote may be called and closed early if enough votes have come in one way so that further votes cannot change the final decision.

In all cases, all and only team members are eligible to vote, with the sole exception of the forced removal of a team member, in which said member is not eligible to vote.

Discussion and votes on personnel matters (including but not limited to team membership and maintainership) are held in private. All other discussion and votes are held in public on the Telco Global API Project mailing list.

For public discussions, anyone interested is encouraged to participate. Formal power to object or vote is limited to team members.

**Consensus**

The default decision making mechanism for the Telco Global API Project is [lazy consensus](https://couchdb.apache.org/bylaws.html#lazy). This means that any decision on technical issues is considered supported by the team as long as nobody objects based on substantiated technical grounds.

Silence on any consensus decision is implicit agreement and equivalent to explicit agreement. Explicit agreement may be stated at will. Decisions may, but do not need to be called out and put up for decision on the Telco Global API Project mailing list at any time and by anyone.

Consensus decisions can never override or go against the spirit of an earlier explicit vote.

If any team member raises objections, the team members work together towards a solution that all involved can accept. This solution is again subject to lazy consensus.

In case no consensus can be found, but a decision one way or the other must be made, any team member may call a formal majority vote.

**Majority vote**

Majority votes must be called explicitly in a separate thread on the appropriate mailing list. The subject must be prefixed with [VOTE]. In the body, the call to vote must state the proposal being voted on. It should reference any discussion leading up to this point.

Votes may take the form of a single proposal, with the option to vote yes or no, or the form of multiple alternatives.

A vote on a single proposal is considered successful if more vote in favor than against.

If there are multiple alternatives, members may vote for one or more alternatives, or vote “no” to object to all alternatives. It is not possible to cast an “abstain” vote. A vote on multiple alternatives is considered decided in favor of one alternative if it has received the most votes in favor, and a vote from more than half of those voting. Should no alternative reach this quorum, another vote on a reduced number of options may be called separately.

**Supermajority vote**

Supermajority votes must be called explicitly in a separate thread on the appropriate mailing list. The subject must be prefixed with [VOTE]. In the body, the call to vote must state the proposal being voted on. It should reference any discussion leading up to this point.

Votes may take the form of a single proposal, with the option to vote yes or no, or the form of multiple alternatives.

A vote on a single proposal is considered successful if at least two thirds of those eligible to vote vote in favor.

If there are multiple alternatives, members may vote for one or more alternative, or vote “no” to object to all alternatives. A vote on multiple alternatives is considered decided in favor of one alternative if it has received the most votes in favor, and a vote from at least two thirds of those eligible to vote. Should no alternative reach this quorum, another vote on a reduced number of options may be called separately.

**Technical decisions**

Technical decisions that only affect a single sub-project are made informally by the maintainer of this sub-project, and [lazy consensus ](https://couchdb.apache.org/bylaws.html#lazy)is assumed. Technical decisions that span multiple parts of the Telco Global API Project should be discussed and made on the Telco Global API Project mailing list.

Decisions are usually made by [lazy consensus](https://couchdb.apache.org/bylaws.html#lazy). If no consensus can be reached, the matter may be resolved by majority vote.

**Decisions about Team Members**

New members may be proposed by any existing member by email to Telco Global API Project team. It is highly desirable to reach consensus about acceptance of a new member. However, the proposal is ultimately voted on by a formal supermajority vote.

If the new member proposal is accepted, the proposed team member should be contacted privately via email to confirm or deny their acceptance of team membership. This email will also be CC'd to Telco Global API Project team for record-keeping purposes.

If they choose to accept, the onboarding procedure is followed.

Team members may retire at any time by emailing the team.

Team members can be removed by supermajority vote on the team mailing list. For this vote, the member in question is not eligible to vote and does not count towards the quorum. Any removal vote can cover only one single person.

Upon death of a member, they leave the team automatically.

In case a member leaves, the offboarding procedure is applied.

**Changes in Governance**

Changes in project governance (GOVERNANCE.md) could be initiated by opening a github PR. The PR should only be opened no earlier than 6 weeks before the end of the project lead's term. The PR should be kept open for no less than 4 weeks. The PR can only be merged follow the same voting process as in Changes in Maintainership.

**Editorial changes**

Editorial changes are changes which fix spelling or grammar, update work affiliation, or similar; they update style or reflect an outside and obvious reality. They do not change the intention or meaning of anything in this document. They must be made via PR and accepted via [lazy consensus](https://couchdb.apache.org/bylaws.html#lazy).

**Changes in Maintainership**

Changes in maintainership have to be announced on the Telco Global API Project mailing list. They are decided by [lazy consensus ](https://couchdb.apache.org/bylaws.html#lazy)and formalized by changing the MAINTAINERS.md file of the respective sub project.

A maintainer or committer may resign by notifying the team mailing list. A maintainer with no project activity for a year is considered to have resigned. Maintainers that wish to resign are encouraged to propose another team member to take over the project.

**Other matters**

Any matter that needs a decision, including but not limited to financial matters, may be called to a vote by any member if they deem it necessary. For financial, private, or personnel matters, discussion and voting takes place on the team mailing list.

## On- / Offboarding

The On- / Offboarding section is informational and can be changed by [lazy consensus ](https://couchdb.apache.org/bylaws.html#lazy)unless challenged. If no consensus can be reached, the matter may be resolved by majority vote.

**Onboarding**

The new member is

- added to the list of team members (PARTICIPANTS.MD). Ideally by sending a PR of their own, at least approving said PR.
- announced on the Telco Global API Project mailing list by an existing team member. Ideally, the new member replies in this thread, acknowledging team membership.
- added to group accounts where applicable. Services with some variety of a group account include but are not restricted to Digital Ocean, DockerHub, GSuite, Netlify, Twitter (via Tweetdeck), Youtube.
- optionally added to the list of contributors.
- added to the team mailing list.

**Offboarding**

The ex-member is

- removed from the list of team members (PARTICIPANTS.MD). Ideally by sending a PR of their own, at least approving said PR. In case of forced removal, no approval is needed.
- removed from the team mailing list , all lists of maintainers and the list of contributors.
- removed from group accounts where applicable. Services with some variety of a group account include but are not restricted to Digital Ocean, DockerHub, GSuite, Netlify, Twitter (via Tweetdeck), Youtube.
- not allowed to call themselves an active team member anymore, nor allowed to imply this to be the case.
- added to a list of previous members if they so choose.

If needed, we reserve the right to publicly announce removal.

## Stepping down policy

Life priorities, interests, and passions can change. If you're a maintainer but feel you must remove yourself from the list, inform other maintainers that you intend to step down, and if possible, help find someone to pick up your work. At the very least, ensure your work can be continued where you left off.

After you've informed other maintainers, create a pull request to remove yourself from the MAINTAINERS file.

## Licensing
- Apache 2.0 license for API source codes
- CC-BY-4.0 license for documentation

## FAQ

**How do I propose a decision?**

Send an email to the Telco Global API Project mailing list with your motion. If there is no objection within a reasonable amount of time, consider the decision made. If there are objections and no consensus can be found, a vote may be called by a team member.

**How do I become a team member?**

To become an official team member, you should intend to make ongoing contributions to one or more project(s) for at least three months. At that point, a team member (typically a maintainer of the project) may propose you for membership. The discussion about this will be held in private, and you will be informed privately when a decision has been made. A possible, but not required, graduation path is to become a maintainer later.

Should the decision be in favor, your new membership will also be announced on the Telco Global API Project mailing list.

**How do I add a sub project?**

As a team member, propose the new sub project on the Telco Global API Project mailing list. If nobody objects, create the sub project in the GitHub repository. Add at least a README.md explaining the goal of the project, and a MAINTAINERS.md with the maintainers of the project (at this point, this probably means you).

**How do I archive or remove a sub project?**

All sub projects should be kept and not removed.

**How do I remove an inactive maintainer?**

A maintainer may resign by notifying the team mailing list. A maintainer with no project activity for a year will be treated as if they had resigned. If there is an urgent need to replace a maintainer, discuss this on the team mailing list.

**How do I remove a team member?**

Team members may resign by notifying the team mailing list. If you think a team member should be removed against their will, propose this to the team mailing list. Discussions will be held there in private.
