# RFC-0002 - Proposed Revisions to FedRAMP 3PAO Requirements

FedRAMP Recognized 3PAOs –

As a part of FedRAMP’s ongoing commitment to improvement and stakeholder
engagement, a 3PAO strategy session was held in FY24 to collaborate on solutions
for addressing current challenges faced by both FedRAMP and FedRAMP recognized
3PAOs. Specifically, two main challenge areas were discussed:

1. FedRAMP highlighted the persistence of assessment deliverables that did not
   meet FedRAMP performance standards around documentation quality and testing
   accuracy/completeness, which resulted in multiple security package
   resubmissions.

2. The 3PAO participants expressed their concerns regarding the high costs of
   training junior staff, which was inhibiting team growth.

At the conclusion of the session, a consensus was made that the best approach to
address these challenge areas was to revise FedRAMP’s 3PAO requirements around
training and certifications to minimize 3PAO personnel training costs while also
ensuring assessors were sufficiently trained to produce high quality products to
the federal government.

As a next step, FedRAMP worked with the American Association for Laboratory
Accreditation (A2LA) to identify how to best revise FedRAMP’s 3PAO policy
([A2LA R311 – Specific Requirements: Federal Risk and Authorization Management Program (FedRAMP)](https://a2la.qualtraxcloud.com/ShowDocument.aspx?ID=5621)),
which is published, maintained, and enforced by A2LA. This collaboration
resulted in the following general and personnel proposed requirement revisions
(italicized) organized by the section they appear in the current version of the
A2LA R311:

## General Requirements

### Requirement 4.5:

Participation in the Baltimore Cyber Range (BCR) technical participation
activity was expanded to include an individual testing exercise for penetration
testers.

_BCR Cyber Penetration Tester Technical Proficiency Activity_

_The BCR Cyber Penetration Tester Technical Proficiency Activity is an
individual certification obtained by the penetration tester which consists of a
multiple-choice written evaluation and a real-time assessment of a multi-server
network environment. Both the written and network evaluation are conducted
remotely with the penetration tester utilizing a third party assessment
organization (3PAO) workstation for evaluation access._

_The written evaluation provides the practitioners an opportunity to demonstrate
basic penetration knowledge while the assessment exercise evaluates the
practitioner’s ability to perform a penetration test and identify issues of a
compromised network. To assure fairness, practitioners are provided a common
suite of industry standard tools. Note, the penetration tester must have
sufficient knowledge of Kali Linux and Metasploit tools to perform the technical
testing activities. Network external and internal Kali Linux/Metasploit servers
are provided for practitioner use. The target system includes Windows
workstations, Linux servers, Windows servers, and a pfSense router. The
practitioner must map system component implementation and configuration issues
to NIST SP 800-53A controls and/or control enhancements identified for each
individual evaluation activity. Actual exam content varies per individual
tester._

_Five NIST SP 800-53A controls/control enhancements are presented for
evaluation. The activity is intended to demonstrate a practitioner’s ability to
test and accurately identify evidence/artifacts required to document
non-compliant security controls in the multi-server network environment. The
provided Penetration Evaluation Test Report (PETR) template is the testing
activity report document._

_Participation Details_

_The evaluations are completed remotely. Zoom, a compatible browser, high-speed
internet access, access to the assessors’ email account, and a workstation
camera (to support Zoom) are the key system evaluation requirements. Access to
the evaluation network is provided via browser. Required credentials are
provided at the start of the evaluation._

**Impact and Rationale:** Currently, only senior and junior assessors are
required to demonstrate their FedRAMP assessment competencies by taking and
passing the BCR technical proficiency exercise. Penetration testers will now
also be expected to take and pass a technical exercise focused on how to perform
a penetration test based on FedRAMP standards. This will enable FedRAMP and
3PAOs to ensure penetration testers have the minimum qualifications needed to
successfully perform a FedRAMP-specific penetration test.

## Personnel Requirements

### Requirement 6.1.1 F.2:

The senior assessor role’s experience and certification levels were revised for
closer alignment with the DoD 8140 Cyber Workforce Qualification Program
certification requirements for training, certifying, and managing a
cybersecurity workforce.

> _3PAOs must employ at least one_ “senior assessor” _for each FedRAMP
> assessment, regardless of the type of assessment. This individual_ is
> accountable for the overall quality of deliverables and signs off on
> assessment _activities performed by the rest of the team._ A senior assessor
> must have at least five years of auditing and/or assessment experience _and
> maintain at least two certifications, where at least one certification must be
> from the Tier 1 Certifications list (below) and an additional certification
> from either of the associated certification tiers (i.e., Tier 1 or Tier 2)
> annotated below._
>
> A senior assessor must have at least five years of auditing and/or assessment
> experience _and maintain at least two certifications, where at least one
> certification must be from the Tier 1 Certifications list (below) and an
> additional certification from either of the associated certification tiers
> (i.e., Tier 1 or Tier 2) annotated below:_
>
> - **Tier 1 Certifications**
>
>   - _Certified Information Systems Security Professional or Associate (CISSP
>     or Associate)_
>   - _CISSP-Information Systems Security Architecture Professional
>     (CISSP-ISSAP)_
>   - _CISSP-Information Systems Security Engineering Professional
>     (CISSP-ISSEP)_
>   - _CISSP-Information Systems Security Management Professional (CISSP-ISSMP)_
>   - _Certified Cloud Security Professional (CCSP)_
>   - _CompTIA Advanced Security Practitioner (CASP+)_
>   - Certified Information Systems Auditor (CISA)
>   - Certified Information Security Manager (CISM)
>   - _GIAC Certified Enterprise Defender (GCED)_
>   - _GIAC Certified Incident Handler (GCIH)_
>   - _GIAC Security Leadership (GSLC)_
>   - _CyberSec First Responder (CFR)_
>   - _Certified Chief Information Security Officer (CCISO)_
>
> - **Tier 2 Certifications**
>   - _Governance, Risk, and Compliance Certification (CGRC)_
>   - _AWS Certified Solutions Architect – Associate, Professional, or Security
>     Specialty_
>   - _Azure Security Engineer Associate_
>   - _Google Professional Cloud Architect_
>   - _Oracle Cloud Infrastructure Architect_
>   - _GIAC Systems and Network Auditor (GSNA)_
>   - _GIAC Security Essentials (GSEC)_
>   - _CompTIA Cybersecurity Analyst (CySA+)_
>   - _CompTIA Cloud+ (Cloud+)_
>   - _CompTIA Security+ (Security+)_
>   - _Certificate of Cloud Security Knowledge (CCSK)_
>   - _Global Industrial Cyber Security Professional (GICSP)_

**Impact and Rationale**: 3PAOs indicated that it was critical for their
organizations to align FedRAMP personnel certification requirements with other
major government compliance programs to allow maximum flexibility for how they
staff assessments.

### Requirement 6.1.1 F.3:

The penetration tester role’s experience and certification levels were revised
for closer alignment with the DoD 8140 Cyber Workforce Qualification Program
certification requirements for training, certifying, and managing a
cybersecurity workforce.

> 3PAOs must have a personnel type that is a “penetration tester”, _for each
> FedRAMP assessment, that_ has the technical competence to perform a
> _penetration test as part of the assessment scope. This individual must have_
> the technical competence to be able to _lead the_ penetration test, in
> accordance with FedRAMP Penetration Test Guidance and requirements. This
> person must _also_ be proficient in _planning, executing, and reporting on all
> facets of the penetration test._ A 3PAO penetration tester must have two years
> of penetration testing experience and at least one industry certification
> related to enhancing the knowledge and skills needed to perform penetration
> testing activities from the following list:
>
> - Cisco Certified Network Professional Security (CCNP Security)
> - CompTIA Advanced Security Practitioner (CASP+) Continuing Education (CE)
> - Certified Information Systems Security Professional (CISSP)
> - Certified Secure Software Lifecycle Professional (CSSLP)
> - CISSP-Information Systems Security Engineering Professional (CISSP-ISSEP)
> - SANS GIAC Penetration Tester (GPEN)
> - GIAC Certified Enterprise Defender (GCED)
> - Certified Ethical Hacker (CEH)
> - Cisco Certified Network Associate-Cyber-Ops (CCNA Cyber Ops)
> - Computer Hacking Forensics Investigator (CHFI)
> - GIAC Certified Forensic Analyst (GCFA)
> - CompTIA PenTest+
> - _OffSec Certified Professional (OSCP)_
> - _OffSec Web Expert (OSWE)_
> - _OffSec Experienced Pentester (OSEP)_
> - _OffSec Web Assessor (OSWA)_
> - _Certified Professional Penetration Tester (eCPPT)_
> - _Web Application Penetration Tester (eWPT)_
> - _Web Application Penetration Tester eXtreme (eWPTX)_
> - _Hack the Box Certified Penetration Testing Specialist (HTB CPTS)_
> - _Burp Suite Certified Practitioner_

**Impact and Rational:** 3PAOs indicated that it was critical for their
organizations to align FedRAMP personnel certification requirements with other
major government compliance programs to allow maximum flexibility for how they
staff assessments.

### Requirement 6.1.1 F.4:

The certification requirements for the junior assessor role were removed.

**Impact and Rationale:** 3PAOs indicated that a more cost effective approach to
train their junior assessor personnel was for their organizations to develop a
robust FedRAMP-specific organizational training program (see Appendix A below).
Additionally, by not requiring specific certifications for their junior assessor
staff, 3PAOs have more flexibility to hire junior level assessors and have them
immediately support assessments under the supervision of their senior assessor
leads.

### Requirement 6.1.5 F.1:

3PAO organizational training program requirements were further defined to
include specific FedRAMP knowledge areas for all personnel who perform FedRAMP
assessments. These specific FedRAMP knowledge areas are mentioned in Appendix A
below.

> 3PAOs must develop an organizational training program for _all_ its personnel
> _(not only specific to the “senior assessor” and “penetration tester” roles)_
> including content incorporating continuing professional education (CPE)
> credits for _the_ FedRAMP _knowledge areas specified in Appendix A._ Training
> shall comprise a minimum of 6 hours for each of the FedRAMP knowledge areas
> _mentioned in Appendix A_. 3PAOs must maintain a list of all training courses
> planned for the year and a statement for each item on the list as to how the
> training is related to these knowledge areas. The training plan must be based
> on the employee role in the assessment team and shall clearly delineate the
> intent of the plan for that individual role. The overall organizational
> training program will be analyzed to determine if there is sufficient
> technical training of assessors for understanding FedRAMP.

**Impact and Rationale:** 3PAOs indicated that a more cost effective approach to
train their junior assessor personnel is for their organizations to develop a
robust FedRAMP-specific internal training program based on knowledge areas
prescribed by FedRAMP. This training program will provide specific elements that
FedRAMP requires 3PAO personnel to be trained on based on common issue areas
found in 3PAO assessment deliverables and establishes a level of training
consistency across all 3PAOs in the program.

### Requirement 6.1.5 F.2:

The number required annual training hours for 3PAO personnel was reduced from 32
to 24 hours.

> All authorized 3PAO personnel must complete at least _24_ hours of training
> annually under the training program detailed in 6.1.5 F.1. These training
> hours may be completed through other accreditation programs with the
> completion of Continuing Professional Education (CPEs) or equivalent, as long
> as the hours are defined adequately within 6.1.5 F.1, above. The sign off on
> successful completion of the CPEs is required and records shall be maintained.
> Also, the _24_ hours of training annually is in addition to the mandatory
> training released by FedRAMP.

**Impact and Rationale:** 3PAOs expressed concern that 32 hours of individual
personnel training was overly burdensome for their organizations financially,
especially for organizations with large teams, due to also being required to
maintain personnel certifications and BCR proficiency training. As an
alternative, 3PAOs will need to implement a more structured internal training
program for all of their personnel that incorporates FedRAMP-specific knowledge
areas as specified in Appendix A below.

### Appendix A FedRAMP Focus Areas for 3PAO Organizational Training Program:

Four (4) FedRAMP focus areas were defined as a basis for the development of an
internal 3PAO training program.

> 1. FedRAMP authorization boundary, dataflow, and network diagrams
>
>    1. FedRAMP Authorization Boundary Guidance
>    2. Security controls relating to the authorization boundary, dataflow, and
>       network diagrams (including all relevant security control enhancements)
>       such as: AC-20, CA-3, CM-12, SA-9, SC-7, and SI-4
>    3. Illustrating the essential elements of authorization boundary, dataflow,
>       and network diagrams to include components such as subnets, alternate
>       processing/storage sites, mobile applications, development/test
>       environments, FIPS 140 validated encryption, and multi-factor
>       authentication methods
>
> 2. FedRAMP FIPS 140-validated encryption
>
>    1. NIST Cryptographic Module Validation Program (CMVP)
>    2. FedRAMP SSP Template - Section 10
>    3. FedRAMP SSP Template Appendix Q - Cryptographic Modules Table
>    4. Security controls relating to encryption requirements (including all
>       relevant security control enhancements) such as: AC-17, AC-18, AC-19,
>       IA-5, MP-5, SC-7, SC-8, SC-13, and SC-28
>    5. NIST SP 800-63-3 Digital Identity Guidelines
>
> 3. FedRAMP NIST SP 800-53 and 800-53A security control interpretation methods
>
>    1. Understanding the differences between leveraged and inherited security
>       controls in a CSP’s SSP
>    2. How to identify security controls that are applicable vs. not applicable
>       in a CSP’s SSP
>    3. How security controls need to be documented in the CIS/CRM
>    4. How to recognize errors concerning “Configuration Settings”
>    5. How to differentiate between Control Implementation Summary (CIS)
>       designations
>    6. How to recognize inconsistencies among related security controls
>    7. How to recognize effective policies and procedures for a given security
>       control
>    8. How to determine if a security control adequately describes the who,
>       what, when, where, why, and how in a SSP’s implementation description
>    9. How to validate customer responsibilities (ensuring at least one
>       option/solution required of a customer meets FedRAMP requirements)
>
> 4. FedRAMP multi-factor authentication requirements
>    1. NIST Special Publication 800-63 (most current revision)
>       1. Differences between the IAL1, IAL2, and IAL3 identity assurance
>          levels
>          - Importance of IAL information
>          - Identity proofing user journey
>          - IAL requirements summary
>       2. Differences between the AAL1, AAL2, AAL3 authentication assurance
>          levels
>          - Importance of AAL information
>          - AAL2 permitted authenticator types, authenticator, and verifier
>            requirements
>          - AAL3 permitted authenticator types, authenticator, and verifier
>            requirements
>          - AAL requirements summary
>       3. Differences between the FAL1, FAL2, and FAL3 federated assurance
>          levels
>          - Importance of FAL information
>          - Federation threats and attacks
>          - Federation threat mitigation strategies
>          - Security Assertion Markup Language (SAML), kerberos, OpenID
>            connect/how they relate to the FAL paradigm
>    2. FedRAMP security control baseline discussion (including all relevant
>       control enhancements) such as: IA-2, IA-2(1), IA-2(2), IA-2(6), IA-5,
>       and IA-8
>    3. Overview of NIST Special Publication 800-63: Digital Identity Guidelines
>       Frequently Asked Questions
>       1. Identity proofing
>       2. Authentication
>       3. Federation and assertions
>
> All personnel in the “penetration tester” role must receive focused internal
> training on four (4) FedRAMP focus areas:
>
> 1. Vulnerability scanning versus penetration testing
>
>    1. What is penetration testing?
>       1. What is the scope of penetration testing?
>       2. Associated threat models applicable to a particular system
>       3. Penetration testing alignment with the FedRAMP security control
>          baselines
>          - Penetration testing in relationship to all FedRAMP baselines
>          - Security controls associated with penetration testing exercises
>    2. What is the scope of vulnerability scanning?
>
> 2. MITRE ATT&CK® Matrix for Enterprise
>
>    1. What is the MITRE ATT&CK® Matrix for Enterprise?
>       1. When is this used?
>       2. Why is this used?
>       3. How is this used?
>
> 3. FedRAMP mandatory attack vectors and applicability to a particular system
>
>    1. Attack Vector 1: External to Corporate
>    2. Attack Vector 2: External to CSP Target System
>    3. Attack Vector 3: Tenant to CSP Management System
>    4. Attack Vector 4: Tenant-to-Tenant
>    5. Attack Vector 5: Mobile Application as part of Target system
>    6. Attack Vector 6: Client-side Component as part of Target System
>
> 4. FedRAMP penetration testing reporting requirements
>    1. Familiarity with penetration testing rules of engagement
>    2. How are penetration testing deficiencies reported in a security
>       assessment package?

**Impact and Rationale:** This internal training program will provide specific
elements that FedRAMP requires 3PAO personnel to be trained on based on common
issue areas found in 3PAO assessment deliverables and establishes a level of
training consistency across all 3PAOs in the program.
