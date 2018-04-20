# National Geospatial-Intelligence Agency (NGA)

# Moving Target Indicator (MTI) Software Modernization

## Request for Proposal (RFP) DRAFT

**April 6, 2018**

## 1.0 PURPOSE

The National Geospatial-Intelligence Agency (NGA), Office of Contract Services (OCS), hereby issues this Request for Proposal (RFP) to procure services in support of the attached Statement of Objectives (SOO). This solicitation will be accomplished using the terms and conditions of the RFP and of the Offeror’s Master Contract under the GSA Federal Supply Schedule (FSS) contract, Schedule 70, General Purpose Commercial Information Technology Equipment, Software, and Services, under Special Item Number (SIN) XXX XX, insert here.

## 2.0 BACKGROUND

NGA intends to retire its current traditional data center and replace it with a cloud-based computing environment. This necessitates migrating motion imagery data - MTI, Video, Wide Area Motion Imagery, and the associated operational capabilities to the cloud.

## 3.0 SCOPE AND OBJECTIVES

_Develop capabilities to ingest, discover, retrieve and visualize MTI data (STANAG 4607, STANAG 4676, and mission data) in the cloud across multiple security domains._

### 3.1 BACKLOG

**3.1.1 STANAG 4607** - Adopt, adapt, or build open services to be exposed or consumed in a cloud-based enterprise for the processing of STANAG 4607 data and data types for the purpose of:

**3.1.1.1 Ingest:** receive data via multicast protocols - ingest both streaming and file based data -  ingest STANAG 4607 formats 1,2, &amp; 3 - ingest up to 1TB/day of MTI data - support search, discovery, retrieval of MTI data;

**3.1.1.2 Catalog:** all source &amp; MTI data - maintain metadata integrity - retain metadata as long as the source data - maintain modifications to metadata - maintain metadata at appropriate classification level and associate it at any classification level - support search, discovery, retrieval, and visualization of MTI;

**3.1.1.3 Discovery and Retrieval:** retrieve a portion of a mission based on defined area, time period, platform ID, type of platform - expose API to external sites;

**3.1.1.4 Visualization:** provide metadata to and display MTI data on an enterprise mapping service - provide a configurable list of MTI missions and status; AND

**3.1.1.5 Storage:** store metadata at appropriate classification level - provide source data based on queries across security domains - Store in accordance with records management laws, policies, etc.

**3.1.2 STANAG 4676 -** Adopt, adapt, or build open services to be exposed or consumed in a cloud-based enterprise for the processing of STANAG 4676 data and data types for the purpose of:

**3.1.2.1 Ingest:** Common vector files (shp, csv, NTRK, KML) - STANAG 4676 in JSON format & edition 1 format - user generated tracks - support discovery & retrieval;

**3.1.2.2 Catalog:** All source generated and user generated metadata and tracks - support proper tagging for discovery, retrieval;

**3.1.2.3 Discovery and Retrieval:** based on location/area and time - at users security domain and lower domains;

**3.1.2.4 Visualization:** provide metadata to and display tracks on an enterprise mapping service; AND

**3.1.2.5 Storage:** store metadata at appropriate classification level - provide source data based on queries across security domains - Store in accordance with records management laws, policies, etc.

**3.1.3 Ancillary / Enabling** - Adopt, adapt, or build ancillary open services to be exposed or consumed in a cloud-based enterprise to meet operational performance and efficiency requirements as further defined for STANAG 4607 & 4676 data and data-types (latency, fidelity, compliance).


### 3.2 LIST OF DELIVERABLES WITH QUALITY ASSURANCE SURVEILLANCE PLAN (QASP)

To satisfy the needs of \_\_\_\_\_\_\_\_\_\_\_\_ the following deliverables shall be provided by the conclusion of performance. The COR will evaluate the performance objectives of deliverables through surveillance as reflected below by reviews and acceptance of work products and services. As indicated, the COR will assess progress towards the final delivered software code. Note that the performance requirements listed below are required for the final deliverable. However, the Government to ensure that the Offeror is on a path to successful final delivery will assess the sprints and incremental delivery of code. (see QASP, ATTACHMENT 02).

