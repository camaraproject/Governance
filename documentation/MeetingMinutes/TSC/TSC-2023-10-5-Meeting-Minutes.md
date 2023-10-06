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
* [x] Henry Calvert - GSMA representative (partly)
* [X] Mark Cornall - GSMA representative (standin for Henry Calvert)
* [X] Jan Friman - (Ericsson) Active Maintainer
* [X] Jose Luis Urien - (Telefonica) Active Maintainer
* [X] Kevin Smith - (Vodafone) Active Maintainer
* [ ] Mahesh Chapalamadugu - (Verizon) End User Council representative
* [X] Shilpa Padgaonkar - (Deutsche Telekom AG) Active Maintainer
* [X] Toshi (Toshiyasu) Wakayama - (KDDI) Active Maintainer

Guest Presenter:

* Casey Cain (Linux Foundation)
* Rebecca Zitha (MTN)

Further attendees (not complete):
* Tanja De Groot (Nokia)
* Hélène Vigne 

Minutes are available within: [https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC](https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC)

## Agenda
* Introduction
* Upcoming community tools for CAMARA (LF, Casey Cain)
* Involvement of TSC members in Sub Projects
* API Backlog
  * New proposals IMEI Fraud & Device Swap
  * Status of Site-to-cloud VPN proposal
* Release Management (#82)
* Commonalities Updates (not discussed)
* Identity & Consent Updates (not discussed)
* Backlog


## Introduction
* Check attendance (see above check marks)
* Next TSC meeting October 19th, 16:00 CEST / 15:00 BST
  * Room booked in GSMA premise in London
  * Registration required for on-site participant (see [message from Mark about invite for hybrid F2F meeting in London](https://lists.camaraproject.org/g/tsc/message/39)) 
  * Start at regular time (16:00 CEST, 15:00 BST), duration 2 hours

## Introduction by Linux Foundation about upcoming changes regarding project organization and tools (Casey Cain)

Linux Foundation (LF) are working at the request of the CAMARA gouverning board. Following services:
* LF tooling will begin to be use-able by the end of the month (preview on tooling here: https://docs.linuxfoundation.org/lfx/ but don't edit for now).
* Wiki within setup, please don't edit yet ([https](https://wiki.camaraproject.org/))
* We will use ZOOM meetings with LF sign-on
  * Need to have a LF id (here: https://openprofile.dev)
  * Change to Zoom will be done for **October 26th and not the 19th meeting**
* Creation of a slack workspace: https://join.slack.com/t/camara-project/shared_invite/zt-23bjzwes5-4aLBtE_E1sO0BJhCLBdZVQ
  * This is an optional, additional communication channel and not replacing the mailing list

## Involvement of TSC members in Sub Projects

* Some answers for TSC members are still missing
* Information is available on the Confluence page here: https://wiki.camaraproject.org/display/CAM/TSC+Members%27+involvement+in+CAMARA+Sub+Projects
* **Please send the remaining information to Herbert per mail**


## API Backlog

### New API Proposals
* Device Swap (introduced by Rebecca Zitha - MTN)
  * Diego: In which WG this could be tackled ? Is it related to fraud like simswap or device status or new WG ?
  * Shilpa: we need to have categorization of APIs
  * Tanja: Name of the family right now is an api name not a family name 
    * --> Mark Cornall: we need wider **technical** category (and not business /use case driven one)
    * --> Tanja: resource based categorizatiion could be a sustainable way forward (e.g. Device Swap provides information about SIM)
  * Ludovic: Be aware of the impact of changing family name in our tools
    * Herbert will check with Markus
  * Ask to Rebecca to check if this API could be part of the sim swap family 
    * --> Herbert alternative proposal: have a new family sim and check which API will fit in.
  * Jan raised that we need to think globally on this as this point about gathering API in a family will happen in future (webRTC & clic to dial for example)
    * Herbert to check also the consequences to move APIs between repositories
  * Eric raises the point that as of today sim swap sub project has no minutes
  * Henry agrees that the families and categories should be  proposed before the API request / proposal is submitted to CAMARA Backlog, should not be TSC work. CAMARA Form needs updating, GSMA will take this action
  * **TSC outcome: No blocking for the API - but we need first to solve the family name to launch this API work - This family name issue must cleared for next TSC**
    * **Action to APIBacklog WG** to nominate already the initial maintainers (so that the repo can be setup immediately after the decision about family name  
* IMEI Fraud (introduced by Rebecca Zitha - MTN)
  * New Family or put it Device Identifier family?
    * Eric explained that because the back end will be different it could be a distinct family than the device identifier API
    * Rebecca: it can fit into device identifier family
    * Diego: what are the input of the request?
      * Rebecca: IMEI
      * Diego: Ok but then how an operator can know as it is a cross operator topic?
  * **TSC Outcome: API proposal accepted - This API will be worked out in the device identifier sub project - first request from the TSC to this sub project is to discuss the input parameter (IMEI but also other?)**

### Situation for Site-to-Cloud proposal
Not discussed.

## Release Management ([#82](https://github.com/camaraproject/Governance/issues/82))
- Thanks to Shilpa we have an issue where all release management points within Commonalitites WG are listed: https://github.com/camaraproject/Commonalities/issues/67 
- **Action** Please add your support to the issue and be ready to discuss this in London  

## Backlog
* Linux Foundation offers Release Management services and trainings – initial presentation in one of following TSC meetings or in a separate meeting
* [Change Working Groups into Sub Projects #84](https://github.com/camaraproject/Governance/issues/84) 

## AOB


