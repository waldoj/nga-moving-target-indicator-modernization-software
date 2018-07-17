# National Geospatial-Intelligence Agency (NGA)

# Moving Target Indicator (MTI) Software Modernization

## Request for Quote (RFQ)

**July 17, 2018**

## 1.0 PURPOSE

The National Geospatial-Intelligence Agency (NGA), Office of Contract Services (OCS), hereby issues this Request for Quote (RFQ) to procure services in support of the attached Statement of Objectives (SOO). This solicitation will be accomplished using the terms and conditions of the RFQ and of the offeror’s Master Contract under the GSA Federal Supply Schedule (FSS) contract, Schedule 70, General Purpose Commercial Information Technology Equipment, Software, and Services, under Special Item Number (SIN) 132 51.

## 2.0 BACKGROUND

NGA intends to retire its current traditional data center and replace it with a cloud-based computing environment. This necessitates migrating motion imagery data — MTI, Video, Wide Area Motion Imagery, and the associated operational capabilities to the cloud.

## 3.0 SCOPE AND OBJECTIVES

## 3.1 Scope

The scope of this effort is to develop capabilities to ingest, discover, retrieve and visualize MTI data (STANAG 4607, STANAG 4676, and mission data) in the cloud across multiple security domains.

**3.1.2 Develop capabilities using agile software development practices:** The offeror shall deliver capabilities defined by epics and user stories managed from an evolving and prioritized program backlog. The program backlog shall be established and maintained by the Government-assigned product owner in collaboration with the offeror’s agile development team.

**3.1.3 Deliver on Demand:** Deployments of production release candidates shall occur on a cadence established by the Government-assigned product owner.

**3.1.4 Offeror and Integrator DevOps Collaboration:** The offeror shall collaborate with a Government-assigned Integrator team to ensure the streamlined and successful deployment, integration, and ongoing support of production releases into SC2S. The Government-assigned product owner shall approve deployment of production release candidates. The Integrator shall complete the security C&amp;A process, deploy approved production releases into SC2S, and lead user acceptance testing activities. Collaboration between the offeror and Integrator shall span across design, development, and testing activities performed prior to SC2S deployments as well as deployment and post-deployment activities as deemed necessary and appropriate. The offeror and Integrator shall collaborate in attaining Authority to Test (ATT) and Authority to Operate (ATO) on SC2S. The offeror and Integrator shall collaborate to ensure that all Solution code, testing, and documentation artifacts comply with all pertinent governance mandates and meet the level of quality necessary to achieve successful integration, operation, and maintenance of offeror-developed software capabilities in SC2S.

### 3.2 Objectives Backlog

**3.2.1 MTI Streaming Data Epic** — As a content service provider, I want to ingest, store, and expose STANAG 4607 and STANAG 4676 streaming data so that downstream systems and applications can consume the data.

Below is a high-level overview of this epic. The story map is a starting point for the definition of user stories under this epic by the Government-assigned product owner in collaboration with the vendor’s agile software development team.

<table>
<thead>
<tr><th>Processing Step</th><th>Sub-Epics/Coarse-Grained Features</th><th>Acceptance Criteria</th></tr>
</thead>
<tbody>

<tr>
<td rowspan="3">INGEST</td>
<td>Ingest streaming data via multicast protocols</td>
<td rowspan="3"><ul><li>Data integrity is enforced and preserved</li><li>Applicable security controls are enforced</li><li>Performance requirements and SLAs are met</li></ul></td>
</tr>

<tr>
<td>Ingest STANAG 4607 formats 1, 2, and 3</td>
</tr>

<tr>
<td>Ingest STANAG 4676 in JSON and Edition-1 formats</td>
</tr>

<tr>
<td rowspan="2">INDEX / CATALOG</td>
<td>Index all streaming MTI data</td>
<td rowspan="2"><ul><li>Data integrity is enforced and preserved</li><li>Applicable security controls are enforced</li><li>Performance requirements and SLAs are met</li></ul></td>

