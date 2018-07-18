<img src="https://www.nga.mil/Partners/PublishingImages/720px-US-NationalGeospatialIntelligenceAgency-2008Seal.svg.png" width="200" style="margin: 20px;" />

# National Geospatial-Intelligence Agency (NGA)

## Moving Target Indicator (MTI) Software Modernization

## Request for Quote (RFQ) - NTIAG18179AS49

## eBuy RFQ: RFQ1306427
	
**July 17, 2018**

## Background

The National Geospatial-Intelligence Agency intends to retire its current traditional data center and replace it with a cloud-based computing environment. This necessitates migrating motion imagery data — MTI, Video, Wide Area Motion Imagery, and the associated operational capabilities — to the cloud.

## Instructions

### Submission of Proposals

The NGA is soliciting proposals in response to this Moving Target Indicator (MTI) Software Modernization Request for Quote (RFQ).  Please submit your quotation in accordance with all instructions specified in the attached RFQ document, specifically section 8.0 of the RFQ, the terms and conditions of your GSA Schedule Contract, and the prices contained therein. Please ensure that your response includes all requested information and that your technical response clearly demonstrates your company’s capability to perform the objectives in the SOO.  

Please submit questions to either the GitHub Repository or to eBuy RFQ1306427 by the due date below. Quotes shall also be submitted to GSA eBuy RFQ1306427 on or before the time specified below. Any quote received after this date and time shall be rejected. Any quote not received through eBuy shall be rejected.

### Timeline

These are the milestones provided for this solicitation:

|No. |	Due Date | Acquisition Event|
| --- | --- | --- |
|**1**	| 17JUL18 |	Solicitation released|
|**2**	| 20JUL18 by 1700EST | Questions due|
|**3**	| 23JUL18 by 1700EST | Letters of Intent|
|**4**	| 31JUL18 by 1700EST | Quotes due (Technical and Price)|
|**5**	| TBD |	Award decision|



## Contents

1. [Request for Quotes (RFQ)](00_RFQ.md)
2. Attachment 01: [Statement of Objectives (SOO)](01_SOO.md)
3. Attachment 02: [Quality Assurance Surveillance Plan (QASP)](02_QASP.md)
4. Attachment 03: [Pricing Template](03_Pricing_Template.xlsx) (Excel file)
5. Attachment 04a: [Available AWS Environment Services & Tools](04a_AWS.md)
6. Attachment 04b: [MTI Backlog](04b_Backlog.md)
7. Attachment 05: [Clauses & Provisions](05_Clauses_and_Provisions.pdf)

Additionally, [all contents can be downloaded as a single PDF](RFQ_Complete.pdf).


## STANAGs

This RFQ cites two “STANAGs,” or NATO STANdardization AGreements, that this work relies on: STANAG 4607 and STANAG 4676. These function like ISO or ANSI standards, but are instead promulgated by the North Atlantic Treaty Organization. There are [STANAGs on many topics](http://nso.nato.int/nso/nsdd/listpromulg.html), some technical, most not. The work here requires parsing both of these STANAG file formats.

### STANAG 4607
4607 defines the NATO [Ground Moving Target Indicator](https://en.wikipedia.org/wiki/Moving_target_indication) (GMTI) format—radar, basically. The NATO Standards Office publishes both [the standard itself](http://nso.nato.int/nso/zPublic/stanags/CURRENT/4607Eed03.pdf) and [an implementation guide](http://nso.nato.int/nso/zPublic/ap/aedp-7(2).pdf). MITRE publishes [an interesting history](https://www.mitre.org/sites/default/files/pdf/05_0164.pdf) of how the 4607 standard came to be. To get an idea of what it looks like to interact with GMTI [see this open source GMTI library](https://github.com/pentlandedge/s4607), [these open source GMTI utilities](https://github.com/pentlandedge/s4607_extra), or [this Leaflet-based GMTI viewer](http://www.hawkstream.net/), which includes sample data.

### STANAG 4676
4676 is the NATO Intelligence, Surveillance and Reconnaissance Tracking Standard, establishing the standard for tracking the location and spatial movement of mobile objects and associated motion imagry. [The standard](http://nso.nato.int/nso/zPublic/ap/AEDP-12(A)V1.pdf) defines an XML schema.


## Public domain

This project is in the [public domain](LICENSE).

