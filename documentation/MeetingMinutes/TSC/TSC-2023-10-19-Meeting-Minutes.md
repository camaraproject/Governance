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

* X from Linux Fundation

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
•	(Further) open issues in https://github.com/camaraproject/Governance/issues


Please find material for the agenda points below.

## Introduction

The participation of TSC Members covers well all CAMARA subproject.


## Release Management

A deck was prepared by Ludovic/Herbert/Shilpa.

Following points were discussed:

**Discussion on API versioning** – DT proposal to use alpha in API path.
  * Add an Alpha or Beta prefix to pre-released APIs and then increment the release version when backwards compatibility is broken.
  * [Action] Herbert will provide rules of management for this proposal
  * The family version should also be considered – will be included in DT Proposal
    * Note: Concept of family of API – This is not relevant for all API project but only when an API project has more than one API. The Family concept is confusing for Open Gateway product Stream

X from Linux Fundation mades a presentation on **Linux Fundation release management service**
  * LF offers service to support release management. 
  * This service is part of the support we got. 
  * Probably the best way to move forward is to have 2/3 people from CAMARA attending LF training on this topic and 


Agreement on **providing a conformance profile** to describe minimum requirement for a given implementation.
    * [Action] Test will be done on Device location API.
    * This conformance profile will be share and looped with GSMA Open gateway product & technical stream.



## Commonalities & ICM

**Update OpenAPI security guideline** (https://github.com/camaraproject/Commonalities/pull/57)
*	Agreement to use openId connect discovery clause in the swagger and provided API scheme for the API in another file.
*	Documentation must also list possible security schema for the APIs. 
        * [Action] Telefonica will propose a wording.
*	We need also to check how security schema are managed in 3GPP --> Tanja De Groot provided links: xxxxx



## New API

### New API Proposal

Green light for **Device Swap API**
  * As of now Device Swap will be managed in an own CAMARA subproject

Green light for **Network Insight API**
  * Request to find a more understandable API name for Network Insight API

Still no progress on **Site-to-Cloud API** (no clear about the demarcation with TMF work on this topic)

### Existing API

Update on Anonymised Subscriber Identifier API. Eric indicated that the Repository is now private in CAMARA.