<tr>
<td>Index to support search, discovery, and retrieval of streaming data</td>
</tr>
<tr>
<td rowspan="3">MISSION MANAGEMENT / STATUS</td>
<td>Expose streaming data (MTI and metadata) so that it is readily consumable by external visualization / display applications /services</td>
<td rowspan="3"><ul><li>Data integrity is enforced and preserved</li><li>Applicable security controls are enforced</li></li>Performance requirements and SLAs are met</li></ul></td></tr>
<tr>
<td>Expose metadata</td>
</tr>
<tr>
<td>Provide a web-interface to present a textual, configurable list of streaming missions and status</td>
</tr>
<tr>
<td>DISCOVER & RETRIEVE</td>
<td>Enable discovery and retrieval of a portion of a streamed mission based on geospatial criteria, temporal criteria, platform ID, type of platform, etc.</td>
<td><ul><li>Applicable security controls are enforced</li><li>Performance requirements and SLAs are met</li></ul></td>
</tr>
<tr>
<td>VISUALIZATION</td>
<td>Display STANAG 4607 and STANAG 4676 streaming data and associated metadata on an enterprise mapping service that conforms to OGC standards. Current enterprise mapping service is GEOINT Visualization Services (GVS) / Map of the World, MoW)</td>
<td>
<ul><li>Applicable security controls are enforced</li>
<li>Performance requirements and SLAs are met</li>
</ul>
</tr>
<tr>
<td>STORE</td>
<td>Enable streaming data to be stored in an enterprise cloud storage service</td>
<td>
<ul><li>Data integrity is enforced and preserved</li>
<li>Applicable security controls are enforced</li>
<li>Performance requirements and SLAs are met</li>
</td>
</tr>
</body>
</table>

**3.2.2 MTI File Data Epic** — As a content service provider I want to ingest, store, and expose STANAG 4607 and STANAG 4676 MTI files and associated mission data so that downstream systems and applications can consume them.

Below is a high-level story map for this epic. The story map is a starting point for the definition of user stories under this epic by the Government-assigned product owner in collaboration with the vendor’s agile software development team.

<table>
<thead>
<tr><th>Processing Step</th><th>Sub-Epics/Coarse-Grained Features</th><th>Acceptance Criteria</th></tr>
</thead>
<tbody>
<tr>
<td rowspan="4">INGEST</td>
<td>Ingest MTI files (STANAG 4607, STANAG 4676) and associated mission data (e.g. imagery, chat logs, audio, etc.)</td>
<td rowspan="4">
<ul><li>Data integrity is enforced and preserved</li>
<li>Applicable security controls are enforced</li>
<li>Performance requirements and SLAs are met</li>
</ul>
</td>
</tr>
<tr>
<td>Process/Condition MTI file data</td>
</tr>
<tr>
<td>Create sanitized/declassified MTI file for general release</td>
</tr>
<tr>
<td>Maintain relational links between MTI files and associated mission data</td>
</tr>

<tr>
<td rowspan="4">INDEX / CATALOG</td>
<td>Index all MTI file data</td>
<td rowspan="4">
<ul>
<li>Data integrity is enforced and preserved</li>
<li>Applicable security controls are enforced</li>
<li>Performance requirements and SLAs are met</li>
</ul>
</td>
</tr>

<tr>
<td>Link MTI date with associated mission data</td>
</tr>
<tr>
<td>Enable metadata lifecycle management</td>
</tr>
<tr>
<td>Index to support search, discovery, and retrieval of MTI and associated mission data</td>
</tr>

<tr>
<td rowspan="3">MISSION MANAGEMENT / STATUS</td>
<td>Expose MTI and metadata so that it is readily consumable by external visualization / display applications /services</td>
<td rowspan="2">
<ul>
<li>Data integrity is enforced and preserved</li>
<li>Applicable security controls are enforced</li>
<li>Performance requirements and SLAs are met</li>
</ul>
</td>
</tr>
<tr>
<td>Expose mission data</td>
</tr>

