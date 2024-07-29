# Project Structure and Roles

## Project Structure

**Sub Projects**

The CAMARA Project is organized primarily into Sub Projects. Each Sub Project is composed of Project participants from multiple companies and organizations, with a common purpose of advancing the Sub Project with respect to a specific Service API topic, for example ‘quality on demand’ or ‘localization’. Our goal is to enable distributed decision making and code ownership. This will be done by providing focused forums for getting work done, making decisions, and onboarding new Contributors.

Each Sub Project is documented with a home page on [wiki.camaraproject.org](https://wiki.camaraproject.org), one or multiple repositories for the API definition and the API documentation (API Repositories), and optionally in additional repositories for provider implementations with API code of the transformation function Northbound --> Southbound (Provider Implementation Repositories).

The wiki home page of a Sub Project should contain at least a description of the scope of the Sub Project, links to the API Repositories which are belonging to the Sub Project, the address of the mailing list on [lists.camaraproject.org](https://lists.camaraproject.org/groups), and the schedule and registation/join link of the regular meeting of the Sub Project. Sub pages should contain the meeting minutes, (informal) supporting documents and (if applicable) release information for the API members as defined by the Release Management working group.

The purpose of an API Repository is the definition and documentation of one or multiple (very closely related) APIs which will be always released together. Each API Repository must have a README.MD file (with a description of the API scope and a link to the Sub Project home page), a CODEOWNERS and a MAINTAINERS.MD file. An API Repository should have at least one Maintainer. Ideally a Sub Project is managed by two or more Maintainers, depending on the size and scope of the API. Here, the responsibilities must be clearly agreed upon between all of the Maintainers. This includes coordinating who is responsible for which issues and pull requests. 
The Contributors to an API Repository are recorded by the mechanisms of GitHub in the Sub Project’s repositories. Each Contributor, Codeowner and Maintainer should also be listed in the [PARTICIPANTS.MD](./PARTICIPANTS.MD) file in the Governance repository root directory. Each API Repository should have a license file, a GOVERNANCE.MD file (pointing to the Governance repository) and subdirectories /documentation/API_documentation, /documentation/SupportingDocuments and /code/API_definitions. Only Codeowners should have write permissions to an API Repository.

A Sub Project should have at least one Maintainer. Ideally a Sub Project is managed by two or more Maintainers, depending on the size and scope of the Sub Project. The Maintainers of a Sub Project are defined by the union of the Maintainers listed within the MAINTAINERS.md files of the API Repositories which are belonging to the Sub Project. It is recommended that there is an overlap between the Maintainers of the API Repositories of the Sub Project, but it is not mandated that all Maintainers of the Sub Project take responsibility for all APIs in the Sub Project.
  
A Provider Implementation Repository only must have a CODEOWNERS file, a license file, a GOVERNANCE.MD file (pointing to the Governance repository) and a subdirectory /code/API_code with API code of the transformation function Northbound --> Southbound. Only Codeowners should have write permissions to a Provider Implementation (PI) Repository. Provider Implementation Repositories have the same name as the API Repository but with suffix _-PI§x§_.

Where a Sub Project has a release process, access and documentation should be such that more than one person can perform a release.

**Working Groups**

Working Groups are primarily used to facilitate topics of discussion that are in scope for the CAMARA Project but that are short-lived or that span multiple Sub Projects. If a subset of Project participants wants to get together and discuss a topic, they can do so by forming a Working Group. The Technical Steering Committee (TSC) decides upon implementing or removing Working Groups.

Working Groups are documented in a separate section of [wiki.camaraproject.org](https://wiki.camaraproject.org) and can have one or multiple GitHub repositories following the API Repository template (the rules for API Repositories apply). In the Readme.md file the repositories of Working Groups are marked with a "Working Group" badge.

**Repositories**

As mentioned before the contributions to the Sub Projects were documented in the respective GitHub repositories of the Sub Projects, and the contributions to Working Groups were documented in the GitHub repositories of the Working Groups. All contributions beyond that, esp. contributions to the Project itself or the TSC are documented in the GitHub repository “Governance”. Additional repositories can be created for project administration purposes. 

For ease of use there are templates for the two types of Sub Project repositories (API and Provider Implementation Repositories), containing all necessary files which can be cloned and adapted. When cloning it has to be ensured that also the branch protection rules are active in the new repositories. For Working Group repositories the API Repository template should be used and adapted.

A repository must have at least one Codeowner. Repositories with branch protection rules must have at least two Codeowners. 

Only Markdown format shall be used as the document standard for documents in the main branch of Sub Project and Working Group repositories. The only exceptions are supporting documents, for which other formats like PDF or PPT are allowed. Note: Documents which are meant as base for discussion or to explain change requests are best attached to an issue. Informal supporting documents are best located within the Sub Project or Working Group wiki.

**Mailing list**

A Project mailing list is established, each Project participant documented in [PARTICIPANTS.MD](./PARTICIPANTS.MD) is added. A message to all Project participants can be sent using <all@lists.camaraproject.org>.

## Changes and contributions to CAMARA ##

In the Project the “Fork and pull model” is used. Changes and contributions to CAMARA shall follow this process:
![PR_Approval_Process](/documentation/images/PR_Approval_Process.png)

1 All changes / contributions shall start with an issue to which initial documents, API definitions or code can be attached. The issue should be discussed in the Sub Project community before working out the best form of action. By means of the issue the traceability of the contributions to CAMARA is also ensured. In addition as general rule there shall be no (later) pull request without a reference to an issue (except minor corrections, to be labeled as “minor”).

2 Either the issue creator or one of the Sub Project Maintainers then shall assign the issue to one of the Contributors of the Sub Project.

3 This Contributor shall create a fork (if necessary), shall create a new branch, and shall copy the branch link into the issue. For the naming of the branch a clear and concrete description shall be used.

Now they can work on the solution and add commits to the branch. If they are done with the work the Contributor shall create a pull request, refer to the addressed issue(s) in the pull request description (and vice versa) and add the commits to the pull request. For the naming of the pull request a clear and concrete description shall be used.

4 The Contributor now shall invite other Sub Project Contributors to review the pull request. The Contributor shall invite at least 2 Maintainers, ideally from different companies and all Codeowners of the repository. As default all Maintainers and all Codeowners of the repository shall be invited as reviewers. Only the initial Contributor should edit a pull request in review (the Contributor is responsible to react on comments) or allow other Contributors explicitly to commit into the pull request.

5 The pull request shall be approved by all Contributors included in the review within a 2 weeks period. If a Contributor doesn't perform a review within that time frame the Contributor automatically accepts the pull request. For conflicting cases rules will be defined later. A two days cool off period after the approval shall be kept. A pull request review in certain cases might lead to a pull request not being approved. In this case, the Codeowner shall close the pull request (and the branch, and the issue) with the appropriate comments and the contribution shall not get merged into the main branch.

6 Finally one of the Codeowners of the repository shall merge the pull request into the main branch. By that the Codeowner closes the pull request. The Codeowner also shall close the branch and the issue (if not already automatically done).
Deliverables of the Sub Project are all artifacts in the main branch of its repositories.

More details can be found in the [CONTRIBUTING.MD](https://github.com/camaraproject/Governance/blob/main/CONTRIBUTING.md).

## Working Groups ##

**API Backlog**

The API Backlog Working Group is supervised by the TSC. The responsibility of the Working Group is to coordinate and prepare all the material needed to evaluate a proposal for a new Sub Project (consisting of one or more related APIs), or scope change of an existing Sub Project (including adding additional APIs to that Sub Project). The prepared material will be evaluated by TSC to decide if a new Sub Project should be onboarded in CAMARA.

The API onboarding and management in CAMARA is described in [API-onboarding.md](./documentation/API-onboarding.md).

**Commonalities**

CAMARA commonalities shall be processed in a Working Group “Commonalities”. The Working Group “Commonalities” works under the supervision of the TSC. The scope of the Working Group is to create guidelines, best practices and concept documents relevant for all APIs in CAMARA. The commonalities Working Group shall work e.g. on the development of a common meta model that shall be used as a reference across the Sub Projects. It is open for members of any Sub Project or Working Group to raise issues in the Technical Steering Committee (TSC) for relevant topics on a need basis.

All Sub Projects must comply with the work in the commonalities Working Group.

**Marketing**

The Marketing Working Group is responsible to plan and perform marketing activities for CAMARA and to maintain marketing material (onepager, presentation, website, GitHub, ...). It is supervised by the Board of the CAMARA Fund.

**Release management**

Each Sub Project shall have a release management. The release cadence shall be determined by the TSC and on a regularly published schedule. Milestones shall be set up within each Sub Project to ensure the ability of each Sub Project to meet the release schedule as defined by the TSC.

Goal is that all Sub Projects updated are released at the same release milestone so that the implementors of the APIs become accustomed to the regular release cadence.

The Release Management working group is supervised by the TSC. The scope of the Working Group is the definition of guidelines and best practices for the API Versioning and release management within the Sub Projects and the support of the TSC in its responsibilities for Release Management.


## Roles, Responsibilities and Requirements

**Project participants**

Project participant (= contributor) status may be given to those who intend to make ongoing contributions to the CAMARA Project. This is usually in the form of code submissions and improvements and/or notable work on documentation but may also include other contributions such as organizing events or user support.

The current Project participants are listed in [PARTICIPANTS.MD](./PARTICIPANTS.MD).

Please note that the CAMARA Project had received significant contributions from a number of unlisted individuals before this governance document was written, and thus formal team membership was created.

To be listed in [PARTICIPANTS.MD](./PARTICIPANTS.MD) is prerequisite for getting any other role in the Project. Also any other role within the Project has to be returned before deleting the name in [PARTICIPANTS.MD](./PARTICIPANTS.MD).

**Changes in Project participation**

A new Project participant can get Project participation by sending a message to <all+subscribe@lists.camaraproject.org>. Changes in Project participantship have to be announced on the CAMARA Project mailing list by the new participant. They are decided  by [lazy consensus ](https://couchdb.apache.org/bylaws.html#lazy).

A Project participant may resign by notifying the team mailing list and by sending a message to <all+unsubscribe@lists.camaraproject.org>. A Project participant with no project activity for a year is considered to have resigned. Project participants that wish to resign are encouraged to propose another Project participant to take over their project work.

**Working Group participants**

Each Project participant can be part of one or more of the Working Groups of the Project by subscribing to the mailing list(s). By that the Project participant gets the role Working Group participant.

A Working Group participant may resign by unsubscribing from the mailing list(s).

**Contributors**

Each Project participant can contribute to the Sub Projects and Working Groups of the Project. Contributors to a Sub Project can contribute by creating pull requests within the API Repositories. To become or resign as Contributor please subscribe / unsubscribe to the mailing list of the Sub Project. The list of Contributors of a specific Sub Project is maintained by the administrators of the Project using GitHub functionality.

**Codeowners**

Codeowners can merge code and accept pull requests. A Codeowner is responsible for the overall quality and stewardship of the Sub Project. Contributors can get a Codeowner role if they are Contributors and deeply involved in contributing code, pull request review, and triaging issues in the Sub Project for a minimum of three months and perform an ongoing contribution. Codeowners are decided by the Maintainers and formalized by changing the CODEOWNERS file. Changes in code ownership have to be announced on the mailing list of the Sub Project.

**Maintainers**

Maintainers are the leaders of a Sub Project. Maintainers are first and foremost contributors that have shown they are committed to the long-term success of a Sub Project. Contributors wanting to become Maintainers are expected to be deeply involved in contributing code, pull request review, and triaging issues in a repository of a Sub Project or Working Group for a minimum of three months and perform an ongoing contribution.

**Changes in maintainership**

When creating a new Sub Project the TSC also nominates the initial Maintainers for the repository/ies of the new Sub Project. After that the Maintainers of a Sub Project decide upon the maintainership.

The merge of two Sub Projects or the move of an API Repository from one Sub Project to another Sub Project need the consensus of the the Maintainers of both involved Sub Projects. The resulting Maintainer team(s) of the Sub Project(s) are again defined as the union of the Maintainers of the API Repositories of the Sub Project(s) (see above). 

Changes in maintainership have to be announced on the mailing list of the Sub Project. They are decided  by [lazy consensus ](https://couchdb.apache.org/bylaws.html#lazy) by all Maintainers of a Sub Project and formalized by changing the MAINTAINERS.MD file of the respective Sub Project.

A Maintainer may resign from the maintainership of one or multiple API Repositories by notifying the Sub Project mailing list. A Maintainer with no Project activity for a year is considered to have resigned. Maintainers that wish to resign are encouraged to propose another Project participant to take over their Project work.

**Maintainer requirements**

The following requirements must be met by an individual wishing to become a Maintainer for a Sub Project: 

- Deep understanding of the technical goals and direction of the Sub Project
- Deep understanding of the technical domain of the Sub Project
- Sustained contributions to the design and direction of the Sub Project, demonstrated by performing all of the following:
  - Authoring and reviewing proposals
  - Initiating, contributing and resolving discussions (emails, GitHub issues, meetings)
  - Identifying subtle or complex issues in designs and implementation pull requests
- Direct contributions to the Sub Project through implementation and / or review

**Maintainer responsibilities**

Maintainers lead one or more Sub Project(s) or parts thereof and serve as a point of conflict resolution amongst the Contributors and are the technical authority for a Sub Project (responsible for vision and direction and overall design, choose/approve change proposals, field technical escalations, etc.). They *MUST* have demonstrated both good judgment and responsibility towards the health of that Sub Project. Sub Project Maintainers *MUST* set technical direction and make or approve design decisions for their Sub Project - either directly, or through delegation of these responsibilities.

Maintainers are also intended to be organizers and facilitators, responsible for the continued operation and progress of the Sub Project and for communication and co-ordination with the other Sub Projects, the TSC, and the Project participants. 

Maintainers should actively participate in pull request reviews and are expected to respond to assigned pull requests in a reasonable time frame, either providing insights, or assign the pull requests to other Maintainers.

The following responsibilities must be met by the Maintainer for a Sub Project:

- Make and approve technical design decisions for the Sub Project.
- Set the technical direction and priorities for the Sub Project.
- Define milestones and releases.
- Mentor and guide Contributors and Codeowners to the Sub Project.
- Ensure continued health of Sub Project
  - Adequate test coverage to confidently release
  - Tests are passing reliably (i.e. not flaky) and are fixed when they fail
- Ensure a healthy process for discussion and decision making is in place and is followed by the Sub Project's Contributors.
- Work with other Sub Project owners to maintain the Project's overall health and success holistically.
