#  Agenda and Minutes of CAMARA Technical Steering Committee (TSC) meeting - 2023-10-05

## Invited TSC Participants

* [X] Herbert Damker - (Deutsche Telekom AG) Active Maintainer, TSC chair
* [X] Eric Murray - (Vodafone) Active Maintainer, TSC deputy chair
* [x] Ludovic Robert - (Orange) Active Maintainer, TSC deputy chair
* [ ] Adnan Saleem - (Radisys) End User Council representative
* [X] Chris Howell - (Vonage) Active Maintainer
* [X] Diego González Martínez - (Telefónica) Active Maintainer
* [X] Doug Makishima - (Summit Tech) End User Council representative
* [X] George Glass - TM Forum representative
* [] Henry Calvert - GSMA representative
* [X] Mark Cornall - GSMA representative
* [X] Jan Friman - (Ericsson) Active Maintainer
* [X] Jose Luis Urien - (Telefonica) Active Maintainer
* [X] Kevin Smith - (Vodafone) Active Maintainer
* [] Mahesh Chapalamadugu - (Verizon) End User Council representative
* [X] Shilpa Padgaonkar - (Deutsche Telekom AG) Active Maintainer
* [X] Toshi (Toshiyasu) Wakayama - (KDDI) Active Maintainer

Guest Presenter:

* Casey Cain (Linux Foundation)
* Rebecca Zitha (MTN)

Attendees:
* Tanja De Groot (Nokia)
* Hélène Vigne 


Minutes are available within: [https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC](https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC)

## Agenda

* Introduction
* Introduction by Linux Foundation about upcoming changes regarding project organization and tools
* New API Proposals
  * Device Swap
  * IMEI fraud
  * Site-To-Cloud (not discussed)
* Release Managment for CAMARA & Alignment with Open Gateway
* Request for private repositories (not discussed)
* Backlog of TSC Topics (not discussed)

Please find material for the agenda points below.

## Introduction
Check attendance
Next TSC meeting October 19th
    Room booked in GSMA premise in London
    Registration required for on-site participant
    2 hours meeting


## Introduction by Linux Foundation about upcoming changes regarding project organization and tools (Casey Cain)

Linux Foundation (LF) are working at the request of the CAMARA gouverning board. Following services:
* LF tooling will begin to be use-able by the end of the month (like a Confluence Wiki - preview here: https://docs.linuxfoundation.org/lfx/ but don't edit for now).
* use of LF ZOOM with LF sign-on
  * Need to have a LF id (here: https://openprofile.dev)
  * Change to Zoom will be done for **October 26th and not the 19th meeting**
* Creation of a slack channel: https://join.slack.com/t/camara-project/shared_invite/zt-23bjzwes5-4aLBtE_E1sO0BJhCLBdZVQ
  * This is an optional chanel and not replacing the mailing list


## Involvement of TSC members in Sub Projects

Some answers for TSC members are still missing.
Information is available on the Confluence page here: https://wiki.camaraproject.org/display/CAM/TSC+Members%27+involvement+in+CAMARA+Sub+Projects


## New API

### New API Proposal

* Device Swap (introduced by Rebecca Zitha - MTN)
  * Diego: In which WG this could be tackled ? Is it related to fraud like simswap or device status or new WG ?
  * Shilpa: we need to have categorization
  * Tanja: Name of the family right now is an api name not a family name 
    * --> Mark Cornall: we need wider **technical** category (and not business one)
  * Ludovic: Be aware of the impact of changing family name in our tools
    * Herbert will check with Markus
  * Ask to Rebecca to check if this API could be part of the sim swap family 
    * --> Herbert proposal : have a new family sim and check which API will fit in.
  * Jan raised that we need to think globally on this as this point about gathering API in a family will happen in future (webRTC & clic to dial for example)
  * Eric raises the point that as of today sim swap WG has not minutes.
  * **TSC outcome: No blocking for the API (providing maintainers is welcome) - We need first to solve the family name to launch this API work - This family name issue must cleared for next TSC**
* IMEI Fraud (introduced by Rebecca Zitha - MTN)
  * New Family or put it Device Identifier family ?
    * Eric explained that because the back end will be different it could be a distinct family than the device identifier API
    * Rebecca: it can fit into device identifier family
    * Diego: what are the input of the request ?
      * Rebecca: IMEI
      * Diego: Ok but then how an operator can know as it is a cross operator topic?
    * **TSC Outcome: Ok for the API - This API will be worked in the device identifier API- first request from the TSC to this WG is to discuss the input parameter (IMEI but also other?)**

### Situation for Site-to-Cloud proposal
Not discussed.


## Release Management 
- Thanks to Shilpa we have an issue where all release management points are liste: https://github.com/camaraproject/Commonalities/issues/67 
- Be ready to discus this in London
  

  ## Backlog
* Linux Foundation offers Release Management services and trainings – initial presentation in one of following TSC meetings or in a separate meeting
* [Change Working Groups into Sub Projects #84](https://github.com/camaraproject/Governance/issues/84) 

## AOB