<tr>
<td>Provide a web-interface to present a textual, configurable list of MTI file data and associated mission data</td>
<td>
<ul>
<li>Applicable security controls are enforced</li>
<li>Performance requirements and SLAs are met</li>
</ul>
</td>
</tr>
<tr>
<td rowspan="2">DISCOVER & RETRIEVE</td>
<td>Enable discovery and retrieval of a portion of an archived MTI mission based on geospatial criteria, temporal criteria, platform ID, type of platform, etc.</td>
<td>
<ul>
<li>Applicable security controls are enforced
<li>Performance requirements and SLAs are met
</ul>
</td>

<tr>
<td>Enable discovery and retrieval of mission data associated with MTI mission based on mission ID</td>
<td>
<ul><li>Applicable security controls are enforced</li><li>Performance requirements and SLAs are met</li></ul>
</td>
</tr>
<tr>
<td>VISUALIZATION</td>
<td>Display STANAG 4607 and STANAG 4676 file data and associated metadata on an enterprise mapping service that conforms to OGC standards. Current enterprise mapping service is GEOINT Visualization Services (GVS) / Map of the World (MoW)</td>
<td>
<ul>
<li>Applicable security controls are enforced</li>
<li>Performance requirements and SLAs are met</li>
</ul>
</td>
</tr>

<tr>
<td>STORE</td>
<td>Enable MTI file data and associated mission data to be stored in an enterprise cloud storage service</td>
<td>
<ul>
<li>Data integrity is enforced and preserved</li>
<li>Applicable security controls are enforced</li>
<li>Performance requirements and SLAs are met</li>
</td>
</tr>
</tbody>
</table>

**3.2.3 Data Management Epic** — As a content service provider I want the ability to manage metadata (create, read, update, and delete (CRUD)) associated with any and all MTI streaming data, data files, and mission data.

**3.2.4 Ancillary / Enabling** - Adopt, adapt, or build ancillary open services to be exposed or consumed in a cloud-based enterprise to meet operational performance and efficiency requirements as further defined for STANAG 4607 &amp; 4676 data and data-types (latency, fidelity, compliance).


### 3.3 List of Deliverables with Quality Assurance Surveillance Plan (QASP)

To satisfy the needs of the Agency, the following deliverables shall be provided by the conclusion of performance. The COR will evaluate the performance objectives of deliverables through surveillance as reflected below by reviews and acceptance of work products and services. As indicated, the Contracting Officer Representative (COR) will assess progress towards the final delivered software code. Note that the performance requirements listed below are required for the final deliverable; however, the Government will assess the sprints and incremental delivery of code, to ensure that the offeror is on a path to successful final delivery (see [QASP, ATTACHMENT 02](02_QASP.md)).

