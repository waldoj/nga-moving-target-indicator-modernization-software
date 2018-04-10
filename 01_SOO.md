# National Geospatial-Intelligence Agency (NGA)

# Moving Target Indicator (MTI) Software Modernization

## Attachment 01: Scope and Objectives

Develop capabilities to ingest, discover, retrieve and visualize MTI data (STANAG 4607, STANAG 4676, and mission data) in the cloud across multiple security domains.

### Backlog

**1. STANAG 4607** - Adopt, adapt, or build open services to be exposed or consumed in a cloud-based enterprise for the processing of STANAG 4607 data and data types for the purpose of:
<ol type="a">
  <li>Ingest: receive data via multicast protocols - ingest both streaming and file based data -  ingest STANAG 4607 formats 1,2, & 3 – ingest up to 1TB/day of MTI data – support search, discovery, retrieval of MTI data;</li>
  <li>Catalog: all source & MTI data – maintain metadata integrity – retain metadata as long as the source data – maintain modifications to metadata – maintain metadata at appropriate classification level and associate it at any classification level – support search, discovery, retrieval, and visualization of MTI;</li>
  <li>Discovery and Retrieval: retrieve a portion of a mission based on defined area, time period, platform ID, type of platform – expose API to external sites;</li>
  <li>Visualization: provide metadata to and display MTI data on an enterprise mapping service – provide a configurable list of MTI missions and status; AND</li>
  <li>Storage: store metadata at appropriate classification level – provide source data based on queries across security domains – Store in accordance with records management laws, policies, etc.</li>
</ol>

**2. STANAG 4676** — Adopt, adapt, or build open services to be exposed or consumed in a cloud-based enterprise for the processing of STANAG 4676 data and data types for the purpose of:
<ol type="a">
  <li>Ingest: Common vector files (Shapefile, CSV, NTRK, KML) – STANAG 4676 in JSON format & edition 1 format – user generated tracks – support discovery & retrieval;</li>
  <li>Catalog: All source generated and user generated metadata and tracks – support proper tagging for discovery, retrieval;</li>
  <li>Discovery and Retrieval: based on location/area and time – at users security domain and lower domains;</li>
  <li>Visualization: provide metadata to and display tracks on an enterprise mapping service; AND</li>
  <li>Storage: store metadata at appropriate classification level – provide source data based on queries across security domains – Store in accordance with records management laws, policies, etc.</li>
</ol>

**3. Ancillary / Enabling** – Adopt, adapt, or build ancillary open services to be exposed or consumed in a cloud-based enterprise to meet operational performance and efficiency requirements as further defined for STANAG 4607 & 4676 data and data-types (latency, fidelity, compliance)
