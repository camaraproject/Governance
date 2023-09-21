#  Agenda and Minutes of CAMARA Technical Steering Committee (TSC) meeting - 2023-09-07

## Invited TSC Participants

* [x] Herbert Damker - (Deutsche Telekom AG) Active Maintainer, TSC chair
* [x] Eric Murray - (Vodafone) Active Maintainer, TSC deputy chair
* [x] Ludovic Robert - (Orange) Active Maintainer, TSC deputy chair
* [ ] Adnan Saleem - (Radisys) End User Council representative
* [ ] Chris Howell - (Vonage) Active Maintainer
* [x] Diego González Martínez - (Telefónica) Active Maintainer
* [x] Doug Makishima - (Summit Tech) End User Council representative
* [x] George Glass - TM Forum representative
* [x] Mark Cornall - GSMA representative
* [x] Jan Friman - (Ericsson) Active Maintainer
* [x] Jose Luis Urien - (Telefonica) Active Maintainer
* [x] Kevin Smith - (Vodafone) Active Maintainer
* [x] Mahesh Chapalamadugu - (Verizon) End User Council representative
* [x] Shilpa Padgaonkar - (Deutsche Telekom AG) Active Maintainer
* [x] Toshi (Toshiyasu) Wakayama - (KDDI) Active Maintainer

Guest Presenter:

* Markus Kümmerle (Deutsche Telekom (AG)

Minutes are available within: [https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC](https://github.com/camaraproject/Governance/tree/main/documentation/MeetingMinutes/TSC)

## Agenda

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
* Request for private repositories (not discussed)
* Backlog of TSC Topics (not discussed)

Please find material for the agenda points below.

## Introduction
Check attendance
TSC meeting October 19th
    Room booked in GSMA premise
    Registration required for on-site participant
    2 hours meeting


## Updates from Gouvernance Board/Director Fund

Announcement of CAMARA directed fund at LF Open Source Summit
Chair & Tresorer have to be elected for the gouvernor board.
Next steps is to decide how fund will be use.

## New API

### Nomination of initial maintainers for the three new sub projects

* Click to Dial
* Know Your Customer
* WebRTC

We have a list of maintainers. 

| subproject| Maintainers|
| ----------|------------|
| Clic-to-Dial<br>China Mobile is the owner| Hanbai Wang (@HanbaiWang) for China Mobile<br>Shuting Qing (@ShutingQing) for Huawei<br>Dan Xu (@DanXu-ChinaTelecom) for China elecom|
| Know Your Customer<br>KDDI is the owner| Toshi Wakayama (@ToshiWakayama-KDDI) and Tetsuya Chiba (@tcchiba) for KDDI<br>Gilles Renoux (@GillesInnov35) for Orange <br>Efthymis Isaakidis (@EfthymisIsaakidis-DTCS) for DT <br>Fernando Prado (@fernandopradocabrillo) for Telefonica<br>Dan Xu (@DanXu-ChinaTelecom) for China Telecom|
|WebRTC<br>Telefonica is the owner| Ricardo Serrano (@TEF-RicardoSerr) for Telefonica<br>Pradeep Achar (@pradeepachar-mavenir) and Sushanth Hegde (@sushanthmavenir) for Mavenir<br>Benjamin Busvel (git to be created) for Orange<br>Jesus Pedruelo (@jesus-pb) and Ratna Ratnanandan (@ratnavf) for Vodafone<br>Deepak Jaiswal (@deepakjaiswal1) for T-Mobile US|

**[Action for Jan]** Ericsson will provide maintainers for Click-to-Dial & WebRTC.

No objection from the TSC for the provided list.

### Name for API family with KYC Match and KYC Fill-in as APIs

'Know Your Customer' is the name agreed by the project group & TCS

### Situation for Site-to-Cloud proposal
Proposal unchanged but discussion between both CAMARA & TMF proposal occurred in the CAMARA git.

We need to have another round of discussion and in particular a statement of the TM Forum for this API.

Pierre Close (AT&T) explained the scope of the TMF API proposal and ask to be involved in the discussion and will reach AT&T involved (for reference[ #271](https://github.com/camaraproject/WorkingGroups/issues/271))


## Private repositories in CAMARA

**Scam Signal**

Update from GSMA on the request for a private repository for Scam Signal
See also https://github.com/camaraproject/Governance/issues/83

- Mark Cornall explained the decision: The private repo will be hosted under GSMA OPAG or Open Gateway directory with limited access & visibility. A specific 'join-in' process wil be triggered to accept people in the group with some legal stuff to agreed.

- Diego asked if CAMARA design rules will be followed in a GSMA API crafted?
  - Mark answered **YES** ! 
  

**Anonymised Subscriber Identifier** discussion: 
- Eric raised the point about the other private topic which is Anonymised Subscriber Identifier. Does this repo should stay in CAMARA? Shilpa thinks this is not a good idea to have private repo in CAMARA as API work will be mentionned in TSC meeting for example which are public available. George raised same arguments to ease TMF contribution
- For the API Anonymised Subscriber Identifier the issues is about the name (Anonymised has a sensitive meaning) and the legal impact of this API (People has not to think that Telco are providing identifier without their consent). 
- Action: Open an issue in API backlog.


## Commonalities

### Way of working Commonalities/TSC

- Shilpa raised the point that we need to find a way to work quickly betwen Commonalities & TSC.
- Shilpa proposal is for specif topic to select people from subproject and inform TSC about a specific work. For next Commonalities meeting Shilpa will list the topics where we need partcipation and bring this list to TSC.

- Diego asked is vote will still be at subproject level or at TSC level?
  - Current gouvernance precise that today the vote is first at subproject and then at TSC level.

### Notification pattern

Almost there - No major points highlighted by Ludovic. 
Now it's time to review and approve if not **blocking** point.



## 	Identify & Consent Management (ICM)
- Way of working ICM/TSC/sub projects
  - especially decisions about Security Schemes


## Release Management 
- See issue https://github.com/camaraproject/Governance/issues/82 for an initial scope of the  discussion
  - As of now all projects are v0.x
- Linux Foundation offers Release Management services and trainings – initial presentation in one of following TSC meetings or in a separate meeting?
    - Proposal to have an extra meeting - not a TSC one as it required 30 minutes.
  


## Other topic

Kevin brings the topic of management of automatic testing of the API. Kevin will prepare a presentation for test TSC.

## --> Action for all

**[Action for all]** Provided a list of subproject where TSC member are involved to be sure we have no subproject representation missing.

## Backlog of TSC Topics (not discussed)



