---
excerpt: Technical infrastructure, testing, software/hardware, SOPs, Helpdesk, and team capacity building
layout: default
title: Technical and Operational
nav_order: 4
has_children: false
has_toc: false
---
# Technical and Operational

Welcome! If you are involved in technical or operational aspects of establishing a Federated EGA node, you are in the right place. The information here covers topics related - but not limited - to technical infrastructure, testing, software/hardware, SOPs, Helpdesk, and team capacity building.

**You might find this page useful if you are:**
- a technical team leader
- responsible for procuring resources
- a software developer or engineer
- a bioinformatician
- a support officer

**By exploring these materials, you will be able to:**
- Understand guidelines and standards for establishing and operating a node
- Set up your node using the local EGA software stack
- Interact with Central EGA using RabbitMQ
- Evaluate your node implementation using the FEGA Maturity Model
- Plan your node <a href="https://docs.google.com/document/d/1r5bm-8vVeN0zTpWQZdfBsMFCwy2RJlspsCdNOzCuZD8/" target="_blank">end-to-end demonstrator</a>

## 1. Identify node requirements

### Standards

- The <a href="https://ega-archive.org/assets/files/EGA-Node-Operations-v2.pdf" target="_blank">FEGA Node Operations Guidelines</a> document gives an overview of the operational areas which require resources in order to establish and operate a Federated EGA node. The document is based on more than 10 years experience of establishing and operating the EMBL-EBI and CRG Central EGA nodes. It provides a breakdown of the operational areas of responsibility into Helpdesk Services, Technical Operations, Software Development, and IT Infrastructure.
- Federated EGA was established on the principle of implementing global, community standards, including those developed as part of <a href="https://www.ga4gh.org/" target="_blank">GA4GH</a> and <a href="https://elixir-europe.org/" target="_blank">ELIXIR</a>.
- <a href="https://www.youtube.com/watch?v=k9R8W3V3ugU" target="_blank">Overview of local EGA services and architecture</a> (19 June 2020)

### Software

A minimal Federated EGA node can be set up on your local infrastructure using the <a href="https://github.com/EGA-archive/LocalEGA" target="_blank">localEGA software (GitHub repository)</a> and the associated <a href="https://localega.readthedocs.io/" target="_blank">Readthedocs</a> webpages. It is not required to use the local EGA software suite, but it is a great option compared to developing your own Federated EGA node software from scratch.

More information about the local EGA software and its implementation can be found in this report on <a href="https://zenodo.org/record/4893191" target="_blank">implementation and documentation to create an operational EGA node</a> (2 June 2021).

### Standard Operating Procedures (SOPs)

It is useful to establish SOPs for common node operational tasks to enable consistent service delivery and streamline internal processes. Use this <a href="https://docs.google.com/document/d/1BWPL9I9PlWiea6k-vcDDwaMu3rM5FSdV_0n8u7hAQpg/edit?usp=sharing" target="_blank">template to develop SOPs for your own node</a>.

Standard interactions between Central EGA and Federated EGA node Helpdesk staff have been developed into a set of SOPs. Follow these SOPs below.

#### Shared FEGA &harr; CEGA SOPs

The following SOPs must be followed as part of current FEGA &harr; CEGA node interactions during the submission process:

- <a href="https://docs.google.com/document/d/1c5YfLqGjCmRlG0NF9lsuU6IWUrCq4u8Ug3Ye5xMrxtI/edit?usp=sharing" target="_blank">Federated EGA Request from submitter to submit to FEGA node</a>
- <a href="https://docs.google.com/document/d/1v7l_ODdh-yxyhWl8Y8R3IZC2hEy5x8KgjBQmFyEyGgw/edit?usp=sharing" target="_blank">Federated EGA Metadata Check and Release Protocol</a>

Central EGA Helpdesk have developed a set of SOPs to harmonise both user-facing processes and internal processes. Explore some examples of these SOPs below or organised in this <a href="https://drive.google.com/drive/folders/14yFvXOxRyGl-ENogIB5TdogIUdL-gmfk?usp=sharing" target="_blank">shared EGA Helpdesk SOP Google Drive</a>. Please note these are example SOPs and will need to be adapted to how your node operates!

