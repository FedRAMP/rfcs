

FedRAMP® Review   
Initiation Checks (RIC)

Part 1: Pre-Assessment 

 

\<Version ALPHA\>

\<2024-12-26\>

TABLE OF CONTENTS

[**Overview	2**](#overview)

[Check 1: Scope	4](#check-1:-scope)

[Check 2: Visibility	5](#check-2:-visibility)

[Check 3: Governance	5](#check-3:-governance)

[Check 4: SSP Front Matter and Attachments/Appendices	6](#check-4:-ssp-front-matter-and-attachments/appendices)

[Check 4A: ISCP and CP test report	6](#check-4a:-iscp-and-cp-test-report)

[Check 4B: Rationale for N/A controls	7](#check-4b:-rationale-for-n/a-controls)

[Check 4C: Consistency between CRM and SSP	7](#check-4c:-consistency-between-crm-and-ssp)

[Check 4D: Diagram readability and consistency	8](#check-4d:-diagram-readability-and-consistency)

[Check 4E: ABD and narrative consistency	9](#check-4e:-abd-and-narrative-consistency)

[Check 4F: Interconnected external services with federal data/metadata	9](#check-4f:-external-services-with-federal-data/metadata)

[Check 4G: Architecture documentation content review	10](#check-4g:-architecture-documentation-content-review)

[Check 4H: Data flow documentation review	11](#check-4h:-data-flow-documentation-review)

[Check 4I: CM-6 control narrative	12](#check-4i:-cm-6-control-narrative)

[Check 4J: CP-9 control narrative	13](#check-4j:-cp-9-control-narrative)

[Check 4K: IA-2 control narrative	13](#check-4k:-ia-2-control-narrative)

[Check 4L: IA-5 control narrative	14](#check-4l:-ia-5-control-narrative)

[Check 4M: IA-8 control narrative	15](#check-4m:-ia-8-control-narrative)

[Check 4N: RA-5 control narrative	16](#check-4n:-ra-5-control-narrative)

[Check 4O: SC-7 control narrative	16](#check-4o:-sc-7-control-narrative)

[Check 4P: SC-13 control narrative	16](#check-4p:-sc-13-control-narrative)

[**RIC Attestation Form	18**](#ric-attestation-form)

# **Overview**

Optional FedRAMP Review Initiation Checks (RIC) help cloud service providers, independent assessors, and federal agency partners understand how FedRAMP evaluates and verifies the completeness, consistency, accuracy, and clarity of an authorization package. Following these checks properly will enable expedited review by FedRAMP and increase the likelihood of a smooth FedRAMP authorization process.

* **RIC Part 1** may be used by the cloud service provider to self-assess after the preparation of the System Security Plan but prior to the independent security assessment of the cloud service offering. 

* **RIC Part 2** may be used by the cloud service provider to self-assess after the completion of the independent security assessment of the cloud service offering and after the preparation of the Security Assessment Plan and Security Assessment Report.

This document contains the RIC Part 1\.

# **RIC Part 1**

The cloud service provider performs the Part 1 checks on the System Security Plan and related attachments/appendices prior to the initial assessment. Each item within each check will generate one of the following results:

* Yes, indicating that this item is fully met  
* No, indicating that this item is applicable but is not fully met  
* N/A, indicating that this item does not apply (only an option for items in certain checks)

If any item within a check results in No, be aware that your cloud service offering may not be ready to undergo an assessment or have its package submitted to FedRAMP. Strongly consider addressing the deficiencies before continuing. 

The appropriate personnel to perform the checks for a cloud service offering will vary by organization. All checks require a solid understanding of cybersecurity and the cloud service offering itself. 

Some parts of checks are strictly editorial in nature – for example, ensuring that a file is present, a diagram is legible, or a plan contains all the sections specified by a template. These parts are labeled as \[Editorial\]. 

# **Check 1: Scope**

The cloud service provider must perform an analysis of the Integrated Inventory Workbook (IIW), vulnerability scans, authorization boundary diagram (ABD), and the associated SSP sections to answer the following questions.   
NOTE: For Rev. 5, see SSP Sections 8.1 and 9.1 and Appendix Q. For Rev. 4, see SSP Sections 9.2, 9.4, and 10.1.

| Are all asset types (operating systems, web servers, container images, etc.) that are listed in SSP System Diagram and System Description reflected in the IIW? | Yes No |
| :---- | :---- |
| Are raw vulnerability scan files provided in machine-readable format and with the following data fields? IP Address FQDN/hostname Ports, Protocols, Services Cryptographic modules Unique detection identifier (tool-specific) CVE identifier Relevant CVSS score CVSS temporal and environmental vectors Original detection date | Yes No |
| Are all components listed in the IIW targeted in the scans, and vice versa? | Yes No |
| Are all ports (non-ephemeral/ephemeral), protocols, and services listed in the SSP Ports & Protocols Table in alignment with open ports found in the scans? | Yes No |
| For Rev. 5, do IIW components match all listed cryptographic modules in SSP Appendix Q, and vice versa? | Yes No N/A |

 

# **Check 2: Visibility**

The cloud service provider must perform an analysis of the IIW, vulnerability scans, and POA\&M deliverables to answer the following questions:

| Are the scans performed with elevated privileges (\<10% authentication failure rate)? | Yes No |
| :---- | :---- |
| Are Network, OS, DB, Web, Container, and SAST/SCA scans performed as applicable on all IIW components? | Yes No |

# **Check 3: Governance** 

The cloud service provider must perform an analysis of the SSP (table where the System Owner, Model, and ISSO are identified) to answer the following questions.  
NOTE: FedRAMP does not review packages for private clouds, grant a FedRAMP Authorized designation, or list private clouds on the FedRAMP Marketplace because the concept of “reuse” does not apply.

| Is the deployment model for the service offering applicable to the agency's use and potential government data involved (public vs. government-only community)?  | Yes No |
| :---- | :---- |
| If applicable, does the SSP annotate why "hybrid" was selected, and does this actually apply to the service offering based on the architecture? | Yes No N/A |
| Is the deployment model listed in the SSP the same as the cloud service offering's FedRAMP Marketplace listing?  | Yes No |
| If the cloud service offering is listed as non-public, do the SSP and Access Control Policy document how customer restrictions are enforced via the sales pipeline? | Yes No N/A |
| Does the System Owner have the organizational authority to address risk for *all* components, processes, and people included in the scope of system policies (budget, resources, charter, etc.)?  | Yes No |

# **Check 4: SSP Front Matter and Attachments/Appendices**

The cloud service provider must perform the following checks around the SSP front matter and attachments/appendices.

## **Check 4A: ISCP and CP test report** 

| Does the package include an Information System Contingency Plan (ISCP)? \[Rev. 5 \-  SSP Appendix G; Rev. 4 \- SSP Attachment 6\] \[Editorial\] | Yes No |
| :---- | :---- |
| Does the ISCP include a corresponding CP test report? \[Rev. 5 \- ISCP Appendix F; Rev. 4 \- ISCP Appendix G\]  It may be included in the associated template, or it may be provided as a separate attachment. \[Editorial\] | Yes No |
| Does the ISCP use the FedRAMP ISCP Template associated with [Revision 4](https://www.fedramp.gov/assets/resources/documents/rev4/REV_4_SSP-A06-FedRAMP-ISCP-Template.docx) or [Revision 5](https://www.fedramp.gov/assets/resources/templates/SSP-Appendix-G-Information-System-Contingency-Plan-\(ISCP\)-Template.docx) (as appropriate)? Are all portions of the template present? (Information may be added to the template.) Have all sections of the template been completed? \[Editorial\] | Yes No |
| Is the CP test report from within the last 12 months? \[Editorial\] | Yes No |
| Does the CP test report include the parts (date, lessons learned, etc.) from the FedRAMP ISCP Template? Does the test indicate whether the cloud service provider is able to meet its RTO and RPO objectives? | Yes No |

## **Check 4B: Rationale for N/A controls** 

Review the CIS Worksheet tab in the CIS/CRM workbook to quickly identify the controls that are marked N/A. \[Rev. 5 \- SSP Appendix J; Rev. 4 \- SSP Attachment 9\] If there are none, this check does not apply, so skip to the next check (check 4C).  
Cloud service providers often misidentify controls as N/A when the capability exists but is not authorized for use per system policies. For example, many cloud service providers consider AC-2(2) to be N/A because temporary/emergency accounts are not used in the environment. FedRAMP considers this control to be applicable. In the AC-2(2) implementation statement, the cloud service provider should reference the policy that prohibits the creation of temporary/emergency accounts and describe any technical controls in place to prevent the creation of and/or audit unauthorized accounts.

| For each control that is marked N/A, is a rationale provided in the corresponding control implementation statement in the SSP as to why the control is not needed? \[Rev. 5 \- SSP Appendix A; Rev. 4 \- SSP Section 13\]  | Yes No |
| :---- | :---- |
| Are controls marked N/A only if they are not technically or functionally applicable to the system? | Yes No |

## **Check 4C: Consistency between CRM and SSP** 

| Do the control originations specified in the SSP Control Summary Information table match the CIS/CRM workbook entries? \[Rev. 5 \- SSP Appendix J; Rev. 4 \- SSP Attachment 9\] | Yes No |
| :---- | :---- |
| Are customer responsibilities clearly delineated in the SSP control implementation statement from the cloud service provider’s responsibilities? | Yes No |
| Do controls address what the customer must do to fulfill their responsibilities for the control?  | Yes No |
| For controls that indicate a customer responsibility, is there a corresponding entry in the CRM within the CIS/CRM workbook that addresses every distinct use case (e.g., unique services or features) where customer responsibilities apply? | Yes No |
| For controls inherited from other cloud service offering vendors, does the CRM match the vendors’ CRM lists of inheritable controls? | Yes No N/A |

## **Check 4D: Diagram readability and consistency** 

The SSP’s authorization boundary diagram (ABD), network diagram, and data flow diagram (DFD) are either included within the SSP \[Rev. 5 \- Section 8.1; Rev. 4 \- Sections 9.2, 9.4, and 10.1\] or are provided as separate attachments. Some cloud service providers choose to combine the ABD, network diagram, and DFDs into a single holistic diagram. This is acceptable.

| For all these diagram(s), is the resolution fully legible, including all characters being clearly distinguishable? \[Editorial\] | Yes No |
| :---- | :---- |
| If separate files are provided for diagrams, are all of the following true for each of those files?  The file opens properly. \[Editorial\] The specific filename is referenced in the associated SSP section with versioning information. \[Editorial\] Each diagram within the separate file(s) has the same figure number corresponding with the figure number used in the SSP. All text within the diagrams is searchable. \[Editorial\] | Yes No N/A |

## **Check 4E: ABD and narrative consistency** 

This involves comparing the ABD to the narrative sections and tables within the SSP to identify any inconsistencies in documenting the services used by the cloud service offering.

Note: For Rev. 5, see SSP Sections 8.1 and 8.2, and Tables 6.1 and 7.1. For Rev. 4, see Section 9.2, Tables 8-3 and 11-1, and Control CA-3 in Table 13-3.

| Are all flows to/from external services clearly depicted on the ABD? | Yes No |
| :---- | :---- |
| Are all services depicted on the ABD also explained in the narrative description? Are all services explained in the narrative description also depicted on the ABD? | Yes No |
| Is each external service identified either as FedRAMP Authorized or as lacking FedRAMP authorization? | Yes No |
| For each service identified as FedRAMP Authorized, does its name match the FedRAMP Marketplace naming convention? | Yes No N/A |
| For each transport service, is its destination depicted? Does supporting text describe the purpose of data delivered to its destination? | Yes No |

## **Check 4F: External services with federal data/metadata** 

| For each interconnected external service that stores/processes federal government data and/or metadata, is one of the following true? The external service is FedRAMP-authorized or FISMA-authorized at the same or higher impact level as the cloud service offering, based on the impact level (high, moderate, low) of federal government data and/or metadata that is stored/processed in the external service. The external service is either lacking a FedRAMP or FISMA authorization altogether OR is not authorized at the same or higher impact level, but there is a corresponding POA\&M that describes the cloud service provider's plans to remediate the risk by moving impacted functionality to a FedRAMP or FISMA authorized service at the same or higher impact level that describes mitigating factors that may reduce the risk.  | Yes No N/A |
| :---- | :---- |

## **Check 4G: Architecture documentation content review** 

| Are all data flows crossing the boundary depicted in the ABD and include the following? All customer and cloud service offering administrator access The flow of software releases from update services to production components (e.g., application updates or patches) Flows to the customer's site (e.g., access to agency’s identity management service) Component-to-component flows In general, depicting flows to groups such as VPCs is insufficient. cloud service providers may make reasonable exceptions, such as depicting a single flow from a scanner going to a text box that describes the components accessed by the scanner (rather than a separate flow to each scanned component). | Yes No |
| :---- | :---- |
| At a minimum, does the ABD depict access flows for the following? Customer users Customer administrators cloud service offering administrator to cloud service offering cloud service offering administrator to IaaS/PaaS console Non-human account access flows | Yes No |
| Does access flow have a high-level depiction of MFA in the ABD? | Yes No |
| Does a corresponding narrative description provide details about the ABD’s access flows? | Yes No |
| Do the ABD and narrative address the following? Authentication consistent with IA-5 (see Check 4L in RIC Part 1 and Check 5B in RIC Part 2). Authentication tokens must be generated by an identity provider (IdP) where: The IdP is inside an authorized boundary, OR The IdP authorization is at the same, or higher, impact level. Authentication tokens must be encrypted when passed through a browser. | Yes No |
| Does the ABD depict the alternate processing and storage site? Is there a corresponding narrative description? Are differences between alternate site configuration and primary site configuration depicted and described? | Yes No |
| In the network diagram, are all of the following true? Is the authoritative DNS server for external access to the cloud service offering (SC-20) depicted? Is the recursive DNS server for external access from the cloud service offering's boundary (SC-21) depicted? Is the recursive server inside a FedRAMP Authorized boundary? Are the connections from cloud service offering components to the recursive server trusted?  Are subnets clearly depicted and consistent with SSP narratives, including SC-7 control description? Do subnets adhere to structures described in the [FedRAMP Subnets White Paper](https://www.fedramp.gov/assets/resources/documents/FedRAMP_subnets_white_paper.pdf), including publicly accessible components in separate subnets and operational and management components in separate subnets? | Yes No |

## **Check 4H: Data flow documentation review** 

For the following checks, see SSP sections 8.1 and 8.2 (for Rev. 5\) and 10.1 (for Rev. 4).

| Are the DFD(s) consistent with their own narrative descriptions in the SSP and with relevant control descriptions (e.g., SC-8(1), SC-13, SC-28)? | Yes No |
| :---- | :---- |
| If multiple DFDs are used: Does each child diagram include a descriptive name that specifies what the particular diagram is depicting in relation to the parent diagram? Does the parent diagram indicate where a child diagram fits into the overall cloud service offering using the same descriptive name of the child diagram? | Yes No N/A |
| On the DFD(s), is the encryption status of all data in transit (data flows) and data at rest (data stores) clearly depicted as one of the following? Encrypted with FIPS-validated modules Encrypted without FIPS-validated modules Unencrypted data flows and stores | Yes No |
| On the DFD(s), do the flows to data stores include the following? All encryption in the management VPC Flows from management tools required for their work (log collection, scanning, etc.) Flows and stores associated with disk/block storage attached to compute components Flows and stores inside container environments | Yes No |
| Are flows for backup and alternate processing sites shown on the DFD(s)? | Yes No |
| Are network components where encryption can terminate (e.g., load balancers and firewalls) included on the DFD(s)? | Yes No |

## **Check 4I: CM-6 control narrative** 

Review the control narrative for CM-6. \[Rev. 5 \- SSP appendix A; Rev. 4 \- SSP section 13\]

| Does it explicitly specify the IT products (e.g., database, operating system, web server) where configuration settings have been applied? For example, Solaris 11 SPARC STIG – Ver. 2, Rel 9\. For Rev. 4, are all baseline configuration settings using at least CIS Benchmarks level 1 for all applicable components? For Rev. 5, are all baseline configuration settings using DoD STIGs for all applicable components? | Yes No |
| :---- | :---- |
| Does it state that all relevant STIGs have been applied based on the core DoD Security Requirement Guides (SRGs) and corresponding Technology SRGs? (e.g., Application SRG, Network SRG, Operating System SRG, Policy SRG) | Yes No |

## **Check 4J: CP-9 control narrative** 
Review the control description for CP-9. \[Rev. 5 \- SSP appendix A; Rev. 4 \- SSP section 13\] NOTE: Data must be backed up and not "mirrored" or "replicated."

| Does part (a) specify the user-level information that is being backed up, frequency and type of backups (at least daily incremental and weekly full), where backups are retained, and how many copies (at least three copies \[one copy online\])? | Yes No |
| :---- | :---- |
| Does part (b) specify the system-level information that is being backed up, frequency and type of backups (at least daily incremental and weekly full), where backups are retained, and how many copies (at least three copies \[one copy online\])? | Yes No |
| Does part (c) specify the system documentation that is being backed up, frequency and type of backups (at least daily incremental and weekly full), where backups are retained, and how many copies (at least three copies \[one copy online\])? | Yes No |

## **Check 4K: IA-2 control narrative** 

Review the control description for IA-2(6) \[Rev. 5\] or IA-2(11) \[Rev. 4\]. \[Rev. 5 \- SSP appendix A; Rev. 4 \- SSP section 13\]

| Is MFA used to authenticate into all privileged and non-privileged accounts within the authorization boundary? | Yes No |
| :---- | :---- |
| Is MFA used to authenticate at the first "hop" within the authorization boundary? For example, logging into the jump host, bastion host, server, management console, etc. | Yes No |
| Does MFA involve a separate device than the system being accessed? For example, using an authenticator app on a mobile device. | Yes No |
| Are the make and model (e.g., OTP, hardware token) of the MFA specified, as well as the FIPS-validated certificate number (if applicable)?  If the MFA is included in a FedRAMP Authorized service, is the associated leveraged service referenced? (Doing so is sufficient.) If an NSA-approved product is used, is the source document listed for obtaining information related to the NSA approval? | Yes No |
| Are all modes of MFA access consistent with those depicted in the ABD? | Yes No |
| Does each have a tool (by vendor) and protocol level (e.g., PIV, OTP, Push) depiction of MFA? | Yes No |
| Is PIV/CAC support indicated for all federal government personnel access? | Yes No |

## **Check 4L: IA-5 control narrative** 

| Does each access mode meet authenticator requirements? Low baseline, Rev. 5: MFA is required per the FedRAMP baseline. Low baseline, Rev. 4: Single-factor is acceptable per NIST SP 800-63B AAL1. Moderate baseline, Rev. 5 and Rev. 4: MFA is required per NIST SP 800-63B AAL2. High baseline, Rev. 5: MFA is required per NIST SP 800-63B AAL3. Password and hard token OTP are no longer accepted. High baseline, Rev. 4: MFA is required per NIST SP 800-63B AAL3. Password and hard token OTP will also be accepted. | Yes No |
| :---- | :---- |
| Does each access mode meet phishing resistance requirements? Low and moderate baselines, Rev. 5: Required for federal agency, contractor, and cloud service provider access. Must be an available option for public access. Low and moderate baselines, Rev. 4: Not required. High baseline, Rev. 5 and Rev. 4: Required. | Yes No |
| Does each access mode meet FIPS 140 requirements for the authenticator and the verifier?: Low baseline: Not required for authenticators. Required for verifiers. Moderate baseline: Required for federal agency, contractor, and cloud service provider access. Not required for public access. High baseline, Rev. 5: NIST SP 800-63 Rev. 3 is required until the final version of NIST SP 800-63 Rev. 4 is published and becomes effective.  High baseline, Rev. 4: A hard token is required with any FIPS 140 validation. FedRAMP will continue to accept FIPS 140 validated hard tokens. | Yes No |
| Does each access mode meet SP 800-63B requirements (e.g., soft tokens acceptable for Moderate baseline, hard tokens required for High baseline)? | Yes No |
| If the cloud service offering provides identity management as a part of the service offering, does the SSP control description include all of the following: How authentication is implemented for cloud service offering access How AAL authentication is supported for customer deployment. In particular: The cloud service offering’s capability to meet the requirements in item 1 of this check for each impact level The customer responsibilities for compliant configuration at each impact level How IAL and FAL are supported for customer deployment (as appropriate) At least one compliant configuration exists for the capabilities described for items 5b and 5c of this check | Yes No |

## **Check 4M: IA-8 control narrative** 

NOTE: This control applies regardless of whether the customer is or is not using PIV to access the service.

| Does the SSP control narrative for IA-8(1) indicate that the back-end technical implementation supports an agency customer's use of PIV (e.g., can accept SAML assertions)? Does it include having a capability in place for accepting and validating PIV when coupled with a customer’s identity provider (IdP)? | Yes No |
| :---- | :---- |

## **Check 4N: RA-5 control narrative** 

| Does the control narrative for RA-5 indicate the vulnerability scanning tool(s) used, the frequency of scanning performed (at least monthly), and the types of components being scanned (at minimum, the network infrastructure components, operating systems, databases, web applications, and container images where used)? | Yes No |
| :---- | :---- |
| Does the control narrative for RA-5(5) indicate that all of the vulnerability scans performed are via privileged or credentialed access? | Yes No |

## **Check 4O: SC-7 control narrative** 

| Is a logical or physical (where applicable/appropriate) subnet structure in place consistent with the [*FedRAMP Subnets White Paper*](https://www.fedramp.gov/assets/resources/documents/FedRAMP_subnets_white_paper.pdf)? | Yes No N/A |
| :---- | :---- |
| For the management planes and the operations planes, are their publicly accessible components in a public subnet? Are their other components in a private subnet? | Yes No |

## **Check 4P: SC-13 control narrative** 

Review the control description for SC-13 to answer the following for all components within the authorization boundary:

| For each data-in-transit (DIT) flow traversing the boundary (e.g., administrator and user access, APIs, and updates) or inside the boundary (e.g., VPC to VPC, server to server, access to IaaS/PaaS services, and backups to storage), is one of the following true? The flow is encrypted by FIPS-validated or documented NSA-approved cryptographic modules (CMs).   The flow is encrypted through the appropriate technical implementation of a FedRAMP Authorized service and completion of appropriate customer responsibilities (e.g., the use of FIPS endpoints). The flow is encrypted by CMs that are not FIPS-validated or NSA-approved, but these CMs are documented in the POA\&M. | Yes No |
| :---- | :---- |
| For each area of data-at-rest (DAR) (e.g., residing in databases, logs, backups, and storage), is one of the following true? The data-at-rest is encrypted using FIPS-validated or documented NSA-approved CMs. The data-at-rest is encrypted through the appropriate technical implementation of a FedRAMP Authorized service and completion of appropriate customer responsibilities (enabling encryption on the database, etc.) The data-at-rest is encrypted by CMs that are not FIPS-validated or NSA-approved, but these CMs are documented in the POA\&M. | Yes No |

# **RIC Attestation Form** 

The RIC attestation form is illustrated here for informational purposes. The final version of this form to be completed and submitted as part of each package will be made available in an editable form outside of this document.

 

| *The \[Federal Agency Name\], \[Cloud Service Provider Name\], and \[Independent Assessor Organization Name\]* attest that the checks from RIC Parts 1 and 2 have been completed and validated, and represent the *\[Cloud Service Offering Name\]* authorization package as accurately as possible. All failed RIC checks are documented and explained below as comments. 

Agency Partner Comments: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ 

CSP Comments: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ 

IA Comments: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ 

Agency Partner Representative: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ Date: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ 

CSP Representative: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_  Date: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ 

IA Representative: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_  Date:\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_  

|
| ----- |
| *v1.4*  |

