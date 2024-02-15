---
excerpt: Best practices for data security, data access management, (meta)data standards, and data flow
layout: default
title: Data and Metadata Management
nav_order: 3
has_children: false
has_toc: false
---
# Data and Metadata Management

Welcome! If you are involved in data or metadata standards aspects of establishing a Federated EGA node, you are in the right place. The information here covers topics related - but not limited - to best practices for data security, data access management, (meta)data standards, and data flow.

**You might find this page useful if you are:**
- a bioinformatician
- a data steward
- a data protection officer
- a support officer

**By exploring these materials, you will be able to:**
- Define data security and access management best practices
- Understand the EGA metadata standard and it's minimal requirements
- Identify data models specific to a domain (*e.g.* COVID-19) and apply them when needed
- Comprehend the (meta)data flow within the Federated EGA Network

## 1. Learn about data security best practices

Central EGA has a <a href="https://ega-archive.org/assets/files/European_Genome_phenome_Archive_Security_Overview.pdf" target="_blank">Security Strategy</a> which defines best practices in ensuring data are stored securely. The EGA has helped develop the recommendations outlined the <a href="https://www.ga4gh.org/docs/ga4ghtoolkit/data-security/2016May10_REV_SecInfrastructure.pdf" target="_blank">GA4GH Security Technology Infrastructure document</a>, which defines guidelines, best practices, and standards for building and operating an infrastructure that promotes responsible data sharing in accordance with the <a href="https://www.ga4gh.org/docs/ga4ghtoolkit/data-security/Privacy-and-Security-Policy.pdf" target="_blank">GA4GH Privacy and Security Policy</a>.

Summary of best practices recommended for Federated EGA nodes:

| Item | Description | Examples/Templates |
|:---|:---|:---|
| Breach response protocol | A protocol for addressing potential security breaches, including consideration of other FEGA nodes, Central EGA, key contacts, and institutional/organisational policies. | Coming soon! |
| Risk register | A risk management tool used to track identified risks including information such as the nature of the risk, reference and owner, and mitigation measures. | Coming soon! |

<br/><br/>

## 2. Explore implemented standards

Central EGA largely adhere to <a href="https://ega-archive.org/about/projects-and-funders/ga4gh/" target="_blank">GA4GH standards</a>. Specific standards already implemented are summarised below:

| Standard | Purpose | Specification Version | Supported Version | Implementation | Publication/Preprint |
|:---|:---|:---|:---|:---|:---|
| Beacon | Supports discovery of genomic variants and individuals. | v1.0.1 | v0.3 | <a href="https://github.com/ga4gh-beacon/specification-v2" target="_blank">Specification</a>, <a href="https://ega-archive.org/about/projects-and-funders/beacon/" target="_blank">Documentation</a>, <a href="https://ega-archive.org/beacon-api/" target="_blank">Endpoint</a> | N/A |
| Crypt4GH | Enables direct byte-level compatible random access to encrypted genetic data stored in community standards (*e.g.* CRAM, VCF). | v1.0 | v1.0 | <a href="http://samtools.github.io/hts-specs/crypt4gh.pdf" target="_blank">Specification</a>, <a href="https://github.com/EGA-archive/crypt4gh" target="_blank">Documentation</a>, Endpoint | <a href="https://doi.org/10.1093/bioinformatics/btab087" target="_blank">DOI</a> |
| Data Use Ontology (DUO) | Allows users to semantically tag datasets with usage restrictions so datasets can be automatically discoverable based on a researcher's authorization level or intended use. | 2021-02-23 | 2021-02-23 | <a href="https://github.com/EBISPOT/DUO" target="_blank">Specification</a>, <a href="https://ega-archive.org/access/data-access-committee/data-use-ontology/" target="_blank">Documentation</a>, <a href="https://www.ebi.ac.uk/ols/api/ontologies" target="_blank">Endpoint</a> | <a href="https://doi.org/10.1016/j.xgen.2021.100028" target="_blank">DOI</a> |
| htsget | Enables secure, efficient, and reliable access to sequencing read and variation data including specific genomic regions. | v1.3.0 | v1.0.0 | <a href="http://samtools.github.io/hts-specs/htsget.html" target="_blank">Specification</a>, <a href="https://github.com/EGA-archive/ega-download-client" target="_blank">Documentation</a>, <a href="https://ega.ebi.ac.uk:8052/elixir/tickets/tickets" target="_blank">Endpoint</a> | <a href="https://doi.org/10.1093/bioinformatics/bty492" target="_blank">DOI</a> |
| refget | Enables access to reference sequences using an identifier derived from the sequence itself. | v1.2.6 | N/A | <a href="http://samtools.github.io/hts-specs/refget.html" target="_blank">Specification</a>, Documentation, Endpoint | <a href="https://doi.org/10.1093/bioinformatics/btab524" target="_blank">DOI</a> |
| Researcher IDs (Passports and visas) | Specifies the collection of researchers that may access a dataset at any given time, and the credentials they must supply. | v1.0.1 | v1.0.1 | <a href="https://github.com/ga4gh-duri/ga4gh-duri.github.io/blob/master/researcher_ids/ga4gh_passport_v1.md" target="_blank">Specification</a>, <a href="https://docs.google.com/document/d/1FTzUYAfV5d2a0zoDkbY9Iy_L5NbSAnHeWnmY2NIrY8M/edit" target="_blank">Documentation</a>, <a href="https://ega.ebi.ac.uk:8443/ega-permissions/swagger-ui/index.html" target="_blank">Endpoint</a> | <a href="https://doi.org/10.1016/j.xgen.2021.100030" target="_blank">DOI</a> |

