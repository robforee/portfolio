# log4j Vulnerability

* Review guidance, advisories and references to understand the scope of the problem.
* Configure exploitation monitoring alerts and WAF mitigation rules for immediate tactical awareness.
* Scan for vulnerable systems using CISA log4j scanner to guide remediation efforts.

## CVE
* [CVE-2021-44228](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-44228)
* [CVE-2021-45046](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-44832)
* [CVE-2021-4104](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-4104)

## Advisory
[CISA / Five Eyes mitigation advisory (2021-12-22)](https://www.cisa.gov/uscert/ncas/alerts/aa21-356a)
[CISA Log4j (CVE-2021-44228) Vulnerability Guidance](https://github.com/cisagov/log4j-affected-db)

## Alert and Mitigation
* Disable Log4j library. 
* Disable JNDI lookups or disable remote codebases.
* Disconnect affected stacks. 
* Isolate the system. 
* Deploy a properly configured Web Application Firewall (WAF) in front of the solution stack. 
* Apply micropatch. 
* Report incidents promptly to CISA and/or the FBI here.

## Detection
[cisagov/log4j-scanner](https://github.com/cisagov/log4j-scanner)

## Exploitation
[GreyNoise log4j monitoring](https://www.greynoise.io/viz/query/?gnql=tags%3A%22Apache%20Log4j%20RCE%20Attempt%22) - GreyNoise analyzes Internet background noise. Use GreyNoise to remove pointless security alerts, find compromised devices, or identify emerging threats.

