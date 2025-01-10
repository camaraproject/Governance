# API Onboarding and Management in CAMARA

## Introduction

This document describes a clear, consistent, and transparent process for the onboarding (submission), evaluation, and management (maintenance and lifecycle evolution) of API proposals in the CAMARA Project.

The process pipeline is depicted in the figure below.

![API process pipeline](images/API_process_pipeline.png)

All stages within this process pipeline are documented in the CAMARA API overview list. Details and clarifications on these stages are provided in the following sections.

## Submission of an API Proposal

The pipeline begins with the submission of an API proposal. This proposal can represent a new API or an enhancement to an existing API.

### Steps for Submission

1. **Create a New Issue**  
   - Open a new issue in the [API Backlog repository](https://github.com/camaraproject/APIBacklog) using the designated issue template.
   - Clearly describe whether it is a new API proposal or an enhancement to an existing API.

2. **Submit a Pull Request (PR)**  
   - Fill out the appropriate API proposal or enhancement template available in the [API Backlog documentation](https://github.com/camaraproject/APIBacklog/tree/main/documentation).
   - Submit this template via a Pull Request (PR) to the repository folder for API proposals.
   - Ensure that the PR is linked to the issue created in step 1.

## Evaluation of API Proposals

After submission, proposals undergo a detailed evaluation process within the "API Backlog" Working Group (WG):

1. **Template Validation**  
   Backlog codeowners verify that all required fields are completed in the template. Missing information shall be provided by the API owner.

2. **Company Support Analysis**  
   Participating companies review the proposal, analyze its content and additional materials, and decide whether to support it from the backlog proposal stage. Supporters shall commit to providing at least one maintainer if accepted.

3. **Backlog Review Sessions**  
   During bi-weekly backlog sessions:
   - Backlog codeowners validate that:
     - The proposal adheres to governance and guidelines of CAMARA, including but not limited to the ProjectCharter, the Code of Conduct, the Contribution guidelines, the API Design Guidelines of Commonalities and the Release Process defined in Release Management.
     - The template is correctly filled out.
   - Participating companies assess:
     - Whether there is overlap with existing APIs.
     - If it is an enhancement or the proposal overlaps with an existin API, approval and validation from affected API groups is required.
   - If no issues arise (*lazy consensus*), the proposal is confirmed as valid for inclusion in the backlog.

4. **TSC Approval and Next Steps**  
   The Technical Steering Committee (TSC) reviews validated proposals during scheduled meetings.
   - Backlog codeowners include agreed proposals in TSC discussion, including target of the API (whether approved APIs will be hosted by a new or existing Sub-Project).
   - TSC confirms that backlog evaluations are complete and correct.
   - TSC approves or rejects proposals based on alignment with project goals and principles.
   
   If approved, onboarding tasks proceed as described below.

## Onboarding Tracker

Once an API proposal is approved by the TSC, onboarding tasks are tracked to ensure smooth implementation. These tasks include:

1. **Repository Creation**  
   A dedicated repository is created for the API under its assigned Sub-Project or as part of a new Sub-Project. The repository structure shall comply with [CAMARA governance guidelines](https://github.com/camaraproject/Governance/blob/main/ProjectStructureAndRoles.md).

2. **Infrastructure Setup**  
   Essential infrastructure is established:
   - Mailing lists for communication.
   - Initial documentation files (`README.md`, `CODEOWNERS`, `MAINTAINERS.md`).
   
3. **Maintainer Assignment**  
   Maintainership responsibilities are assigned based on commitments made during evaluation.

4. **Development Kickoff**  
   Stakeholders are notified that development can begin, and initial contributions are encouraged.

Progress on these tasks is documented in tracking issues maintained by the API Backlog Working Group.

## Lifecycle Management of APIs

All new APIs begin their journey in a *Sandbox* repository and evolve through defined lifecycle stages: **Sandbox → Incubated → Graduated → Archived**. This progression ensures clarity on maturity levels, development expectations, and implications for deployment and maintenance.

### Lifecycle Stages

#### **1. Sandbox Stage**
The Sandbox stage is the entry point for all new APIs. It is designed for experimentation and early development, allowing contributors to explore ideas without strict requirements.

**Characteristics:**
- APIs in this stage are experimental and may lack full documentation or test coverage.
- Open for contributions from any participant in the CAMARA Project.
- No guarantees of stability or long-term support.
- Can be initially independant, but should aim to either get accepted by an existing CAMARA Sub Project or to build up the necessary prerequisites to be able to apply for the creation of a new CAMARA Sub Project during Incubation.
- A Sandbox API Repository which is not part of an existing Sub Project will get a Wiki page (in the Sandbox section), a preliminary mailing list, a Slack channel, and (on request) a Zoom meeting for their communication.
- **Can release only Initial API versions, but no Stable API versions**

**Requirements:**
- The scope of the proposed API and initial use cases are described and fit in general into the scope of CAMARA.
- At least one initial Maintainer and one initial Codeowner (could be the same person) is nominated.

**Transition to Incubated Stage:**
To move to the Incubated stage, an API shall:
1. Release at least one Initial API version which is implemented by at least one operator (technical validation of the API in real environment).
2. Scope, Use cases, Documentation and API definition are fully aligned with Initial version Meta-release requirements (including alignment with latest available [Commonalities](https://github.com/camaraproject/Commonalities) and [ICM](https://github.com/camaraproject/IdentityAndConsentManagement) guidelines)
3. Have at least three committed maintainers listed in `MAINTAINERS.md` who support the API, belonging to three different companies. This requirement ensures a wide commitment of the industry in the API(s).
4. Maintainers of the Sandbox Repository apply for Incubation by opening an issue in the API Backlog working group.
5. The API Backlog working group will do a pre-check on behalf of the TSC, which will confirm (or not) the inclusion of the repository as Incubated in an existing (preferable) or new CAMARA subproject.

---

#### **2. Incubated Stage**
APIs in the Incubated stage have shown early promise with initial adoption and support from multiple contributors.

**Characteristics:**
- API(s) specified in an Incubated repository warranty stability and long-term support.
- An Incubated repositoriy is part of CAMARA Sub Project, including subroject Wiki Page, mailing list, Slack channel and Zoom meeting for communitacion.
- **Can release Initial and Stable API versions.**

**Requirements:**
- Full compliance with CAMARA governance standards as outlined in [Project Structure and Roles](https://github.com/camaraproject/Governance/blob/main/ProjectStructureAndRoles.md).
- Scope and use cases are fully documented. At this stage, API(s) part of the Incubated repository shall ensure that there is no overlap with any other API in the camera's portfolio, preventing duplicative functionalities to maintain a coherent set of offerings for developers.
- Have at least three committed maintainers listed in `MAINTAINERS.md` who support the API, belonging to three different companies. This requirement ensures a wide commitment of the industry in the API(s).
- Have at least three committed codeowners listed in `CODEOWNERS.md` who support the API, belonging (preferable) to three different companies. This requirement ensures that CAMARA Governance is followed.
- Branch protection is activated in the repository.


**Transition to Graduated Stage:**
To move to the Graduated stage, an API shall:
1. Demonstrate long-terms specification maturity by having participated within two CAMARA release cycles with at least one Stable API version.
2. Demonstrate wide market adoption across multiple companies or projects, by including APIs which have been deployed and certified within at least one complete market or #n operators across #m markets.
3. Maintainers of the Incubated Repository apply for Grduation by opening an issue in the API Backlog working group.
4. The API Backlog working group will do a pre-check on behalf of the TSC, which will confirm (or not) the inclusion of the repository as Graduated.

---

#### **3. Graduated Stage**
The Graduated stage represents mature APIs that are widely adopted and considered stable and mature both technical and commercially.

**Characteristics:**
- API(s) specified in a Graduated repository warranty stability and long-term support.
- **Can release Initial and Stable API versions.**

**Requirements:**
- Full compliance with CAMARA governance standards as outlined in [Project Structure and Roles](https://github.com/camaraproject/Governance/blob/main/ProjectStructureAndRoles.md).
- Evidence of active usage in production environments by multiple stakeholders.
- Have at least three committed maintainers listed in `MAINTAINERS.md` who support the API, belonging to three different companies. This requirement ensures a wide commitment of the industry in the API(s).
- Have at least three committed codeowners listed in `CODEOWNERS.md` who support the API, belonging to three different companies. This requirement ensures that CAMARA Governance is followed.
- Branch protection is activated in the repository.
- Stable group participation by ensuring mature processes to replace Maintainers and Codeowners within the API Repository based on merits (long-term group activity).
  
---

#### **4. Archived Stage**
The Archived stage is for deprecated or obsolete APIs that are no longer maintained or used actively. This status mainly applies for sandbox repositories that never reach an initial release, or incubated/graduated repositories that discontinue the evolution of APIs.

**Transition to Archived Stage:**
- Inactivity within a new Sandbox API repository:
  1. Three months (no contributions of documents or API specs)
  2. No release of an Initial API version after six months
- Lack of participation of a Sandbox API repository within two consecutive CAMARA release cycles
- Lack of participation of an Incubated or Graduated API repository within two consecutive CAMARA release cycle, if there would be changes necessary to stay aligned with the CAMARA Guidelines
- TSC is in charge of proposing and validating the transition of a repository to a Archived Stage

**Characteristics:**
- APIs in this stage are retained for historical reference but are not recommended for use.
- No active development or support is provided.

**Requirements:**
- Documentation indicating why the API was archived (e.g., replaced by a newer API, lack of usage).
- Clear communication to stakeholders about its status and alternatives if applicable.

---

## API Management and Maintenance

In case of a GO decision by the TSC, the designated Sub-Project assumes responsibility for the new API or API family. The Sub-Project begins contributing to the following areas:
- API definitions.
- API documentation.
- Provider implementations.
- Test artifacts.

The Sub-Project will follow the versioning guidelines defined by the Commonalities Working Group to maintain API versions. 

When a new release for an API is accepted by the Sub-Project and merged into the main branch, the [CAMARA API overview list](https://github.com/camaraproject/APIBacklog/blob/main/documentation/APIbacklog.md) will be updated accordingly.

### Documentation in the CAMARA API Overview List

The **CAMARA API Overview List** is a centralized table used to document all API proposals, their progress, and metadata throughout their lifecycle. It provides transparency and traceability for all stakeholders involved in the CAMARA project.

The overview list is structured with the following columns:

| **Column Name**                                | **Description**                                                                                          |
|------------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **API [Family] Name**                          | The name of the API or API family (e.g., "Messaging API Family").                                         |
| **Supporters in API Backlog Working Group (*API Owner)** | List of companies supporting the API proposal in the Backlog WG. The API owner is marked with an asterisk (*). |
| **API [Family] Proposal Template & Registration Date** | A link to the proposal template filled out during submission and the date it was registered.             |
| **API Backlog & TSC - Status**                 | Current status of the API in the backlog or TSC decision (e.g., "Approved", "Rejected", or "In Progress").|
| **Sub-Project Link & Active Maintainers**      | A link to the Sub-Project repository where the API is hosted and a list of active maintainers.            |
| **Latest Release & Date**                      | Information about the latest release version of the API and its release date.                            |

---

## API Deployment

APIs that have been successfully tested in one or more operator networks can be deployed in live environments.

When an operator (either a CAMARA partner company or an external company) deploys an API definition from a CAMARA API release, it is recommended that this deployment is reported to GSMA for it to be reported in the Open Gateway [live deployment map](https://open-gateway.gsma.com/).

Certification process is followed by GSMA to validate that the deployed API is aligned with the CAMARA specification and guidelines.

---

## Clean-Up

To maintain clarity and relevance in the [CAMARA API overview list](https://github.com/camaraproject/APIBacklog/blob/main/documentation/APIbacklog.md), old entries can be removed under certain conditions:
1. **Old Releases:**  
   Lines for old releases of APIs can be deleted when those releases are no longer deployed anywhere.

2. **Responsible Party:**  
   The responsible Sub-Project is tasked with removing outdated entries from the overview list.

This clean-up process ensures that only actively maintained and deployed APIs are listed, reducing clutter and improving usability.
