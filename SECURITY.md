#Security Policy: Guardian Framework

#Report Vulnerabilites

*Email: All vulnerabilites are given automated detailed reports sent to admin
*If failed report, include description of vulnerability, steps to reproduce & potential impact
* Remediation MUST start within 24 Hours
  
#Automated Protectin
Every Pull Request is subject to:
*Static Analysis(SAST): CodelQL scans for logic flaws
*Secret Detection: GitGuardian scans for leaked API keys/credentials
*Dependency Auditing(SCA): Checking libraries for known CVEs
*Infrastructure Scanning: Verifying Docker and Cloud Configs