| Deliverable or Required Services | Performance Standard(s) | Acceptable Quality Level | Method of Surveillance\* |
| --- | --- | --- | --- |
| Tested Code | Code delivered under the order must have substantial test code coverage and a clean code base Version-controlled NGA GitHub repository of code that comprises product that will remain in the NGA government domain | Minimum of 90% test coverage of all relevant code |   |
| Properly Styled Code | [18F Front-End Guide](https://frontend.18f.gov/#js-style) | 0 linting errors and 0 warnings |   |
| Accessible | Web Content Accessibility Guidelines 2.0 AA (WCAG 2.0 AA) standards | 0 errors reported for WCAG 2.0 AA standards using an automated scanner and 0 errors reported in manual testing |   |
| Deployed | Code must successfully build and deploy into staging environment. | Successful build with a single command |   |
| Documentation | All dependencies are listed and the licenses are documented. Major functionality in the software/source code is documented. Individual methods are documented inline using comments that permit the use tools such as JsDoc. System diagram is provided. | Combination of manual review and automatic testing, if available |   |
| Secure | OWASP Application Security Verification Standard 3.0 | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities |   |

**\*** _The government will determine the method of surveillance and frequency of surveillance based on the successful offeror’s PWS._

## 4.0 PERIOD OF PERFORMANCE

This order shall be comprised of one (1) base period of six (6) calendar months and two (2) option periods of six (6) calendar months each. The total potential period of performance is **18 months.**

## 5.0 PLACE OF PERFORMANCE

The primary place of performance will be at the contractor’s facility.


## 6.0 CONTRACT TYPE

The Government anticipates awarding a Time-and-Materials (T&amp;M) type task order against company’s existing General Services Administration (GSA) Schedule Information Technology 70 (IT 70) contract.


## 7.0 OPERATING CONSTRAINTS (NON-FUNCTIONAL REQUIREMENTS)

### 7.1 PERSONNEL SKILLS AND KNOWLEDGE

The offeror shall provide qualified personnel with relevant experience and domain knowledge in line with the Statement of Objectives, in terms of necessary skills and the requisite level of knowledge and experience. The offeror shall assign those persons whose resumes are submitted with its quotation and who are identified in the offeror’s quotation as Key Personnel. All offeror employees assigned to perform this task order will be Key Personnel. Broadly, a team assigned to perform on this task order should have experience with:

**7.1.1** Building and testing web-based or mobile applications: user-centric design practices, usability testing, user experience design, visual design, cloud deployment, open-source login / authentication services, Agile and Scrum methodologies, etc.; _AND_

**7.1.2** Parsing binary data streams.

### 7.2 ENVIRONMENT

**Develop the Solution for Deployment in SC2S:** The offeror shall deliver the Solution as incremental, production-ready software releases optimized to operate within SC2S. SC2S is a classified AWS cloud-computing environment, for Government use, that hosts the subset of commercial AWS-derived services described in [attachment 04a: AWS Cloud Service Availability](04a_AWS.md). The offeror may leverage the AWS services listed in attachment 04a as part of the Solution. The offeror may not incorporate non-AWS services into the Solution unless the services are native to the code base developed by the offeror. As additional service offerings from the AWS commercial cloud gain approval for deployment in SC2S, the offeror may incorporate them into subsequent releases (see [ATTACHMENT 04a](04a_AWS.md)).

## 8.0 INSTRUCTIONS AND EVALUATION

Please submit your quotation in accordance with the instructions specified in this RFQ, the terms and conditions of your GSA Schedule Contract, and the prices contained therein. Please ensure that your response includes all requested information and that your technical response clearly demonstrates your company’s capability to perform the objectives in the SOO. These are the milestones provided for this solicitation:

| **No.** | **Due Dates** | **Acquisition Event** |
| --- | --- | --- |
| 1 | 17JUL18 | Solicitation released |
| 2 | 20JUL18 by 1700EST | Questions due |
| 3 | 23JUL18 by 1700EST | Letters of Intent |
| 4 | 31JUL18 by 1700EST | Quotes due (Technical and Price) |
| 5 | TBD | Award decision |

Page size for all documents provided shall be 8.5 x 11 inches and shall be single spaced with at least 1 inch margins for all sides. The font size shall be no less than 12 points. Files shall not be zipped (.zip).

Do not lock or encrypt any files emailed as part of the proposal submission. Perform a virus check prior to emailing any files; a virus infected file may cause rejection of that file and could result in the offeror no longer being considered for award. All submissions related to this RFQ and the above Acquisition Events shall be submitted via e-mail to the following:

|Karen L. Eichelberger | Contracting Officer |[Karen.L.Eichelberger@nga.mil](mailto:Karen.L.Eichelberger@nga.mil)|
| --- | --- | --- |
Joseph Hicks        Contract Specialist        [Joseph.W.Hicks@nga.mil](mailto:Joseph.W.Hicks@nga.mil)

This procurement is being conducted in accordance with FAR Subpart 8.4, Federal Supply Schedules. This is not a FAR Part 15, Contracting by Negotiation, procurement. All submissions in response to this RFQ are considered quotations and not proposals or offers, even if labeled as such. The offerors agree to and are bound by all instructions, procedures and rules of this RFQ under Part 8. The Government is not obligated to determine a competitive range, conduct discussions, solicit final revised quotations, or use other techniques associated with FAR Part 15. The contracting techniques associated with FAR Part 15.3 do not apply in any way, shape, or form to this action.
### 8.1 INSTRUCTIONS FOR WRITTEN QUOTATIONS

Written quotes (all sections) are due by no later than by **1700 EST on JULY 31th, 2018**. Quotes not submitted via e-mail, or not received by the above deadline, will NOT be evaluated. Contact the Contracting Officer and/or the Contract Specialist if you have not received a confirmation of receipt, including attachments, within 24 hours of your quote submission.

Your written quote shall contain the following sections:

- **Staffing Plan including Key Personnel information** (Resumes and any Letters of Intent); the Staffing Plan has a **three (3) page** limit, with a **two (2) page** limit per Resume and a one (1) page limit per Letter of Intent,
- **Performance Work Statement** (PWS) responsive to the SOO; with **five (5) page** limit total;
- **Similar Experience**; three (3) pages per project, requisite project code submitted via Git repository **does not** count against page limitation; AND
- **Completed Price Quote** ([template provided](Pricing_Template.xlsx)).

**8.1.1 STAFFING PLAN (Factor 1)**

Describe your staffing plan based on your technical understanding and approach for the requirements with an estimated level of effort to complete.

Provide a comprehensive list of all proposed key personnel by name, title, duties, roles, and include a subsequent resume for each proposed key personnel. Each resume shall include a brief description of the relevant experience and capability of the personnel proposed, as well as address the individual’s technical background, education, work experience, and accomplishments as they relate to the activities required in this solicitation. If proposing key personnel who are not currently employed or a teaming partner, then you are also required to provide a signed letter of intent. Resumes shall not exceed **two (2) pages** in length.

**8.1.2 PERFORMANCE WORK STATEMENT (Factor 2)**

Provide your technical understanding and approach to the performance objectives (SOO) under Section 3 - Scope and Objectives requirements. The PWS may include any relevant information on framework, tools, technologies and processes. The estimated level of effort shall include a breakdown of labor categories, including the title, number of personnel, and hours. The page limit for the PWS is **five (5) pages.**  Do not submit price related information with the written PWS.

**8.1.3 SIMILAR EXPERIENCE (Factor 3)**

Provide a list of at least two (2), but no more than three (3) relevant projects delivered either by the offeror, by a Teaming Partner proposed in response to this solicitation, or by any Key Personnel proposed in response to this solicitation. Please identify how your proposed team was involved in the project.

**8.1.3 SIMILAR EXPERIENCE (Factor 3)**

Provide a comprehensive list of similar projects delivered either by the Offeror, by a Teaming Partner proposed in response to this solicitation, or by any Key Personnel proposed in response to this solicitation. Please identify how your proposed team was involved in the project.

**8.1.3.1** Links to the Git repository (either credentialed or public) that includes the source code developed and accepted for the relevant projects must be provided;

**8.1.3.2** The projects must have been delivered by either a) the offeror itself or, alternatively, b) a teaming partner that is proposed in response to this solicitation, or, alternatively, c) any key personnel that is being proposed in response to this solicitation. Please identify how the offeror’s team was involved in the development. Offerors that include similar experience of the same key personnel who directly participated in the cited similar experience will be ranked higher than those who propose projects that did not involve their key personnel;