#### Example User-facing Process SOPs
- <a href="https://docs.google.com/document/d/1gze9UW3yBN2TmFNFS3NFsHxPrdWNx-A74lFsxj8Xs_Q/edit?usp=sharing" target="_blank">Handling Incomplete Submissions</a>
- <a href="https://docs.google.com/document/d/16_5G97hUUyU2-vjHAD-Yb7XNRCE6A_PQWRWERqnDSFY/edit?usp=sharing" target="_blank">Handling Unresponsive DACs</a>
- <a href="https://docs.google.com/document/d/1NHNTmhfguAgCKyLuf1tQAdYWLAeCFBUeFYgONdd17bY/edit?usp=sharing" target="_blank">Users Sharing Credentials</a>
- <a href="https://docs.google.com/document/d/1DC_HJaePbaDomNe-99fdAyZ1d4CodBfqU2uavCcpL3g/edit?usp=sharing" target="_blank">Reporting Unreasonable Users</a>
- <a href="https://docs.google.com/document/d/1geswkX9Com_Y4bnbLEtTKd0XXG6ByuADlCsLHppf074/edit?usp=sharing" target="_blank">Changing User Institution</a>

#### Example Internal Node Process SOPs
- <a href="https://docs.google.com/document/d/1qIURMTn6-cDv9ZxVsVkJSK5SUcK7Wq-jxbFuD_6gT34/edit?usp=sharing" target="_blank">Helpdesk Ticket Management</a>
- <a href="https://docs.google.com/document/d/10GWK-iw12JF_JX0KL2aUTjsZ8G2liw2A-t_PV5Y81FY/edit?usp=sharing" target="_blank">Helpdesk Ticket Assignment</a>

## 2. Learn from current node implementations

Check-out current Federated EGA node implementations from some of the first established nodes:

- <a href="https://research.csc.fi/-/fega" target="_blank">Finnish FEGA Node</a>
- <a href="https://www.ghga.de/" target="_blank">German Human Genome-phenome Archive (GHGA)</a>
- <a href="https://ega.elixir.no/" target="_blank">Federated EGA Norway</a>
- <a href="https://fega-test.bsc.es/docs/" target="_blank">Spanish FEGA (es-FEGA)</a>
- <a href="https://nbis.se/infrastructure/sensitive-data-archive.html" target="_blank">Swedish Sensitive Data Archive</a>

### Technical requirements

{% include_relative countries_tech_stack/national_nodes_technical_stack.html %}


Hear more details about node implementations:
- <a href="https://www.youtube.com/watch?v=eEoKmMKGCc4" target="_blank">Norway, Sweden, and Finland FEGA node architecture and implementations</a> (19 June 2020)
- <a href="https://www.youtube.com/watch?v=DSd_UJyqoGU" target="_blank">Further details on the Norwegian node</a> (19 June 2020)

### Node experiences

Click a title below to read more about node experiences in the FEGA onboarding journey!

<details>
  <summary><strong>Selecting submission pilots - FEGA Sweden</strong></summary>
  <br>
  <h5>What did we do?</h5>
  
  The Swedish node selected <a href="https://www.nature.com/articles/ejhg2017130" target="_blank">SweGen</a> as its first submission pilot project a few years before the federation was officially established. This project was chosen because staff at the Swedish ELIXIR node had been engaged in it and because the data was considered a good genomic reference for the Swedish population.<br><br>
  To avoid relying on a single pilot dataset, the node eventually decided to engage with two additional projects. At that point, the node had gained a better understanding of what a good pilot project could look like. A few candidates were selected among projects that had expressed interest in depositing data at the node. Semi-structured interviews were then held with two candidate projects before they were officially selected. The local helpdesk team (at the time consisting of only two persons) was responsible for the selection process, but the final decision was made at FEGA node’s management level.<br><br>

  <h5>What went well?</h5>
  
  For the semi-structured interview, the local helpdesk team created a questionnaire. This allowed the node to collect necessary information before pilots were selected and made it easier to perform the evaluation. Asking the questions was in itself a good way to inform the candidates about the node’s expectations. The questionnaire included questions related to for example data availability, dataset details (e.g. submission type, file types and file sizes), legal matters (e.g. ethical permit and data processing agreement) and information about people that needed to be involved (e.g. their roles and their availability).<br><br>

  <h5>What could have gone better?</h5>
  
  Having a strategy already when selecting the first pilot would probably have made the node’s work more efficient. It would also have made it easier for the node to communicate its expectations to the people that represented the candidate projects. If we had selected pilots now, we would probably have selected three pilot projects already from the start.<br><br>

  <h5>What did we learn?</h5>
  
  Good communication of expectation is key to success. It is also crucial that the people you engage with have the motivation, patience and enough time to dedicate to the work.<br><br>

