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

Effectively there is no "ASD hardening guidance" for PDF applications, and thehe Adobe vendor hardening guidance is more a specification document rather than a hardening guide which means we need to look elsewhere.

The two recommended options would be:

- US DOD STIGS
  - [NIST Adobe Acrobat Reader DC Continuous Track STIG Ver2, Rel3 Checklist Details](https://ncp.nist.gov/checklist/666)
- CIS Benchmark