**8.1.3.3** If you fail to submit at least two (2) relevant code repositories in the same language as proposed for this requirement you will be deemed non-responsive and not be considered for award;

**8.1.3.4** Code repositories submitted must have been for projects completed within the past three (3) calendar years, with staffing profiles of approximately five (5) to nine (9) Full Time Equivalent (FTE) personnel.

Quotes that fail to include any of the required information identified under 8.1 above will not be considered for award. Inclusion of caveats, assumptions, or exceptions to the requirement of any kind, in any part of the submission, will result in the offeror no longer being considered for award.

**8.1.4 Price Quote**

Offerors should complete both tabs of the pricing template ([ATTACHMENT 03](03_Pricing_Template.xlsx)). The first tab is for the base period of six months, the second tab is for the first option period of six months, and the third tab is for the second option period of six months. For purposes of pricing the option period, the offeror should assume continued performance by all members of the proposed team at full operating capacity for the duration of the performance period. **The price quotation must be received no later than the due date indicated above.** All proposed labor rates must be consistent with the terms, conditions, and rates of your GSA Schedule Master Award. Proposed labor rates must be fully burdened and include profit, fringe benefits, salary, indirect rates, and the Contract Access Fee (CAF).

The Price Quote shall also contain a cover page containing the following information:

- GSA Contract Number
- Cage Code
- DUNS number
- Tax ID or Business Size
- Validity period for quote (minimum of 90 days)
- Company Point of Contact (name, phone number, email address)
- Payment terms
- Indicate any discounts from your GSA established rates

