# CAMARA Technical Steering Committee (TSC) meeting - 2023-09-07

## Invited TSC Participants

* [x] Herbert Damker - (Deutsche Telekom AG) Active Maintainer, TSC chair
* [x] Eric Murray - (Vodafone) Active Maintainer, TSC deputy chair
* [x] Ludovic Robert - (Orange) Active Maintainer, TSC deputy chair
* [ ] Adnan Saleem - (Radisys) End User Council representative
* [x] Chris Howell - (Vonage) Active Maintainer
* [x] Diego González Martínez - (Telefónica) Active Maintainer
* [x] Doug Makishima - (Summit Tech) End User Council representative
* [x] George Glass - TM Forum representative
* [x] Henry Calvert - GSMA representative
* [x] Jan Friman - (Ericsson) Active Maintainer
* [x] Jose Luis Urien - (Telefonica) Active Maintainer
* [x] Kevin Smith - (Vodafone) Active Maintainer
* [ ] Mahesh Chapalamadugu - (Verizon) End User Council representative
* [ ] Shilpa Padgaonkar - (Deutsche Telekom AG) Active Maintainer
* [x] Toshi (Toshiyasu) Wakayama - (KDDI) Active Maintainer

Minutes are available within: [https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC](https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC)

## Agenda proposal

* Introduction
* Way of working within TSC
* F2F/hybrid Meeting Oct 19th in London?
* New API Proposals
  * Click to Dial
  * KYC Match
  * KYC Fill-in
  * Site-to-Cloud VPN
  * WebRTC
* Notification pattern - request for feedback from Commonalities WG
* Release Managment for CAMARA & Alignment with Open Gateway
* Request for private repositories
* Backlog of TSC Topics

Please find material for the agenda points below.


## Introduction

* Check attendance of TSC participants
* TSC Agreed on proposed agenda

## Way of Working of the TSC

Just as reminder:

