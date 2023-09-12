# API onboarding and management in CAMARA

## Introduction

This document aims at describing a clear, consistent and transparent process for the onboarding (submission) and management (maintenance) of API proposals and APIs in the CAMARA Project.

The process pipeline is depicted in the figure below.

![API process pipeline](images/API_process_pipeline.png)

All stages within this process pipeline are documented in the CAMARA API overview list. An example can be seen here:

![API process pipeline](images/API_overview_list.png)

This is only a draft for the overview list, the real overview list shall be implemented based on HTML so that changes can be tracked easily. Details and clarifications on the stages conforming this pipeline are provided in the following sections.

## Submission of an API proposal

The pipeline is triggered with the submission of an API proposal. This API proposal can represent a new API or a new API family.

API proposals can be submitted by everybody, including OPAG (GSMA Open Gateway), CAMARA member companies, and existing CAMARA Sub Projects or Working Groups (if these realize that the scope has to be increased). 

To proceed with the submission, the API owner shall follow these steps:

- Fill in the template available [here](https://github.com/camaraproject/WorkingGroups/blob/main/Commonalities/documentation/API-proposal-template.md) and save it with the following name: "APIproposal\_\<APIname\>\_\<owner\>. md" locally.
- Create a new issue in the API Backlog Working Group repository, labeled with "API Backlog".
- Upload the filled-in template to [GitHub repository folder for API proposals](https://github.com/camaraproject/WorkingGroups/tree/main/APIBacklog/documentation/SupportingDocuments/API%20proposals) via Pull Request. This Pull Request shall be associated to the issue created in the previous step.

## Evaluation of the API proposal

Upon submission, the following steps are executed in "API Backlog" Working Group (WG):

1. The WG chair checks that the template is duly filled in. Otherwise, the API owner is requested to provide missing information.
2. Each company analyses the API proposal, and decides whether it wants to support it. If a company wants to become supporter, the company name needs to be included in the "Supporters in API Backlog Working Group" column for that API. The WG participant representing that company will do this by submitting a Pull Request against the [API backlog](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md). </br>NOTE: The more support an API proposal gets, the better (it may get more traction).
3. When the API owner considers the API proposal is in good shape to go for approval, it informs the WG chair accordingly.
4. Upon receiving this information, the WG chair merges the original Pull Request into the main branch, and sends the API proposal to the Technical Steering Committee (TSC) of CAMARA. This action shall be completed at least one week prior to the TSC meeting where the API proposal will be voted upon. 

The whole procedure (steps 1-4) should be done within 2 regular meetings of the API Backlog WG. Nonetheless, it is up to the API owner to decide if it wants to shorten or extend this time period. 

In parallel, the API proposal is formally registered in CAMARA by adding it to the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md) The WG chair creates a new line in the table and fills in API family name, API family owner, API family proposal registration date, the link to the application template and the supporters for it.

## TSC decision on API proposal

Upon receiving the API proposal and notification from the WG chair, the TSC studies the proposal and votes it at the TSC meeting.

- **Not Accepted**: The API proposal is rejected and will not be included in any API Sub Project, and shall either (1) be removed from the API Backlog, with objecting companies to provide justifications why, or (2) returned to the API Backlog, with the TSC including in the 'justications' section the  clarifications required/gaps to be addressed/corrections required in order for the API to be re-submitted by the API supporters.
- **Accepted** In this case, the TSC shall specify whether the API proposal is to be hosted by a new or existing Sub Project.

Main tenets for TSC voting:

- Tenet #1: Open-source projects are contribution-driven. There should be no guidelines to prevent partners to contribute. If a company would like to work on a certain API proposal they should be welcome to do it.
- Tenet #2: The TSC shall make sure that APIs belonging together (close topic/content, API families) are developed within the same Sub Project, while ensuring that Sub Projects are not too small (difficult to track them down) or too big (difficult to be managed). There should be only one API for each purpose.
- Tenet #3: There could be situations where API proposal complies with acceptance criteria (template duly filled out) but has not supporters other than the proponent company. What to do in this situation? Recommendation is to accept the API proposal and see how successful it will be in terms of industry adoption.

The TSC may also propose changes to an API proposal and take the decision considering these changes. The TSC documents the decision in the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md) (fills in columns TSC date and TSC decision / Sub Project; in case of a No-Go "Rejected" is documented there).

## API management and maintenance

In case of a GO decision of the TSC the named Sub Project takes over responsibility for the new API or API family and starts making contributions for the API definition(s), API documentation, provider implementation and test artefacts.

The Sub Project will follow the versioning guidelines as defined in the Commonalities Working Group to maintain the API versions. Based on an internal consensus within the Sub Project, releases will be cherry-picked and release branches will be appropriately created. If a deliverable (API definition, API documentation, API code, successful test) for a release of an API is available (accepted by the Sub Project and merged in the main branch) the Sub Projects adds the link to it in the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md).

If there are more than one API in an API family / API Sub Project for each of them a separate line in the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md) shall be added.

If there are more than one releases for an API for each of these releases a separate line in the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md) shall be added. It is target only to have 3 releases for one API at the same time: one in development and two in production.

If there are more than one provider implementations for one release for an API for each of these provider implementations a separate line in the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md) shall be added.

The requested data to be filled in the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md) is API name, API release, link to API definition, link to API documentation, link to API code and partner which has tested an API release.

## API deployment

If an API is successfully tested in one or more operator networks, it can be used for deployment also in live environments.

In case an operator (CAMARA partner company or external company) uses an API definition of a CAMARA API release, this operator is recommended to document it in the last column (API deployed at company and country) of the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md). If possible, also a link to the site (e.g. portal) where the deployed API can be accessed is recommended to be inserted.

## Clean up

Lines for old releases of APIs (when these aren't deployed anywhere anymore) in the [CAMARA API overview list](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIBacklog.md) can be deleted by the responsible API Sub Project.