Inclusion of caveats, assumptions, or exceptions to the requirement of any kind, in any part of the submission, will result in the offeror no longer being considered for award.


## 9.0 EVALUATION AND BASIS FOR AWARD

**9.1 Evaluation Process**

The final award for this requirement will be based on best-value principles, utilizing the trade-off process. Accordingly, award will be made to the responsible and technically acceptable offeror whose quotation provides the greatest overall value to the Government, price and other factors considered.

The Government is more concerned with obtaining superior technical capabilities than with making awards at the lowest overall price to the Government. However, the Government will not make awards at a significantly higher overall price to achieve slightly superior technical value. Offerors are advised that the technical evaluation factors combined are significantly more important than price.

**The evaluation factors for award are as follows in descending order of importance:**

- Factor 1: Staffing Plan
- Factor 2: Technical Understanding and Approach
- Factor 3: Similar Experience
- Factor 4: Price

**9.1.1 Technical Evaluation**

We will review your responses to ensure they demonstrate an understanding of the requirements outlined in the proposed PWS, particularly Section 3, and the strength of the proposed development expertise, agile practices, and implementation of UX design. For each requested section, the Government will review the following:

- **Staffing Plan:** The Government will evaluate the offeror’s proposed staffing methodology and skill levels/labor categories as well as the availability and relevant work experience demonstrated by Key Personnel.
- **Technical Understanding and Approach:** The Government will evaluate the offeror’s technical approach: level of knowledge, technical expertise, and overall understanding of the requirement. The Government will also evaluate the offeror’s skills with open source software development, human-centered design, and continuous deployment methods.
- **Similar Experience:** The Government will evaluate the offeror’s experience in performing projects of similar scope and complexity. The Government will also evaluate the offeror’s experience with open source software development, human-centered design, and continuous deployment methods.

**9.1.2 Price Evaluation**

Each offeror’s price quotation will be evaluated separately from the technical response. Note that as submissions become more technically equal in their merit, the evaluated price becomes more important.

## 10.0 BASIS FOR AWARD

The final award for this requirement will be based on best-value principles per FAR 8.405-2. Accordingly, award will be made to the responsible and technically acceptable offeror whose quote provides the greatest overall value to the Government, price and other factors considered.

This best-value determination will be accomplished by comparing the value of the differences in the technical factors for competing offers under consideration in the technical evaluation, based on their strengths, weaknesses, and risks, with differences in their price to the Government.

In making this comparison, the Government is more concerned with obtaining superior technical and management capabilities than with making awards at the lowest overall price to the Government. However, the Government will not make awards at a significantly higher overall price to achieve slightly superior technical value. Offerors are advised that the technical evaluation factors combined are significantly more important than price.


## 11.0 CONTRACT ADMINISTRATION

### 11.1 KEY PERSONNEL

Key personnel and staffing requirements will be defined at the TO level. The name and resume of key personnel shall be designated in writing to the CO for approval. Prior to removing, replacing, or diverting any key personnel, the Offeror shall notify the CO no less than fifteen (15) calendar days in advance and shall submit a proposed replacement for Government review within fifteen (15) days of notification. The Government retains the right, at its discretion, to reject any proposed replacements of key personnel.

### 11.2 ATTACHMENTS

| **Attachment Number** | **Description** |
| --- | --- |
| 01 | SOO |
| 02 | QASP |
| 03 | Pricing Template |
| 04a | Available AWS Environment Services &amp; Tools |
| 04b | MTI Backlog |
| 05 | Clauses &amp; Provisions |