* [Responsibilities of the TSC](https://github.com/camaraproject/Governance/blob/main/ProjectCharter.md#:~:text=The%20TSC%20is%20responsible%20for%20all%20aspects%20of%20oversight%20relating%20to%20the%20Project) are defined within the [Project Charter](https://github.com/camaraproject/Governance/blob/main/ProjectCharter.md). 
* The meetings are publically announced in the project Governance README.md. The Chair has send invitation to the TSC participants (reach out to Herbert if you need the invitation again)
* Rules for decision making (voting) are also defined in the [Project Charter](https://github.com/camaraproject/Governance/blob/main/ProjectCharter.md)

Proposal:

* As long as we don't have a proper wiki available, the proposal for agenda drafts and MoM is the following (similar to the practice in the sub projects):
  * Agenda will be announced via a draft pull request within the CAMARA Governance repo. The link will be sent to the TSC mailing list and a list of the agenda points
  * Minutes will be captured by the Co-Chairs or a volunteering TSC participant. The draft minutes will be made available as a pull request within the CAMARA Governance repo. They will be reviewed in minimum by the Chair or one of the Co-Chairs. TSC participants can provide corrections as reviews. The minutes will be merged after one week as agreed.
  * ...

Proposal:

* Communication tools are 
  * Github (issues, minutes, ...)
  * Email list tsc@lists.camaraproject.org (especially for the purposes defined within the project charter)
  * In addition it is consider to have a Slack instance for CAMARA as a more agile communication channel. It will be part of the community management by LF and can be used by all sub projects
* ...

Discussion/Decisions:

* No comment from the audience --> **Herbert Proposal accepted.**

## TSC F2F/hybrid Meeting Oct 19th in London?

GSMA OPG, OPAG and Open Gateway have f2f meetings in London in the week of October 16th to 20th. 
Should we aim to have a colocated (hybrid) TSC meeting on Thursday, 19th, 16:00 CEST / 15:00 BST?
(note: on Oct 20th is the OGW hybrid meeting)

Discussion/Decisions:
  * Henry Calvert (GSMA) welcomes the idea 
  * (**Action**) Henry will check if it is possible to book a room for this.
 * We need to have an idea of who we will come - probable attendees: Shilpa, Herbert, Ludovic, Diego, Doug, Jan, José Luis



## API Backlog: Decision about five (5) new API proprosals

José A. Ordóñez Lucena asks on behalf of the working group API Backlog the TSC to decide about the following five (5) new API proposals:
* Click to Dial
* KYC Match
* KYC Fill-in
* Site-to-Cloud VPN
* WebRTC

Details are available in the material in the message sent by Jose on Sept 1st: https://lists.camaraproject.org/g/tsc/message/20 

Proposal: 
* TSC participants can raise objections and nominate initial maintainers for the new API subprojects on the TSC mailing list
* The supporting organizations should nominate their initial maintainers (AP: Jose) also until then

Discussion/Decisions:

  * Herbert reminded 'rules of engagement' for new api proposal management - if no objections, the TSC pronounces GO for the API proposal.
  * José Antonio Ordoñez Lucena reminded to the team the process in API Backlog project
    * Chris Howell asks if there is a guideline to make decision
    * José provides 3 recommendation:
      * Check if the API did no conflict with OPG service/CAMARA API
      * Be sure to keep a good balance about workload for the team 
      * Be sure to have enough supporters for the API (if not, TSC could ask for more time to encourage to get more supporter)

  * Herbert asked to the tean if any member has objections to take decision today --> no objection

  * New API decision:
    * Click to Dial: No objection - Go  
      * (Action) Henry Calvert (GSMA) will try to get more supporter for this API (and get in touch with China Mobile)
      * Jan Friman (Ericsson) indicated that Ericsson will probably ask to be part of the maintainers
      * (Action) TSC has to request Chinal Mobile & Huawei to nominate Maintainer
    * KYC Match: No objection - Go  
    * KYC Fill: No objection - Go  
      * TSC proposal is to have separate API but tackled in a same (Working Group) WG within a same API family - Toshi as API proposal owner agreed.
      * (Action) Working group or API backlog team has to provide a name for this WG (like customer Data as suggestd by Herbert)
      * (Action) : TSC has to provide maintainers name (Toshi)
    * Site-To-Cloud: clarification requested
      * Possible collision with work done in TMF
      * George Glass mentions that AT&T will showcase in TMF a catalyst on same topic.
      * * (Action) TSC asks to China Mobile to clarify this API scope with current work done by AT&T & Check if AT&T could be a supporter of the API
    * WebRTC: no objection - Go
      * TSC request the (future) WG in charge of this API to check possible collision with WebRTC standard.
      * (Action) : TSC has to provide maintainers name (TEF)



## Commonalities: Notification pattern - request for feedback

Ludovic Robert will present the current status of discussions about Notification patterns (Issue #44, PRs #56 and #43) in Commonalities. The notification topic is open for a long time and several sub project are waiting for the outcomes.

Proposal:
* Request for action to review and provide feedback on PR #56

Discussion/Decisions:
* Ludovic quickly went through the proposal and in particular the alignement with CloudEvents standard.
* The proposal is documented in the Design Guideline
* (Action) We encouraged member to provide feedback on PR#56 (here: https://github.com/camaraproject/Commonalities/pull/56)
*  (Action) Ludovic has to provide update on this topic for next TSC meeting.


## Release Management for CAMARA & Alignment with Open Gateway

See discussion and input within [Define Release Management for CAMARA #82](https://github.com/camaraproject/Governance/issues/82), especially the presentation attached within Helene Vigue's comment: [Open Gateway Product WS _ Ways of Working with CAMARA Proposal [1].pptx](https://github.com/camaraproject/Governance/files/12525953/Open.Gateway.Product.WS._.Ways.of.Working.with.CAMARA.Proposal.1.pptx)

Discussion/Decissions:
* We need a WG to work on this topic
  * Herbert will craft a proposal for next meeting on this topic
* Helene Vigue/ Henry Calvert provided GSMA feedback:
  * GSMA is the 'front end' to identify & provide new API requirements
  * GSMA process needs to fit in with CAMARA new api proposal. 
  * GSMA needs to have some clarity on CAMARA work & deliverables fulfillment
  * (Action)) We need to work together.



## Request for private repositories

Henry Calvert and/or Helene Vigue will present the need for a private repository for a Scam Signal API (note: not yet an API Proposal in API Backlog)

See also https://github.com/camaraproject/Governance/issues/83

* The TSC needs to decide if and how private repositories could and will be supported in CAMARA

Discussion/decision:
* ...

## Backlog of TSC Topics

* Relation of TSC with its working groups and sub projects
  * The following working groups and sub projects are currentlly working on overarching topics and should be therefore according to the project charter supervised by the TSC:
    * API Backlog
    * Commonalities
    * Identity & Consent
  * Related issue: [Change Working Groups into Sub Projects #84](https://github.com/camaraproject/Governance/issues/84) 
* [Process to publish v1.0 of an API](https://github.com/camaraproject/Governance/issues/85) 
* ...


## AOB