<br/><br/>

### Data file standards

Recommended file formats for:
- Sequencing data (unaligned or aligned reads): <a href="http://samtools.github.io/hts-specs/CRAMv3.pdf" target="_blank">CRAM</a>, <a href="https://samtools.github.io/hts-specs/SAMv1.pdf" target="_blank">BAM</a>
- Variant data: <a href="https://samtools.github.io/hts-specs/VCFv4.2.pdf" target="_blank">VCF</a>
- Phenotype/clinical data: <a href="https://doi.org/10.1101/2021.11.27.21266944" target="_blank">Phenopackets</a>

### Metadata standards

The following resources represent EGA and community guidelines for submitted metadata:
- <a href="https://ega-archive.org/submission/metadata/ega-schema/" target="_blank">EGA metadata model</a>
- General FEGA standards
  - <a href="https://youtu.be/U6ilhM-XOhU" target="_blank">Introduction to metadata</a> video produced by CSC
  - <a href="https://youtu.be/0anBkJbF7XY" target="_blank">Introduction to phenotypic data</a> video produced by CSC
- Community-specific FEGA standards
  - <a href="https://zenodo.org/record/4893222" target="_blank">COVID-19 metadata mapping model</a> across COVID-19 studies in Federated EGA (ELIXIR-CONVERGE)
  - <a href="https://docs.google.com/spreadsheets/d/1RXrJIzHKkyB8qx5tHLQjcBioiDAOrQ3odAuqMS3pUUI/edit#gid=549383528" target="_blank">COVID-19 Host Genetics Initiative data dictionary</a>
  - <a href="https://youtu.be/AInMx8xj_Lk" target="_blank">Phenotypic metadata: the COVID-19 example</a> video produced by CSC
  - <a href="https://youtu.be/josXa1CydxA" target="_blank">Building a metadata model for COVID-19</a> video produced by CSC
- Recommended ontologies to search for concepts and terms using the **Ontology Look-up Service** (<a href="https://www.ebi.ac.uk/ols/" target="_blank">OLS</a>)
  - **Experimental Factor Ontology** (EFO): <a href="https://www.ebi.ac.uk/ols/ontologies/efo" target="_blank">ontology record</a> at OLS; EFO <a href="https://github.com/EBISPOT/efo" target="_blank">GitHub repository</a>.
  - **Data Use Conditions** (DUO): <a href="https://www.ebi.ac.uk/ols/ontologies/duo" target="_blank">ontology record</a> at OLS; DUO <a href="https://github.com/EBISPOT/DUO" target="_blank">GitHub repository</a>.

### Quality control

Coming soon!

## 3. Understand data definitions and flow

As defined in the Federated EGA Collaboration Agreement, and in alignment with definitions outlined in the GDPR, the following data definitions are used in the context of Federated EGA:

- **Administrative Data**. Data which are generated through the operation of Federated EGA. This may include personal data according to Art. 4 Nr. 1 GDPR which is directly identifying, such as names and email addresses which are used to communicate with, and support, service users. It may also include personal data and business data which are used internally by staff working on behalf of EGA Central or Federated EGA Nodes and exchanged between them.
- **Non-personal Metadata**. Information that describes or annotates research data to facilitate its interpretation or to describe the relationship between data elements that cannot be used to identify a data subject. For example, the name of the instrument used to generate the data. Non-personal metadata generated or processed by the Node will be shared with EGA Central for inclusion in a searchable, online, public metadata catalogue.
- **Personal Metadata**. Information that describes or annotates research data to facilitate its interpretation or to describe the relationship between data elements that has the potential to identify a data subject. For example, demographic or ancestry information that can be used to identify individuals. Personal metadata are not made available through a public metadata catalogue and are not shared between EGA Central and the Node.
- **Research Data**. Omics or other forms of genetic (according to Art. 4 Nr. 13 GDPR) and health data (according to Art. 4 Nr. 15 GDPR) that are used for scientific research purposes. This is considered to be special category personal data under Art. 9(1) in conjunction with Art. 4 Nr. 1 GDPR.

Here you can view how the different types of <a href="https://docs.google.com/presentation/d/1IrU5jPJpGQ7n-WH-7WvJZjjH03ww9LfFMLK1kTBeAco/edit#slide=id.gcf2c0c3039_0_126" target="_blank">data flow within the Federated EGA network</a>.

## 4. What's next?

Coming soon!
