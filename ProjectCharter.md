# Project Charter

## Technical Charter of the CAMARA Project

This technical charter (the “Charter”) describes the rules and governance of the CAMARA Project (the “Project”). It is meant to be followed by all the contributors, codeowners and maintainers of, and other participants in (collectively, “Project participants”), the Project. Common terminology used in this governance document is defined below:
- **CAMARA Project**: The sum of all activities and Sub Projects performed under the governance protocol defined in this document.
- **Project participant**: participants in the CAMARA Project.
- **Technical Steering Committee (TSC)**: the technical oversight body for the Project.
- **TSC participant**: a member of the TSC.
- **Working Group**: a group of Project participants working on a specific topic as directed by the TSC.
- **Working Group participant**: a Project participant contributing to a specific Working Group, which may span one or more Sub Projects.
- **Sub Project**: A subproject of the CAMARA Project led by a voluntary group, open to anyone to participate.
- **Repository**: Sub Projects and Working Groups have one or multiple GitHub repositories to document their artifacts and documentation.
- **Sandbox Repositories** can exist independent of a Sub Project or Working Group, e.g. during the initial development phase of an API. 
- **Maintainer**: is a leader of an individual Sub Project or Working Group who has been named in the MAINTAINERS.MD files of one of the repositories of the Sub Project or Working Group. 
- **Codeowner**: a committer of an individual Repository who has been named in the CODEOWNERS files of the Repository. Codeowners merge code and accept pull requests.
- **Contributor**: a Project participant who contributes to the Project and creates pull requests.
- **Partner**: is an organization who employs a Project participant, or on whose behalf a Project participant is authorized to make contributions.

The Project is an independent open-source project, not controlled by any single company or organization and has been established as CAMARA Project a Series of LF Projects, LLC. LF Projects, LLC is a Delaware series limited liability company (“LF Projects”). Governance for the CAMARA Fund is documented in the CAMARA Fund Charter.

For specific guidance on the practical steps for contributing to the Project and any Sub Project or Working Group please see our [Contribution Guidelines](./CONTRIBUTING.md).

## Principles