| **Deliverable or Required Services** | **Performance Standard(s)** | **Acceptable Quality Level** | **Method of Surveillance** |
| --- | --- | --- | --- |
| Tested Code | Code delivered under the order must have substantial test code coverage and a clean code base  Version-controlled NGA GitHub repository of code that comprises product that will remain in the NGA government domain | Minimum of 90% test coverage of all relevant code | Combination of manual review and the results from automated testing |
| Properly Styled Code | [18F Front End Guide](https://frontend.18f.gov/#js-style) | 0 linting errors and 0 warnings | Combination of manual review and the results from automated testing |
| Accessible | Web Content Accessibility Guidelines 2.0 AA (WCAG 2.0 AA) standards | 0 errors reported for WCAG 2.0 AA standards using an automated scanner and 0 errors reported in manual testing | [http://squizlabs.github.io/HTML\_CodeSniffer/](http://squizlabs.github.io/HTML_CodeSniffer/)or  [https://github.com/pa11y/pa11y](https://github.com/pa11y/pa11y) |
| Deployed | Code must successfully build and deploy into staging environment. | Successful build with a single command | Combination of manual review and automatic testing |
| Documentation | All dependencies are listed and the licenses are documented. Major functionality in the software/source code is documented. Individual methods are documented inline using comments that permit the use tools such as JsDoc. System diagram is provided. | Combination of manual review and automatic testing, if available | Manual review |
| Secure | OWASP Application Security Verification Standard 3.0 | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities | Clean tests from a static testing SaaS (such as Gemnasium) and from OWASP ZAP, along with documentation explaining any false positives |

## 4.0 PERIOD OF PERFORMANCE

This order shall be comprised of one (1) base period of six (6) calendar months and two (2) option periods of six (6) calendar months each. The total potential period of performance is **not-to-exceed 18 months.**



## 5.0 PLACE OF PERFORMANCE

The primary place of performance will be at the contractor’s facility.



## 6.0 CONTRACT TYPE

The Government anticipates awarding a Time-and-Materials (T&amp;M) type task order against company’s existing General Services Administration (GSA) Schedule Information Technology 70 (IT 70) contract.



## 7.0 OPERATING CONSTRAINTS (NON-FUNCTIONAL REQUIREMENTS)

### 7.1 PERSONNEL SKILLS AND KNOWLEDGE

The Offeror shall provide qualified personnel with relevant experience and domain knowledge in line with the Statement of Objectives, in terms of necessary skills and the requisite level of knowledge and experience. The Offeror shall assign those persons whose resumes are submitted with its quotation and who are identified in the Offeror’s quotation as Key Personnel. All Offeror employees assigned to perform this task order will be Key Personnel. Broadly, a team assigned to perform on this task order should have experience with:

**7.1.1** Building and testing web-based or mobile applications: user-centric design practices, usability testing, User experience design, Visual design, Specific code languages, Cloud deployment, Open-source login / authentication services, Agile and scrum methodologies, etc.; AND_

**7.1.2** _Parsing binary data streams._

### 7.2 ENVIRONMENT

**7.2.1** The implemented solution shall be in conformance with NGA’s Certification and Accreditation process (e.g., ICD 503)

**7.2.2** The developed solution shall be in conformance with NGA’s Readiness process.

**7.2.3** Available AWS Environment Services & Tools (see ATTACHMENT 04)



## 8.0 INSTRUCTIONS AND EVALUATION

Please submit your quotation in accordance with the instructions specified in this RFP and the terms and conditions of your GSA Schedule Contract, and the prices contained therein. Please ensure that your response includes all requested information and that your technical response clearly demonstrates your company’s capability to perform the objectives in the SOO. The Government intends to award based on initial offers. Therefore, it is critical that you are fully responsive to the solicitation and submit your best offer initially. These are the milestones provided for this solicitation:

| **No.** | **Due Dates** | **Acquisition Event** |
| --- | --- | --- |
| 1 | TBD | Solicitation released |
| 2 | TBD plus 2-3 days | Questions due |
| 3 | TBD plus 4-6 weeks | Proposals due (Technical and Price) |



### 8.1 INSTRUCTIONS FOR PROPOSALS

**8.1.1 TECHNICAL UNDERSTANDING AND APPROACH (Factor 1)**

Provide your understanding of the performance objectives for Section 3 requirements. Also, describe your staffing plan based on your technical understanding and approach for the requirements with an estimated level of effort to complete. The estimated level of effort shall include a breakdown of labor categories, including the title, number of personnel, and hours. The page limit for this written technical proposal is **three (3) pages.** Do not submit price related information with the written technical proposal.

**8.1.2 KEY PERSONNEL (Factor 2)**

Provide a comprehensive list of all proposed key personnel by name, title, contact information, duties, roles, and include a subsequent resume for each proposed key personnel. Each resume shall include a brief description of the relevant experience and capability of the personnel proposed, as well as address the individual’s technical background, education, work experience, and accomplishments as they relate to the activities required in this solicitation. If proposing key personnel who are not currently employed or a teaming partner, then you are also required to provide a signed letter of intent. Resumes shall not exceed **one (1)**  **page** in length.

**8.1.3 SIMILAR EXPERIENCE (Factor 3)**

Provide a comprehensive list of similar projects delivered either by the Offeror, by a Teaming Partner proposed in response to this solicitation, or by any Key Personnel proposed in response to this solicitation. Please identify how your proposed team was involved in the project.

**8.1.3.1** Links to the Git repository (either credentialed or public) that includes the source code that was developed and accepted for the project must be provided;

**8.1.3.2** The projects must have been delivered by either a) the Offeror itself or, alternatively, b) a teaming partner that is proposed in response to this solicitation, or, alternatively, c) any key personnel that is being proposed in response to this solicitation. Please identify how the Offeror’s team was involved in the development. Offerors that include similar experience of the same key personnel who directly participated in the cited similar experience will be ranked higher than those who propose projects that did not involve their key personnel;

