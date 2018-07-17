# National Geospatial-Intelligence Agency (NGA)

# Moving Target Indicator (MTI) Software Modernization

## Attachment 01: Scope and Objectives

Develop capabilities to ingest, discover, retrieve and visualize MTI data (STANAG 4607, STANAG 4676, and mission data) in the cloud across multiple security domains.

### Backlog

#### 1. MTI Streaming Data Epic

As a content service provider I want to ingest, store, and expose STANAG 4607 and STANAG 4676 streaming data so that downstream systems and applications can consume the data.

Below is a high-level story map for this epic.  The story map is a starting point for the definition of user stories under this epic by the Government-assigned product owner in collaboration with the vendor’s Agile software development team.

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
<td>Display STANAG 4607 and STANAG 4676 streaming data and associated metadata on an enterprise mapping service that conforms to OGC standards. Current enterprise mapping service is GEOINT Visualization Services (GVS)/Map of the World,(MoW)</td>
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

#### 2. MTI File Data Epic

As a content service provider I want to ingest, store, and expose STANAG 4607 and STANAG 4676 MTI files and associated mission data so that downstream systems and applications can consume them.

Below is a high-level story map for this epic.  The story map is a starting point for the definition of user stories under this epic by the Government-assigned product owner in collaboration with the vendor’s Agile software development team.

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
<td>Display STANAG 4607 and STANAG 4676 file data and associated metadata on an enterprise mapping service that conforms to OGC standards. Current enterprise mapping service is GEOINT Visualization Services (GVS)/Map of the World, (MoW)</td>
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

#### 3. Data Management Epic

As a content service provider I want the ability to manage metadata (create, read, update, and delete) associated with any and all MTI streaming data, data files, and mission data.

#### 4. Develop capability for SC2S
Deliver working code to accomplish user tasks within SC2S.  SC2S is an AWS classified cloud-computing environment for Government use.  It has a subset of commercial AWS services with limitations currently described in attachment 04a: AWS Cloud Service Availability. The developer is limited to the AWS services listed in attachment 04a in providing their solution.  Amazon continually introduces more services from the current AWS commercial offerings into SC2S, which the developer can use for subsequent deliveries.

#### 5. Use agile and scrum
The developer produces, tests, and delivers capability drawn from the evolving program feature backlog, in accordance with the priorities of the government product owner, for deployment into the staging environment at the end of each sprint.

#### 6. Deliver on Demand; prepare integrator for success
The developer delivers its product and avails associated documentation to an integrator. The integrator performs the remaining security steps necessary to deploy the code to the classified environment. The integrator performs integration testing, and gains user acceptance. We anticipate regular collaboration between the developer and integrator in order to resolve any compliance or performance deltas discovered between the unclassified development-staging environment and the classified operational environment. Developer will work with the integrator to deliver code within the integrator-defined, repeatable, automated build process.  Once notified of a production issue the developer will react quickly and work with the integrator to resolve the issue.

#### 7. Address Scalability – vertical and horizontal
NGA expects MTI streams and data volumes to grow over time and the capability needs to be built on top of a scalable architecture. The architecture supports growth in users, traffic, or data size while maintaining performance. The capability scales linearly and proportionally to demand. Your design should seamlessly leverage the unlimited on-demand capacity through automated elastic scaling provided by cloud services.
