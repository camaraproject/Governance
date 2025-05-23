# Project Structure and Roles

## Project Structure

**Overview**

The work of CAMARA is organized in 
* Sub Projects and their API Repositories
* Working Groups and their Repositories

API Repositories in CAMARA are classified with one of three stages of maturity:

* Sandbox
* Incubating
* Graduated

Sandbox API Repositories can initially exist independent of a Sub Project. The process for the creation of new Sandbox repositories, the transition to Incubating and Graduated API Repositories, and (potential) archiving of API Repositories is described within the [API Onboarding and Lifecycle documentation](./API-Onboarding-and-Lifecycle.md).

**Sub Projects**

Sub Projects are the primary structure of the CAMARA Project. Each Sub Project is composed of Project participants from multiple companies and organizations, with a common purpose of advancing the Sub Project with respect to a specific Service API topic, for example ‘quality on demand’ or ‘localization’. Our goal is to enable distributed decision making and code ownership. This will be done by providing focused forums for getting work done, making decisions, and onboarding new Contributors.

Each Sub Project has a home page on the [CAMARA wiki](https://lf-camaraproject.atlassian.net/), one or multiple repositories for the API definition and the API documentation (API Repositories), and optionally additional repositories for provider implementations with API code of the transformation function Northbound --> Southbound (Provider Implementation Repositories).

The wiki home page of a Sub Project should contain at least a description of the scope of the Sub Project, links to the API Repositories which are belonging to the Sub Project, the address of the mailing list on [lists.camaraproject.org](https://lists.camaraproject.org/groups), and the schedule and registration/join link of the regular meeting of the Sub Project. Sub pages should contain the meeting minutes, (informal) supporting documents and (if applicable) release information for the API Repositories of the Sub Projects as defined by the Release Management working group.

A Sub Project should have at least three Maintainers. The Maintainers of a Sub Project are defined by the union of the Maintainers listed within the MAINTAINERS.md files of the API Repositories which are belonging to the Sub Project. It is recommended that there is an overlap between the Maintainers of the API Repositories of the Sub Project, but it is not mandated that all Maintainers of the Sub Project take responsibility for all API Repositories in the Sub Project.

**API Repositories**

The purpose of an API Repository is the definition and documentation of one or multiple (very closely related) APIs which will be always released together.

The following API Repositories rules shall apply for all (independent) Sandbox, Incubating, and Graduated API repositories.

A repository must have at least one Codeowner. Repositories with branch protection rules must have at least two Codeowners. Only Codeowners should have write permissions to an API Repository. For requirements regarding the Maintainers see the definition of Sandbox, Incubating and Graduated API Repositories.

Each API Repository must have a README.MD file (with a description of the API scope), a license file, a GOVERNANCE.MD file (pointing to the Governance repository), a CODEOWNERS, and a MAINTAINERS.MD file.

Each API Repository should have subdirectories /documentation/API_documentation, /documentation/SupportingDocuments, /code/API_definitions, and /code/Test_definitions. 
  
API Repositories can have in addition Provider Implementation (PI) Repositories on their side. Provider Implementation Repositories only must have a CODEOWNERS file, a license file, a GOVERNANCE.MD file (pointing to the Governance repository) and a subdirectory /code/API_code with API code of the transformation function Northbound --> Southbound. Only Codeowners should have write permissions to a Provider Implementation (PI) Repository. Provider Implementation Repositories have the same name as the API Repository but with suffix _-PI§x§_.

**Sandbox API Repositories**

A Sandbox API Repository is meant for the rapid development of a new API proposal through one or multiple initial API versions (0.x.y) until the first public release of an initial or stable API Version within the context of a CAMARA Meta-release. The work within Sandbox API Repositories - like in all API repositories - shall follow the governance and guidelines of CAMARA, including but not limited to the ProjectCharter, the Code of Conduct, the Contribution guidelines, the API Design Guidelines of Commonalities and the Release Process defined in Release Management.

A Sandbox API Repository can be created independent of a CAMARA Sub Project (Independent Sandbox Repository) or in context of an existing CAMARA Sub Project. It is the first stage for every new API proposal developed in CAMARA, for details see the [API Onboarding and Lifecycle documentation](./API-Onboarding-and-Lifecycle.md).

* If a Sandbox API Repository belongs to a Sub Project it links within the README.md to the Sub Project wiki home page. Mailing list, meetings will be for these Sandbox API Repositories organized in context of the Sub Project. The Sub Project may already nominate or approve Maintainers for the Sandbox API Repository, which are with that also Maintainers of the Sub Project.

* An Independent Sandbox API Repository which is not part of an existing Sub Project will get a page in a separate section of the [CAMARA wiki](https://lf-camaraproject.atlassian.net/), a preliminary mailing list, a Slack channel, and (on request) a Zoom meeting to be able to communicate with the community and attract contributors. The MAINTAINERS.md file of an Independent Sub Project may already list contributors who are committed to the support the API Repository as Maintainers. But they are not yet Maintainers of a Sub Project in the sense of the Project Charter.

A Sandbox API Repository must have at least one Codeowner. If the Sandbox API Repository has two or more Codeowners the activation of branch protection rules is recommended.

Sandbox API Repositories are marked with a "Sandbox" badge in the README.md file and get a topic "Sandbox" assigned within the CAMARA GitHub Organization.

**Incubating API Repositories**

An Incubating API Repository is meant for the further evolution of an API which has been implemented already by at least one operator, fits into the CAMARA API portfolio and has gained sufficient support within the CAMARA community. For details of the transition process to Incubating stage see the [API Onboarding and Lifecycle documentation](./API-Onboarding-and-Lifecycle.md).

An Incubating API Repository has the same structure as a Sandbox API Repository, with the following additional requirements: 
* An Incubating API Repository must belong to a CAMARA Sub Project (either an existing one or a new Sub Project created as part of the incubation process). 
* The repository should have at least three Maintainers from different companies (out of the group of Maintainers of the Sub Project it belongs to). 
* Branch protection rules must be activated, therefore a minimum of two Codeowners is required. 
* All changes and contributions in the repository are following the description below.

Incubating API Repositories are marked with an "Incubating" badge in the README.md file and get a topic "Incubating" assigned within the CAMARA GitHub Organization.

**Graduated API Repositories**

A Graduated API Repository maintains a stable CAMARA API which has been widely adopted within the market. Details of the Graduation process will be defined within the [API Onboarding and Lifecycle documentation](./API-Onboarding-and-Lifecycle.md). 

Graduated API Repositories have no additional technical requirements compared to Incubating API Repositories. It is important that the Sub Project ensures that there is a succession management for leaving Maintainers and Codeowners in place.

Graduated API Repositories are marked with a "Graduated" badge in the README.md file and get a topic "Graduated" assigned within the CAMARA GitHub Organization.

**Working Group Repositories**

Working Groups are primarily used to facilitate topics of discussion that are in scope for the CAMARA Project but that are short-lived or that span multiple Sub Projects. If a subset of Project participants wants to get together and discuss a topic, they can do so by forming a Working Group. The Technical Steering Committee (TSC) decides upon implementing or removing Working Groups, and their Maintainers.

Working Groups are documented in a separate section of [CAMARA wiki](https://lf-camaraproject.atlassian.net/) and can have one or multiple GitHub repositories following the API Repository template (the rules for API Repositories apply). In the Readme.md file the repositories of Working Groups are marked with a "Working Group" badge.

**Repositories Rules**

As mentioned before the contributions to the Sub Projects were documented in the respective GitHub repositories of the Sub Projects, contributions to Independent Sandbox Repositories were documented within that, and the contributions to Working Groups were documented in the GitHub repositories of the Working Groups. All contributions beyond that, esp. contributions to the Project itself or the TSC are documented in the GitHub repository “Governance”. Additional repositories can be created for project administration purposes. 

For ease of use there are templates for API and Provider Implementation Repositories, containing all necessary files which can be cloned and adapted. When cloning it has to be ensured that also the branch protection rules are active in the new repositories if needed. For Working Group repositories the API Repository template should be used and adapted.

Only Markdown format shall be used as the document standard for documents in the main branch of API and Working Group repositories. The only exceptions are supporting documents, for which other formats like PDF or PPT are allowed. Note: Documents which are meant as base for discussion or to explain change requests are best attached to an issue. Informal supporting documents are best located within the Sub Project or Working Group wiki.

**Mailing list "all"**

A Project wide mailing list is established, each Project participant documented in [PARTICIPANTS.MD](./PARTICIPANTS.MD) is added. A message to all Project participants can be sent using <all@lists.camaraproject.org>.

## Changes and contributions to CAMARA ##

In the Project the “Fork and pull model” is used. Changes and contributions to CAMARA shall follow this process:
![PR_Approval_Process](/documentation/images/PR_Approval_Process.png)

1 All changes / contributions shall start with an issue to which initial documents, API definitions or code can be attached. The issue should be discussed in the Sub Project community before working out the best form of action. By means of the issue the traceability of the contributions to CAMARA is also ensured. In addition as general rule there shall be no (later) pull request without a reference to an issue (except minor corrections, to be labeled as “minor”).

2 Either the issue creator or one of the Sub Project Maintainers then shall assign the issue to one of the Contributors of the Sub Project.

3 This Contributor shall create a fork (if not yet done before), shall create a new branch within the fork, and shall copy the branch link into the issue. For the naming of the branch a clear and concrete description shall be used.

Now they can work on the solution and add commits to the branch. If they are done with the work the Contributor shall create a pull request, refer to the addressed issue(s) in the pull request description (and vice versa) and add the commits to the pull request. For the naming of the pull request a clear and concrete description shall be used.

4 The Contributor now shall invite other Sub Project Contributors to review the pull request. The Contributor shall invite at least 2 Maintainers, ideally from different companies and all Codeowners of the repository. As default all Maintainers and all Codeowners of the repository shall be invited as reviewers. Only the initial Contributor should edit a pull request in review (the Contributor is responsible to react on comments) or allow other Contributors explicitly to commit into the pull request.

5 The pull request shall be approved by all Contributors included in the review within a 2 weeks period. If a Contributor doesn't perform a review within that time frame the Contributor automatically accepts the pull request. For conflicting cases rules will be defined later. A two days cool off period after the approval shall be kept. A pull request review in certain cases might lead to a pull request not being approved. In this case, the Codeowner shall close the pull request (and the branch, and the issue) with the appropriate comments and the contribution shall not get merged into the main branch.

6 Finally one of the Codeowners of the repository shall merge the pull request into the main branch. By that the Codeowner closes the pull request. The Codeowner also shall close the branch and the issue (if not already automatically done).
Deliverables of the Sub Project are all artifacts in the main branch of its repositories.

More details can be found in the [CONTRIBUTING.MD](https://github.com/camaraproject/Governance/blob/main/CONTRIBUTING.md).

## Working Groups ##

**API Backlog**

The API Backlog Working Group is supervised by the TSC. The responsibilities of the Working Group are to take the decisions about API Proposals, including the creation of (Sandbox) API Repositories, to support the transition process of API Repositories, and to prepare the material for the creation of new Sub Projects or scope changes of existing Sub Projects (e.g. adding new API Repositories to a Sub Project).

The decision about new Sandbox API Repositories will be taken by the Working Group. Decision about the transition to Incubating or Graduated stage, and the onboarding of new Sub Projects will be taken by the TSC. Changes of existing Sub Projects have to be approved by the involved Sub Projects.

The API onboarding and API lifecycle process in CAMARA are described in the [API Onboarding and Lifecycle documentation](./API-Onboarding-and-Lifecycle.md).

**Commonalities**

CAMARA commonalities shall be processed in a Working Group "Commonalities”. The Working Group “Commonalities” works under the supervision of the TSC. The scope of the Working Group is to create guidelines, best practices and concept documents relevant for all APIs in CAMARA. The Commonalities Working Group shall work e.g. on the development of a common meta model that shall be used as a reference across the Sub Projects. It is open for members of any Sub Project or Working Group to raise issues in the Technical Steering Committee (TSC) for relevant topics on a need basis.

All Sub Projects must comply with the work in the Commonalities Working Group.

**Identity and Consent Management**

The Identity and Consent Management Working Group, operating under the supervision of the Technical Steering Committee (TSC), focuses on defining and developing privacy-first solutions for subscriber identification, and user authentication, and the purpose of the API access, and user consent capture, storage, and management. These solutions ensure that the API access is always authorized and secure.
The Working Group's efforts include developing the Security and Interoperability Profile, which encompasses CAMARA definitions for authentication and authorization (AuthN/AuthZ) flows.

All Sub Projects must comply with the work in the Identity and Consent Management Working Group.

**Marketing**

The Marketing Working Group is responsible to plan and perform marketing activities for CAMARA and to maintain marketing material (onepager, presentation, website, GitHub, ...). It is supervised by the Board of the CAMARA Fund.

**Release management**

Each API Repository shall follow a release process. The release process and the cadence of common meta-releases shall be determined by the TSC, and on a regularly published schedule. Milestones shall be set up within each API Repository to ensure the ability of each API Repository to meet the release schedule as defined by the TSC.

Goal is that all the Sub Projects updates are released at the same release milestone so that the implementors of the APIs become accustomed to the regular release cadence of CAMARA. 

The Release Management working group is supervised by the TSC. The scope of the Working Group is the definition of guidelines and best practices for the API Versioning and release management within the Sub Projects, API Repositories, and Working Groups, and the support of the TSC in its responsibilities for Release Management.

All API and Working Group Repositories must comply with the work in the Release Management Working Group for releases and pre-releases.

## Roles, Responsibilities and Requirements

**Project participants**

Project participant status may be given to those who intend to make ongoing contributions to the CAMARA Project. This is usually in the form of code submissions and improvements and/or notable work on documentation but may also include other contributions such as organizing events or user support.

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

Each Project participant can contribute to the Repositories of the Project by creating pull requests. Contributors should be subscribed to the mailing list of the Sub Project, Independent Sandbox Repository, or Working Group. The list of Contributors of a specific Repository is maintained by the administrators of the Project using GitHub functionality.

**Codeowners**

Codeowners can merge code and accept pull requests. A Codeowner is responsible for the overall quality and stewardship of the Repository. Contributors can get a Codeowner role if they are Contributors and deeply involved in contributing code, pull request review, and triaging issues in a Sub Project or Working Group for a minimum of three months and perform an ongoing contribution. Codeowners are decided by the Maintainers responsible for the Repository and formalized by changing the CODEOWNERS file. Changes in code ownership have to be announced on the mailing list of the Sub Project or Working Group.

**Maintainers**

Maintainers are the leaders of a Sub Project or Working Group. Maintainers are first and foremost contributors who have shown a commitment to the long-term success of the Project. Contributors wanting to become Maintainers are expected to be deeply involved in contributing code, pull request review, and issue triaging issues in a Repository of the Project for a minimum of three months and perform an ongoing contribution to the Project.

Note: Project participants listed within the MAINTAINERS.md file of an Independent Sandbox API Repository are candidates to get Maintainers when the API Repository gets part of a Sub Project, but are not yet Maintainers of a Sub Project in the context of the Project Governance. However, the following description of the role should also apply to them.

**Changes in maintainership**

When creating a new Sub Project or Working Group the TSC also nominates the initial Maintainers for the repository/ies of the new Sub Project or Working Group. After that the Maintainers of a Sub Project or Working Group decide upon the maintainership of the Repositories belonging to the Sub Project or Working Group.

The merge of two Sub Projects, the move of an API Repository from one Sub Project to another Sub Project, or the adoption of an Independent Sandbox API Repository by a Sub Project need the consensus of the the Maintainers of the involved Sub Projects. The resulting Maintainer team(s) of the Sub Project(s) are again defined as the union of the Maintainers of the API Repositories of the Sub Project(s) (see above). 

Changes in maintainership of a Sub Project have to be announced on the mailing list of the Sub Project. They are decided  by [lazy consensus ](https://couchdb.apache.org/bylaws.html#lazy) by all Maintainers of a Sub Project and formalized by changing the MAINTAINERS.MD file of the respective API Repository/ies.

Changes in maintainership of a Working Group have to be announced on the mailing list of the TSC. They are decided  by [lazy consensus ](https://couchdb.apache.org/bylaws.html#lazy) by the TSC Participants and formalized by changing the MAINTAINERS.MD file of the respective Working Group Repository/ies.

A Maintainer may resign from the maintainership of one or multiple API Repositories by notifying the respective mailing list. A Maintainer with no Project activity for a year is considered to have resigned. Maintainers that wish to resign are encouraged to propose another Project participant to take over their Project work.

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

Maintainers lead one or more Sub Project(s), Working Group(s) or parts thereof and serve as a point of conflict resolution amongst the Contributors and are the technical authority for a Sub Project or Working Group (responsible for vision and direction and overall design, choose/approve change proposals, field technical escalations, etc.). They *MUST* have demonstrated both good judgment and responsibility towards the health of that Sub Project. Maintainers *MUST* set technical direction and make or approve design decisions for their Sub Project or Working Group - either directly, or through delegation of these responsibilities.

Maintainers are also intended to be organizers and facilitators, responsible for the continued operation and progress of the Sub Project and for communication and co-ordination with the other Sub Projects, Working Groups, the TSC, and the Project participants. 

Maintainers should actively participate in pull request reviews and are expected to respond to assigned pull requests in a reasonable time frame, either providing insights, or assign the pull requests to other Maintainers.

The following responsibilities must be met by the Maintainer for a Sub Project:

- Make and approve technical design decisions for the Sub Project or Working Group.
- Set the technical direction and priorities for the Sub Project or Working Group.
- Define milestones and releases.
- Mentor and guide Contributors and Codeowners to the Sub Project or Working Group.
- Ensure continued health of the Sub Project or Working Group
  - Adequate test coverage to confidently release
  - Tests are passing reliably (i.e. not flaky) and are fixed when they fail
- Ensure a healthy process for discussion and decision making is in place and is followed by Contributors.
- Work with other Sub Project and Working Group leaders to maintain the Project's overall health and success holistically.