**8.1.3.3** If you fail to submit two code repositories in the same language as proposed for this requirement will be deemed non-responsive and not be considered for award;

**8.1.3.4** Code repositories submitted must have been for projects completed within the past three (3) calendar years, with staffing profiles of approximately five (5) to nine (9) Full Time Equivalent (FTE) personnel in periods of performance lasting no more than six (6) calendar months.

Written technical quotes that fail to include any of the items identified above will not be considered for award. Inclusion of caveats, assumptions, or exceptions to the requirement of any kind, in any part of the submission, will result in the Offeror no longer being considered for award.

## 9.0 PRICE PROPOSAL

Offerors should complete both tabs of the pricing template (ATTACHMENT 03). The first tab is for the base period of six months, the second tab is for the first option period of six months, and the third tab is for the second option period of six months. For purposes of pricing the option period, the offeror should assume continued performance by all members of the proposed team at full operating capacity for the duration of the performance period. **The price quotation must be received no later than the due date indicated above.** All proposed labor rates must be consistent with the terms, conditions, and rates of your GSA Schedule Master Award. Proposed labor rates must be fully burdened and include profit, fringe benefits, salary, indirect rates, and the Contract Access Fee (CAF).



## 10.0 BASIS FOR AWARD

The final award for this requirement will be based on best-value principles. Accordingly, award will be made to the responsible and technically acceptable Offeror whose quote provides the greatest overall value to the Government, price and other factors considered. This best-value determination will be accomplished by comparing the value of the differences in the technical factors for competing offers under consideration in the technical evaluation, based on their strengths, weaknesses, and risks, with differences in their price to the Government.

In making this comparison, the Government is more concerned with obtaining superior technical and management capabilities than with making awards at the lowest overall price to the Government. However, the Government will not make awards at a significantly higher overall price to achieve slightly superior technical value. Offerors are advised that the technical evaluation factors combined are significantly more important than price.



## 11.0 CONTRACT ADMINISTRATION

### 11.1 THE CONTRACTING OFFICER (CO)

The Contracting Officer (CO) is responsible for monitoring contract compliance, contract administration, and cost control and for resolving any differences between the observations documented by the contracting officer’s representative (COR) and the Offeror. The CO will designate one full-time COR as the Government authority for performance management. The number of additional representatives serving as technical inspectors depends on the complexity of the services measured, as well as the Offeror’s performance, and must be identified and designated by the CO.

Contracting Officer (CO): TBD


### 11.2 THE CONTRACTING OFFICER’S REPRESENTATIVE (COR)

The contracting officer’s representative (COR) is designated in writing by the CO to act as his or her authorized representative to assist in administering a contract. COR limitations are contained in the written appointment letter. The COR is responsible for technical administration of the project and ensures proper Government surveillance of the Offeror’s performance. The COR is not empowered to make any contractual commitments or to authorize any contractual changes on the Government’s behalf. Any changes that the Offeror deems may affect contract price, terms, or conditions shall be referred to the CO for action.  The COR will have the responsibility for completing QA monitoring forms used to document the inspection and evaluation of the Offeror’s work performance. Government surveillance may occur under the inspection of services clause for any service relating to the contract.

Contracting Officer’s Representative (COR): TBD


### 11.3 KEY PERSONNEL

Key personnel and staffing requirements will be defined at the TO level. The name and resume of key personnel shall be designated in writing to the CO for approval. Prior to removing, replacing, or diverting any key personnel, the Offeror shall notify the CO no less than fifteen (15) business days in advance and shall submit a proposed replacement for Government review within fifteen (15) days of notification. The Government retains the right, at its discretion, to reject any proposed replacements of key personnel.


### 11.4 CLAUSES & PROVISIONS

See **ATTACHMENT 05** for additional provisions and clauses applicable to this Task Order Request for Proposal. In the event

### 11.5 ATTACHMENTS

| **Attachment Number** | **Description** |
| --- | --- |
| 01 | SOO |
| 02 | QASP |
| 03 | Pricing Template |
| 04 | Available AWS Environment Services & Tools |
| 05 | Clauses & Provisions        (TBD) |
