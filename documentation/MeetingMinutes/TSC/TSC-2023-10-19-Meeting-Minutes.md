#  Agenda and Minutes of CAMARA Technical Steering Committee (TSC) meeting - 2023-10-19

## Invited TSC Participants

* [x] Herbert Damker - (Deutsche Telekom AG) Active Maintainer, TSC chair
* [x] Eric Murray - (Vodafone) Active Maintainer, TSC deputy chair
* [x] Ludovic Robert - (Orange) Active Maintainer, TSC deputy chair
* [x] Adnan Saleem - (Radisys) End User Council representative
* [ ] Chris Howell - (Vonage) Active Maintainer
* [x] Diego González Martínez - (Telefónica) Active Maintainer
* [x] Doug Makishima - (Summit Tech) End User Council representative
* [ ] George Glass - TM Forum representative
* [ ] Henry Calvert - GSMA representative
* [x] Mark Cornall - GSMA representative
* [x] Jan Friman - (Ericsson) Active Maintainer
* [x] Jose Luis Urien - (Telefonica) Active Maintainer
* [ ] Kevin Smith - (Vodafone) Active Maintainer
* [x] Mahesh Chapalamadugu - (Verizon) End User Council representative
* [x] Shilpa Padgaonkar - (Deutsche Telekom AG) Active Maintainer
* [x] Toshi (Toshiyasu) Wakayama - (KDDI) Active Maintainer

Guest Presenter:

* David McBride (Linux Fundation)

Attendees:
*  Sylvain Morel (Orange)
*  Helene Vigue (GSMA)
*  Ivan Izaquirre MArtin (Telefonica)
*  Dinesh Muthukumar
*  Mehdi Jafarizadeh
*  Pierre Close (AT&T)
*  Casey Cain (Linux Fundation)
*  Tanja de Groot (Nokia)


Minutes are available within: [https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC](https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC)

## Agenda

* Introduction
* Release Management (#82) 
* Commonalities & ICM 
    * Alignment around securitySchemes and security of CAMARA API specs
* API Backlog 
    * New proposal for review "Network Insights"
    * Decision on API Family for "Device Swap"
    * Status of Site-to-cloud VPN proposal
* (Further) open issues in https://github.com/camaraproject/Governance/issues
* AOB

Please find material for the agenda points below.

## Introduction

The participation of TSC Members covers well all CAMARA subproject.

## Release Management

A deck was prepared by Ludovic/Herbert (Available within meeting notes folder)

Following points were discussed:

**Discussion on API versioning** – DT proposal to use alpha<n> in API path until and API (major) version is stable
  * Distinction between repostiory release (semantic version as before) and the version shown within API base path
    * A sub project repository can contain one or multiple (closely related) APIs
    * Each API has its own version number which may be different to that of the family release. One of the proposal was that the release could match the most advanced API in sub-project. E.g.: Release 3.0 with API-X in version 3.0, API-Y in version v2alpha1 plus in version v1.0.2, etc)"
    * In addition every API within a sub project will have in the basepath
      * the major version of the API only in case of a **stable** API (e.g. qod/v1)
      * the major version of the API + a postfix alpha or beta, potentially with a number (e.g. qod/v1alpha3 for the third alpha version of an API)
      * (potentially only alpha and stable will be used within CAMARA sub projects)
    * A sub project (release) can contain
      *  multiple APIs with different maturity, e.g. location-verification/v1 and location-retrieval/v1alpha1
      *  multiple versions of the same API, e.g. edge-discovery/v1 (stable) and edge-discovery/v2alpha1
    * sub project release will remain with 0.x until first API reaches stable v1. E.g.: A release v0.1 may include an API in v1alphaX
    * Released APIs with the same base-path will contain only non-breaking changes (are backward-compatible)
    * The version number of the sub project release allows to identify the changes between two releases of an API with the same base path   
  * **[Action]** Herbert will provide rules of management for this proposal
  * The family version should also be considered – will be included in DT Proposal
    * Note: Concept of family of API – This is not relevant for all API project but only when an API project has more than one API. The Family concept is confusing for Open Gateway product Stream and should be reconsidered, potentially renamed.

David from Linux Fundation presented on **Linux Fundation release management support service**
  * LF offers service to support release management. 
  * This service is part of the support we get in CAMARA from LF. 
  * Probably the best way to move forward is to have 2/3 people from CAMARA attending LF training on this topic and 

Agreement on **providing a conformance profile** to describe minimum requirement for a given implementation.
    * **[Action]** Test will be done on Device location API.
    * This conformance profile will be shared and looped with GSMA Open gateway product & technical stream.

## Commonalities & ICM

**Update OpenAPI security guideline** (https://github.com/camaraproject/Commonalities/pull/57)
*	Agreement to use openId connect discovery clause in the Open API Specification (OAS) and provided API scheme for the API in another form (either in seperate file or as documentation section within the OAS).
*	Documentation must also list possible security schema for the APIs. 
  * **[Action]** Telefonica will propose a wording.
*	We need also to check how security schema are managed in 3GPP
  *	Tanja De Groot provided following links: [3GPP 5G APIs](https://forge.3gpp.org/rep/all/5G_APIs), esp. [TS29122_CommonData.yaml](https://forge.3gpp.org/rep/all/5G_APIs/-/blob/REL-18/TS29122_CommonData.yaml)
  *	Shilpa added the following specific link: [TS24558_Eees_EASDiscovery.yaml](https://forge.3gpp.org/rep/all/5G_APIs/-/blob/REL-18/TS24558_Eees_EASDiscovery.yaml)
* **Voting in Commonalities and ICM groups**:  as their decisions affect many other working groups, discussions needing a voting should be escalated to TSC.

## New API

### New API Proposal

Green light for **Device Swap API**
  * As of now Device Swap will be managed in an own CAMARA subproject
  * **[Action]** API Backlog to provide proposed list of initial maintainers to TSC (as agreed in last TSC)
  * **[Action]** CAMARA Admin: Create new sub project

Green light for **Network Insight API**
  * **[Action]** Request to API Backlog to find a more specific and understandable API name for Network Insight API (see discussion within API Backlog issue)
  * **[Action]** API Backlog to provide proposed list of initial maintainers to TSC
  * **[Action]** CAMARA Admin: Create new sub project

Still no progress on **Site-to-Cloud API** (not clear about the demarcation with TMF work on this topic)

## (Further) open issues in https://github.com/camaraproject/Governance/issues

Only partly discussed.

* [Handling of private repos #83](https://github.com/camaraproject/Governance/issues/83)
  * Decision was taken within TSC on Sept 21st that there will be no private repositories in CAMARA hosted
  * Eric proposed to archive the exisitng private repository Anonymised Subscriber Identifier. Functionality to be reconsidered if there is a request from OGW product team.
  * The proposal was accepted.

## AOB

The meeting of 2 hours was considered as very productive. The participants agreed to extend further TSC meeting from 1 hour to 2 hours.

The next TSC meetings would be according to the schedule on:
  * Nov 2nd (first Thursday)
  * Nov 16th (third Thursday)
  * Dec 7th (first Thursday)
  * Dec 21st (third Thursday)
  * Jan 4th (first Thursday)
  * Jan 18th (third Thursday)
Decision which meeting will be skipped as end-of-year break will be taken later.