</details>

<details>
  <summary><strong>Selecting submission pilots - FEGA Finland</strong></summary>
  <br>
  <h5>What did we do?</h5>
  
  The Finnish node's experience differed from the Swedish node's approach. In our case, we did not proactively choose a pilot project; instead, researchers and users approached us seeking specific services critical to publishing. These services were instrumental in enabling them to publish their research papers and secure funding for their ongoing studies. These researchers faced a unique challenge: while their dataset had been consented for research use and reuse, strict restrictions prevented its transfer outside of Finland. The Finnish Federated EGA service and their integration with CSC’s services (SD Apply and SD Desktop) played a pivotal role in overcoming this obstacle. By ensuring that no additional copies of the data were created and making it accessible only via a secure virtual desktop environment, Federated EGA became natural and often the only possible solution for the researchers. While we received inquiries from numerous research projects, we faced the challenge of managing expectations due to the absence of a clear timeline for the service availability. Consequently, we had to make difficult decisions and, unfortunately, had to decline some requests to ensure the effective allocation of our resources.<br><br>

  <h5>What went well?</h5>
  
  During our collaboration with one of the research groups in the pilot phase, we established effective communication channels, including face-to-face meetings, which allowed us to understand their specific needs better. These meetings proved invaluable as they facilitated comprehensive testing of data uploads, a process that sometimes-required additional support next to the technical documentation. We also worked closely with the researchers to establish legal agreements with the data controller, in this case, the university hospital. This partnership was crucial in navigating the legal complexities surrounding data usage. This specific study, involving single-cell RNA sequencing of human cells, posed minimal data size constraints, with data totalling approximately 20 GB. This relatively small dataset size, coupled with the absence of intricate phenotype data, simplified the data submission process and contributed to the overall success of our collaboration.<br><br>

  <h5>What could have gone better?</h5>
  
  One of the primary challenges we encountered was the lack of a clearly defined timeline or the frequent postponement of timelines throughout the pilot. This uncertainty created significant frustration for both the researchers and our team. Researchers, whose careers and funding were contingent on the pilot’s progress, found it especially challenging to understand why the process was often delayed. The absence of a predictable timeline made it difficult for us to manage expectations effectively and communicate transparently about project milestones and progress. In hindsight, having a more structured and consistent timeline could have mitigated these issues and improved the overall experience for all parties involved.<br><br>

  <h5>What did we learn?</h5>
  
  The overall experience was positive, and it served as a valuable learning opportunity for our team. However, reflecting on our experience, we recognize that there were areas where we could have improved. Better planning and coordination across the nodes, as well as with the central EGA, would have greatly benefited the pilot. Aligning timelines and needs between all parties involved, including researchers, the FEGA nodes, and the central EGA, could have led to a more streamlined and efficient process. In hindsight, leveraging the operation committee could have played a pivotal role in addressing challenges collectively and finding solutions collaboratively, aligning our efforts more effectively and ensuring smoother and more productive collaborations.<br><br>