The CAMARA Project adheres to the following principles:
- Open: The Project is open source. That especially means that the Project has a clear pro-competitive goal to define/harmonize and develop open, global, and interoperable API solutions using an open and transparent process at all times. All Project participants are encouraged to be observant that there is no patent ambush and no market power abuse and report if any.
- Welcoming and respectful: We abide by the [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
- Transparent and accessible: Changes to the Project organization, Project code repositories, and activities related to LF Projects and the Linux Foundation are done in public. A primary reason that the CAMARA Project exists is as a forum for collaboration. The work in the Project should be done in the open. Except as authorized by the TSC with respect to security and code of conduct issues, Project participants must communicate in the open, ensure other Project participants can find notes of meetings, discussions, designs, and decisions, and periodically communicate a high-level summary of their contribution work to the Project.
- Merit: Ideas and contributions are accepted according to their technical merit and alignment with Project objectives, scope, and design principles.
- Diversity: All boards in CAMARA should reflect a diverse mix of companies.

## CAMARA Project

A global partnership could address much of the challenges in scaling API services across heterogenous operator architectures.

The development of open, global, and interoperable API solutions could benefit customers and developer ecosystems by giving access to operator capabilities in whatever network customers are in and therefore allow applications to run consistently between telco networks and countries. A new form of collaboration between various players (telcos, ISVs, device manufacturers, hyperscalers, etc.) could address much of the challenges in scaling API services across heterogenous operator architectures as well as advance the connectivity industry towards a more robust and faster core network, encourage the faster adoption of capabilities and as a result create value for the entire tech industry.

* Accelerate technology development
    * Build sustainable ecosystems around collaborative projects across industries.
    * Drive industry alignment by facilitating industry discussions with telcos, ISVs, device manufacturers, hyperscalers, etc.
* Harmonization of APIs
    * Harmonize and convert APIs to a user understandable format.
    * Achieve harmonization through working code vs. documents.
    * Implementation experience should guide the harmonization process.
    * Enable interoperability (e.g. effortless portability of applications between different operators), compatibility (applicability to different network technologies) and interconnectivity (to enable interoperator collaboration).
* Education and promotion
    * Actively promote the APIs via various forums, events, conferences, training programs, ecosystems and social media.
    * Promote best practices by aggregating and publishing lessons learned.
* Accelerate commercial adoption
    * Create awareness around use cases and services.
    * Minimize implementation effort though easy-to-consume APIs.
    * Foster the API integration in relevant developer’s environments and ecosystems.
    * Enable the provision of customer service and support for the design phase and experimentation.

APIs grouped by services and bundled up into API families could reduce the complexity of accessing operator capabilities for developers and enterprises. CAMARA Project is an independent open source project and not controlled by any single company.  Monetization of APIs is outside the Project’s scope; designing and consumption of APIs is within scope. 

## Scope of the Project

**Functional and technical scope**

From a functional perspective the scope is limited to telco APIs, that means APIs in the domain of telco mobile networks, telco fixed line networks, telco edge cloud, etc. or supporting these (e.g. for authentication). CAMARA only works on customer-facing northbound APIs. East-west federation / roaming APIs are out of scope for CAMARA.

**Northbound scope**

We differentiate between 3 types of Northbound APIs:
-	Service APIs: APIs intended for end consumers and integrated by developers to invoke a certain telco capability.
-	Service Management APIs: APIs intended for end consumers to manage or get data about offered Service APIs in application runtime, e.g., check service availability or performance information.
-	Operate APIs: Operational and maintenance APIs provided by a telco to channel partners for the purpose of service fulfillment and assurance to their [channel partner] customers. This may include service provisioning for a mobile user, technical API performance monitoring, fault ticketing, information exchange such as product catalog, pricing, settlement, etc.

In the following picture you can find an illustration of these 3 types of APIs. Service APIs and Service Management APIs are in scope of CAMARA (and both will be referred to in the following as CAMARA APIs), Operate APIs are out of scope of CAMARA (these are already covered by other SDOs = Standards Development Organizations like TM Forum).

![Interface types in NaaS](/documentation/images/InterfaceTypesInNaaS.jpg)
*Figure 1 - Interface types in NaaS*

**Transformation functions**

Service APIs and Service Management APIs mean an abstraction / aggregation of e.g. 3GPP APIs, Broadband Forum APIs or ETSI MEC APIs to hide telco complexity, keep control at the operator side and fulfill regulatory and data privacy constraints.

![Transformation function](/documentation/images/TransformationFunction.jpg)  
*Figure 2 - The transformation function translates exposed service APIs into call flows that invoke internal telco capabilities*

The definition and documentation of CAMARA APIs (including the mapping tables for the attributes to the southbound APIs if useful) is in scope of the Project and in scope of the harmonization. The transformations functions (business logic that calls the southbound APIs, transforms the data and provides the function for the CAMARA APIs) are in scope of the Project as example or reference implementations, but not in scope of the harmonization. So each telco operator can implement the transformation functions in the best manner considering network topology and vendors, and can use the reference implementation as an orientation and starting point.

**API consumption**

The way how the different API types shall be consumed is shown in the figure below.

![Typical consumers / producers of each API type](/documentation/images/ConsumersProducersOfAPIType.jpg) 
*Figure 3 - Typical consumers / producers of each API type*

Hyperscalers and aggregators have the possibility to create own enriched products based on the CAMARA APIs and expose that in addition to the CAMARA APIs.

Remark: In Figure 1, 3 and 4 we mention "Consumers", "End Consumers" and "API Consumers" in the following sense:
* Developers of customer companies or independent developers can include API calls into their applications/code
* End users of these applications then trigger API calls while using the applications

**Alignment with other SDOs**

The following picture shows how the different API standards complement each other.

![Different entities participating in the NaaS service standardization](/documentation/images/NaaSServiceStandardization.jpg)
*Figure 4 - Different entities participating in the NaaS service standardization*

CAMARA project defines CAMARA APIs, with a contribution-driven approach and in collaboration with the developer community.

TMForum develops the Operate APIs, as an evolution of its Open APIs, working jointly with aggregator and developer platform owners, to facilitate their integration with the operator’s NaaS Platforms.

Several SDOs cover the different technology domains that provide the telco capabilities, through Technology-specific APIs, that are exposed by CAMARA, like Broadband Forum (Home and fixed access networks), O-RAN (Radio access network), IETF and ONF (Transport networks), 3GPP (Radio access and core networks), ETSI (network function virtualization), Cloud Native Computing Foundation (container management), etc. These SDOs provide exposure functions to be able to interact with the network systems from external platforms.

More details can be found in the whitepaper “The Ecosystem for Open Gateway NaaS API Development” (jointly published by GSMA, CAMARA, Linux Foundation and TMForum) available [here](./documentation/The-Ecosystem-for-Open-Gateway-NaaS-API-development.pdf).

**Service scope**

The service scope of the CAMARA Project is limited to the following activities:
-	Collect API requirements from GSMA OPG (Operator Platform Group, a GSMA group that defines the reference architecture and requirements of the platform the operators use to expose their capabilities to Customers via APIs) and other sources. That can be a (prioritized) list of API families seen as useful for the customers, a functional description of the APIs (attributes, function, result), and also non-functional requirements for the APIs (response time, scalability, performance, etc.). All APIs developed within GSMA/OPG and contributed to the CAMARA Project will be developed under Apache-2.0.
-	Define Service APIs and Service Management APIs (e.g. by Swagger) and create test plan / cases and tools from a business and API consumer perspective
-	Develop Service APIs and Service Management APIs (and reference implementation for transformation functions)
-	Create test cases and perform verifications and tests from developer perspective (to show that the Service APIs, the and Service Management APIs and the transformation functions have been developed correctly)
-	Create developer friendly documentation for Service APIs and Service Management APIs
-	Test Service APIs and Service Management APIs from business and customer perspective (validation) in telco network(s)
-	Create deployment packages for Service APIs and Service Management APIs
-	Create a reference architecture for Service APIs and Service Management APIs (if possible preferred solution is to refer to an existing architecture)
-	Define a standard API lifecycle, development and test process including tools for the project

**Deliverables**

The following deliverables are provided by the CAMARA Project:
-	Service API and Service Management API definitions and documentation
-	Optionally Service API and Service Management API code (reference implementation for transformation functions) and
-	Test plans, cases and tools

both contained in deployment packages.
In addition a
-	Reference architecture for Service APIs and Service Management APIs
-	Description of the standard API lifecycle, development and test process

is created.

## Governance

**Technical Steering Committee (TSC)**

The Technical Steering Committee is composed of:
-	10 representatives of Sub Projects as selected by the Maintainers of Sub Projects and Working Groups (“Sub Project representatives”); 
-	3 representatives of the End-User Council as selected by the End-User Council (“EUC representatives”); 
-	1 non-voting representative of the GSMA and
-	1 non-voting representative of the TMForum

Any Maintainer may nominate themselves or another Maintainer of any Sub Project or Working Group for consideration as a Sub Project representative. The Maintainers will vote using ranked choice voting (or another method approved by the TSC) and those 10 nominees receiving the highest number of votes will be elected to the TSC as Sub Project representatives.

Any participant of the EUC may recommend any participant of the EUC for consideration as a EUC representative. EUC participants will vote using ranked choice voting (or another method approved by the TSC) and those 3 nominees receiving the highest number of votes will be elected as EUC representatives.

TSC commitments will be 15 months. The first twelve months will be duties as described herein. The final three months will be non-voting, shepherding of incoming TSC members to maintain council continuity.

The TSC includes one non-voting participant from both GSMA and TM Forum.

All voting TSC participants will vote using ranked choice voting (or another method approved by the TSC) to determine the chair.

The TSC may choose an alternative approach for determining the voting participants of the TSC (any such alternative approach will be documented in the Project’s repository). Any meetings of the TSC are intended to be open to the public, and can be conducted electronically, via teleconference, or in person.

The TSC may approve an alternate attendance policy. Any TSC participant who fails to attend, or to have a alternate attend on their behalf, more than 30% of the meetings of the TSC in any six-month period will lose the right to vote, and will not be counted for quorum purposes, on the TSC until that TSC participant has attended two consecutive meetings of the TSC (with their vote restored as of the second meeting).

The technical roles of the Sub Projects, Working Groups and Sandbox Repositories are described in the [Project Structure And Roles](./ProjectStructureAndRoles.md) file. The TSC may adopt or modify roles so long as the roles are documented in the [Project Structure And Roles](./ProjectStructureAndRoles.md) file. Participation in the Project through becoming a Project participant is open to anyone so long as they abide by the terms of this Charter.

The TSC may (1) establish workflow procedures for the submission, approval, and closure/archiving of Sub Projects and Working Groups, (2) set requirements for the change of Project participants from one technical role to another, and (3) amend, adjust, refine and/or eliminate any technical roles, create new roles, and publicly document any roles, as it sees fit.

Responsibilities: The TSC is responsible for all aspects of oversight relating to the Project, which may include:
- approving Sandbox Repository and Sub Project proposals (including, but not limited to, incubation, deprecation, and changes to a Sub Project’s scope);
- organizing Sub Projects and removing Sub Projects;
- creating and removing of Working Groups to focus on cross-project technical issues and requirements;
- appointing representatives to work with other open source or open standards communities;
- determining the release cadence of the Sub Projects and the scope of the releases;
- approve election processes for the technical Project;
- establishing community norms, workflows, issuing releases, and security issue reporting policies;
- approving and implementing policies and processes for contributing (to be published in the [Contribution Guidelines](./CONTRIBUTING.md)) and coordinating with LF Projects to resolve matters or concerns that may arise as set forth in this Charter;
- discussions, seeking consensus, and where necessary, voting on technical matters relating to the code base that affect multiple projects; and
- receive and resolve escalations from Sub Projects on blocked topics or areas where Sub Projects or Working Groups are seeking input from the TSC, i.e. when the established decision process did not end up in a resolution for that topic at Sub Project or Working Group level.

It is open for members of any Sub Project or Working Group to raise issues in the TSC group for relevant topics on a need basis.

**End-User Council**

The EUC is composed of individuals employed by organizations that use CAMARA APIs and can provide feedback on how those APIs work. EUC participants are expected to consist primarily of developers but telecommunications companies and aggregators could also qualify if they utilize APIs to build projects or services for their own use. If there is a question as to whether a particular organization qualifies to appoint someone to the EUC, the TSC will decide.

The EUC is expected to meet monthly, and EUC meetings will be open to the public.

## Decision Making

**Voting Principles**

The CAMARA Project usually runs by informal consensus, however sometimes a formal decision must be made (reasons for this see below).

Depending on the subject matter, different methods of voting are used as laid out below.

For all votes, voting must be open for at least one week. The end date should be clearly stated in the call to vote. A vote may be called and closed early if enough votes have come in one way so that further votes cannot change the final decision.

In all cases, of votes within the TSC, End-User Council, Working Groups or Sub Projects, only Project participants are eligible to vote, with the sole exception of the forced removal of a Project participant, in which said Project participant is not eligible to vote.

Discussion and votes on personnel matters (including but not limited to Project participation) are held in private. All other discussion and votes are held in public.

For public discussions, anyone interested is encouraged to participate. Formal power to object or vote is limited to Project participants.

**Consensus**

The default decision making mechanism for the CAMARA Project is [lazy consensus](https://couchdb.apache.org/bylaws.html#lazy). This means that any decision on technical issues is considered supported by the team as long as nobody objects based on substantiated technical grounds.

Silence on any consensus decision is implicit agreement and equivalent to explicit agreement. Explicit agreement may be stated at will. Decisions may, but do not need to be called out and put up for decision on the appropriate mailing list at any time and by anyone.

Consensus decisions can never override or go against the spirit of an earlier explicit vote.

If any Project participant raises objections, the Project participants work together towards a solution that all involved can accept. This solution is again subject to [lazy consensus](https://couchdb.apache.org/bylaws.html#lazy).

In case no consensus can be found, but a decision one way or the other must be made, any Project participant may call a formal majority vote.

**Majority vote**

Majority votes must be called explicitly in a separate thread on the appropriate mailing list. The subject must be prefixed with [VOTE]. In the body, the call to vote must state the proposal being voted on. It should reference any discussion leading up to this point.

Votes may take the form of a single proposal, with the option to vote yes or no, or the form of multiple alternatives.

A vote on a single proposal is considered successful if more eligible to vote are in favor than against.

If there are multiple alternatives, participants may vote for one or more alternatives, or vote “no” to object to all alternatives. It is not possible to cast an “abstain” vote. A vote on multiple alternatives is considered decided in favor of one alternative if it has received the most votes in favor, and a vote from more than half of those voting. Should no alternative reach this quorum, another vote on a reduced number of options may be called separately.

**Supermajority vote**

Supermajority votes must be called explicitly in a separate thread on the appropriate mailing list. The subject must be prefixed with [VOTE]. In the body, the call to vote must state the proposal being voted on. It should reference any discussion leading up to this point.

Votes may take the form of a single proposal, with the option to vote yes or no, or the form of multiple alternatives.

A vote on a single proposal is considered successful if at least two thirds of those eligible to vote in favor.

If there are multiple alternatives, participants may vote for one or more alternatives, or vote “no” to object to all alternatives. It is not possible to cast an “abstain” vote. A vote on multiple alternatives is considered decided in favor of one alternative if it has received the most votes in favor, and a vote from at least two thirds of those voting. Should no alternative reach this quorum, another vote on a reduced number of options may be called separately.

**TSC decisions**

TSC votes can be initiated by any TSC voting participant.

For votes taken during a TSC meeting (in person, by telephone or online conference or similar), quorum requires at least 50% of all voting participants of the TSC to be present. The TSC may continue to meet if quorum is not met but will be prevented from making any decisions at the meeting.  Except as provided elsewhere in this Charter, decisions by vote at a TSC meeting require a majority vote of those in attendance, provided quorum is met. If an already taken decision has to be revised a super majority is necessary.

For votes taken by email or similar asynchronous means, voting decisions require at least a 50% vote of all participants of the TSC. Decision is then taken by majority vote. If an already taken decision has to be revised a super majority is necessary.

**Technical decisions**

Technical proposals that only affect a single Sub Project are decided by [lazy consensus](https://couchdb.apache.org/bylaws.html#lazy). If no consensus can be reached, the matter may be resolved by majority vote. 

Technical decisions that span multiple parts of the CAMARA Project should be discussed and made in the Commonalities Working Group or other Working Groups established by TSC for cross-project technical issues.
Decisions are usually made by [lazy consensus](https://couchdb.apache.org/bylaws.html#lazy). If no consensus can be reached, the matter may be resolved by majority vote by the TSC.
 
## Intellectual Property Policy

Project participants acknowledge that the copyright in all new contributions will be retained by the copyright holder as independent works of authorship and that no contributor or copyright holder will be required to assign copyrights to the Project.

Except with respect to alternative licenses approved by the TSC as described below, all contributions to the Project are subject to the following:
- All new inbound contributions (of any materials including APIs and definitions, machine-readable YAML files and similar contributions, code, testing scripts and tools, human-readable documentation and information that is designed to provide instructions or other information regarding Project materials or contributions) to the Project (collectively “Project Materials”) must be made using the Apache License, Version 2.0, available at https://www.apache.org/licenses/LICENSE-2.0 (the “Project License”).
- Only exception is the documentation contributed to or created by the Outreach Committee (former Marketing Working Group) in the repository [https://github.com/camaraproject/Marketing](https://github.com/camaraproject/Marketing). For that the [Creative Commons Attribution 4.0 International license](https://creativecommons.org/licenses/by/4.0/legalcode.txt) shall apply. It is strongly forbidden to save any API-related definition, documentation or code in this repository.
- All new inbound contributions of Project Materials must be:
  - accompanied by a Developer Certificate of Origin (http://developercertificate.org) sign-off in the source code system that is submitted through a TSC approved contribution process which will bind the authorized contributor and, if not self-employed, their employer to the applicable license; and
  - made pursuant to a duly executed Contributor License Agreement (in the form as approved by the TSC).
- All outbound Project Materials will be made available under the Project License.
- The Project may seek to integrate and contribute back to other open source projects (“Upstream Projects”). In such cases, the Project will conform to all license requirements of the Upstream Projects, including dependencies, leveraged by the Project. Upstream Project code contributions not stored within the Project’s main code repository will comply with the contribution process and license terms for the applicable Upstream Project.

The TSC may approve the use of an alternative license or licenses for inbound or outbound contributions on an exception basis. To request an exception, please describe the contribution, the alternative open source license(s), and the justification for using an alternative open source license for the Project. License exceptions must be approved by a two-thirds vote of the entire TSC.

Contributed files should contain license information, such as SPDX short form identifiers, indicating the open source license or licenses pertaining to the file.

## Policies

Project participants will comply with the policies of LF Projects as may be adopted and amended by LF Projects, including, without limitation the policies listed at https://lfprojects.org/policies/ which include the antitrust policy located here: https://lfprojects.org/policies/antitrust-policy/.

When amending or adopting any policy applicable to the Project, LF Projects will publish such policy, as to be amended or adopted, on its web site at least 30 days prior to such policy taking effect; provided, however, that in the case of any amendment of the Trademark Policy or Terms of Use of LF Projects, any such amendment is effective upon publication on LF Projects’ web site.

All Project participants must allow open participation from any individual or organization meeting the requirements for contributing under this Charter and any policies adopted for all Project participants by the TSC, regardless of competitive interests. Put another way, the Project team must not seek to exclude any Project participant based on any criteria, requirement, or reason other than those that are reasonable and applied on a non-discriminatory basis to all Project participants.

LF Projects will hold title to all trade or service marks used by the Project (“Project Trademarks”), whether based on common law or registered rights, and domain names and code repository accounts. Project Trademarks will be transferred and assigned to LF Projects to hold on behalf of the Project. Any use of any Project Trademarks by collaborators in the Project will be in accordance with the license from LF Projects and insure to the benefit of LF Projects.

Under no circumstances will the Project undertake or will LF Projects be expected or required to undertake any action on behalf of the Project that is inconsistent with the tax status or purpose, as applicable, of LF Projects or its affiliates.

## Amendment

This Charter may be amended by a two-thirds vote of two-thirds of the TSC and is subject to approval by LF Projects.
