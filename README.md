# ASD Essential Eight PLY

This is a repository for further guidance on the Australian Signals Directorate (ASD) Essential Eight, often refered to as the "Essential 8" or "E8".

Authoritative source is the [Essential Eight](https://www.cyber.gov.au/resources-business-and-government/essential-cybersecurity/essential-eight) webpage.

Trivia: The essential eight is derrived from ASD's [Strategies to migigate cyber security incidents]https://www.cyber.gov.au/resources-business-and-government/essential-cyber-security/strategies-mitigate-cyber-security-incidents) of which there are 37 in total.

## User application hardening

### PDF Applications

PDF software is hardened using ASD and vendor hardening guidance, with the most restrictive guidance taking precedence when conflicts occur.

Derrived from these ISM controls:

> **Control: ISM-1670; Revision: 1; Updated: Jun-25; Applicability: NC, OS, P, S, TS; Essential Eight: ML2, ML3**
> PDF applications are blocked from creating child processes.

> **Control: ISM-1860; Revision: 3; Updated: Jun-25; Applicability: NC, OS, P, S, TS; Essential Eight: ML2, ML3**
> PDF applications are hardened using ASD and vendor hardening guidance, with the most restrictive guidance taking precedence when conflicts occur.

> **Control: ISM-1824; Revision: 1; Updated: Jun-25; Applicability: NC, OS, P, S, TS; Essential Eight: ML2, ML3**
> PDF application security settings cannot be changed by users.

ISM also references:

> Further information on hardening Adobe Reader and Adobe Acrobat can be found in [Adobe’s Security Configuration Guide for Acrobat publication](https://www.adobe.com/devnet-docs/acrobatetk/tools/AppSec/index.html).

#### Adobe Acrobat

Effectively there is no "ASD hardening guidance" for PDF applications. Adobe's guidance is more a set of considerations and specification documents rather than a hardening guide which means its useful to look elsewhere.

- Adobe
  - [Adobe’s Security Configuration Guide for Acrobat publication](https://www.adobe.com/devnet-docs/acrobatetk/tools/AppSec/index.html)
  - [Preference Reference for Acrobat and Adobe Reader](https://www.adobe.com/devnet-docs/acrobatetk/tools/PrefRef/Windows/index.html)

The two recommended options would be:

- US DOD STIGS
  - [NIST Adobe Acrobat Reader DC Continuous Track STIG Ver2, Rel3 Checklist Details](https://ncp.nist.gov/checklist/666)
- US National Security Agency (NSA)
  - [Recommendations for Configuring Adobe Acrobat Reader DC in a Windows Environment](https://media.defense.gov/2022/Jan/20/2002924940/-1/-1/1/CTR_CONFIGURING_ADOBE_ACROBAT_READER_20220120.PDF)

#### Microsoft Edge, PDF reader

There isn't a lot of detail on whether Edge's PDF reader needs hardening, in the [Microsoft Edge Enterprise documentation](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-browser-policies/viewxfapdfiniemodeallowedfilehash) there is only two settings relating to the PDF reader which don't look recommended.

They do have this [Video](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-video-pdf-reader) but it doesn't seem to add much.

### Browser

#### Microsoft Edge

https://learn.microsoft.com/en-us/deployedge/microsoft-edge-policies