</details>
-----
<details>
  <summary><strong>Establishing data processing agreements with data controllers - FEGA Sweden</strong></summary>
  <br>
  <h5>What did we do?</h5>
  
  In order to process personal data in Sweden you must comply with the EU General Data Protection Regulation (GDPR). Since the Swedish FEGA node is formally hosted by Uppsala University, this means that a data processing agreement is needed whenever data comes from a different legal entity. To make it easier for Swedish researchers to submit data, the node decided to set up general data processing agreements with the country’s major universities.<br><br>

  <h5>What went well?</h5>
  
  When a researcher wants to submit data to the Swedish node, he or she generally doesn’t need to sign a separate data processing agreement with Uppsala university, which would have been needed if there were no general data processing agreements. Because the node has used the same template for all its general data processing agreements, all the agreements now basically look the same.<br><br>

  <h5>What could have gone better?</h5>
  
  It took the node several years to sign agreements with all the major Swedish universities. The reason for this was mainly the discussions that needed to happen with the legal experts at the different universities. It is hard to say what the node could have done differently.<br><br>

  <h5>What did we learn?</h5>
  
  General data processing agreements may require the node to develop additional operating procedures. If the data providing organization must sign a data processing agreement whenever a new dataset is deposited at the node, this will make it obvious who the data controller is for that dataset. If a general processing agreement is used instead, the node’s local helpdesk will have to verify the data controller by other means.<br><br>

</details>

<details>
  <summary><strong>Establishing data processing agreements with data controllers - FEGA Finland</strong></summary>
  <br>
  <h5>What did we do?</h5>
  
  In Finland, the Federated EGA is hosted by CSC - IT Center for Science. The landscape here is marked by a diversity of data controllers, predominantly from academic organizations, university hospitals, and biobanks. To streamline and facilitate the data submission process for researchers, we have initiated discussions with all data controllers involved to have standardized DPAs. The goal is to establish comprehensive DPAs that encompass the necessary legal requirements while simplifying the process for those wishing to deposit data with the Federated EGA. This collaborative approach aims to provide researchers with a smoother path for sharing their data within the boundaries of legal compliance.<br><br>

  <h5>What went well?</h5>
  
  In addition to supporting and receiving support from researchers throughout this process, we have also successfully raised awareness within their organizations. This proactive approach has allowed us to familiarize these entities with the legal requirements and processes of FEGA, including their involvement in establishing Data Access Committees (DACs) where necessary. By promoting a broader understanding of the service's operational framework and legal compliance, we've not only facilitated smoother interactions with researchers but also enhanced overall transparency and cooperation among the organizations involved.<br><br>

  <h5>What could have gone better?</h5>
  
  The discussions with some experts and organizations proved challenging, primarily due to the diverse expertise required to address various aspects of the agreements. The need to navigate these complexities in a more streamlined manner became evident, and we recognize the importance of finding more efficient and structured ways to engage and collaborate with these experts in the future. Moreover, the uncertainty with the timelines also had an impact on the process. This uncertainty occasionally led to delays and hindered the pace of progress. Sharing best practices and experiences with our counterparts in other nodes might have provided valuable insights and strategies to address these challenges more effectively.<br><br>

  <h5>What did we learn?</h5>
  
  Our key takeaways encompass the critical importance of organizational support, the necessity of hiring or involving domain experts, and the strategic allocation of dedicated time and resources for efficient management of this process.<br><br>

</details>
<br>

## 3. Evaluate your implementation

- Understand the domains in which a node matures using the [Federated EGA Maturity Model](../maturity-model/)
- Assess the technical and operational maturation of your node by doing a self-assessment against the [Federated EGA Maturity Model](https://docs.google.com/spreadsheets/d/1WgvwwANlRh_OPAy8RY53xfzopFMwstG08zcg3LOTyZQ/copy)
- Demonstrate the full set of node services for users by planning your <a href="https://docs.google.com/document/d/1r5bm-8vVeN0zTpWQZdfBsMFCwy2RJlspsCdNOzCuZD8/edit?usp=sharing" target="_blank">Federated EGA end-to-end demonstrator</a>
- Determine compliance of services with FEGA specifications by performing compliance tests (Coming soon!)
- Evaluate ability to scale services by performing stress tests (Coming soon!)

## 4. What's next?

To hear up-to-date progress of FEGA and discussions with existing and interested FEGA nodes in the ELIXIR Federated Human Data (FHD) Community, join the <a href="https://elixir-europe.org/intranet/join-groups" target="_blank">ELIXIR FHD Mailing List</a> (select "Human Data") and attend the <a href="https://docs.google.com/document/d/10OwVvHbJ7i1gI1Iw4zmVsOs8kDrG077Y52juehiFcmU/edit" target="_blank">ELIXIR FHD Community Calls</a>.
