# Awesome OWASP Security Testing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of OWASP projects, standards, and companion tools for application security testing.

This list focuses on resources for **security testing of web apps, APIs, mobile apps, and supporting infrastructure**, anchored on OWASP flagship projects and complemented by widely-adopted open-source tools. Each entry is a real, current project — verify license, maintenance status, and version compatibility against the upstream docs before adopting.

## Contents

- [OWASP Standards and Guides](#owasp-standards-and-guides)
- [OWASP Tools](#owasp-tools)
  - [DAST and Scanners](#dast-and-scanners)
  - [Vulnerable Apps for Practice](#vulnerable-apps-for-practice)
  - [Dependency and Supply Chain](#dependency-and-supply-chain)
  - [Threat Modeling](#threat-modeling)
  - [WAF and Rule Sets](#waf-and-rule-sets)
  - [Vulnerability Management and Orchestration](#vulnerability-management-and-orchestration)
  - [Knowledge and Training](#knowledge-and-training)
- [Companion Tools](#companion-tools)
  - [DAST](#dast)
  - [SAST](#sast)
  - [SCA and SBOM](#sca-and-sbom)
  - [Secret Scanning](#secret-scanning)
  - [Infrastructure as Code Scanning](#infrastructure-as-code-scanning)
  - [Container and Runtime](#container-and-runtime)
  - [API Security](#api-security)
  - [Mobile Security](#mobile-security)
  - [Reconnaissance](#reconnaissance)
- [Standards and Frameworks (non-OWASP)](#standards-and-frameworks-non-owasp)
- [Learning Platforms](#learning-platforms)
- [Books](#books)
- [Communities and Events](#communities-and-events)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)
- [License](#license)

## OWASP Standards and Guides

- [OWASP Top 10](https://owasp.org/www-project-top-ten/) — The flagship awareness document listing the most critical web application security risks.
- [OWASP API Security Top 10](https://owasp.org/API-Security/) — Top API-specific risks (BOLA, broken authentication, mass assignment, etc.).
- [OWASP Mobile Top 10](https://owasp.org/www-project-mobile-top-10/) — Top risks for mobile applications.
- [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/) — Risks specific to applications built on large language models.
- [OWASP Web Security Testing Guide (WSTG)](https://github.com/OWASP/wstg) — Comprehensive guide for testing the security of web applications and services.
- [OWASP Mobile Application Security Testing Guide (MASTG)](https://github.com/OWASP/owasp-mastg) — Comprehensive manual for mobile app security testing and reverse engineering.
- [OWASP Application Security Verification Standard (ASVS)](https://github.com/OWASP/ASVS) — Verification requirements for designing, building, and testing application security controls.
- [OWASP Mobile Application Security Verification Standard (MASVS)](https://github.com/OWASP/owasp-masvs) — Security verification standard for mobile apps, paired with MASTG.
- [OWASP Software Assurance Maturity Model (SAMM)](https://owaspsamm.org) — A prescriptive model for assessing and improving software security posture.
- [OWASP Cheat Sheet Series](https://github.com/OWASP/CheatSheetSeries) — Concise, high-value guidance for developers and testers on specific AppSec topics.
- [OWASP Proactive Controls](https://owasp.org/www-project-proactive-controls/) — Top techniques developers should adopt to build secure software.
- [OWASP DevSecOps Guideline](https://owasp.org/www-project-devsecops-guideline/) — Reference for integrating security into CI/CD pipelines.

## OWASP Tools

### DAST and Scanners

- [OWASP ZAP](https://github.com/zaproxy/zaproxy) — Flagship open-source web application scanner with passive scanning, active attack, fuzzing, and scriptable automation.
- [OWASP Nettacker](https://github.com/OWASP/Nettacker) — Automated penetration testing and vulnerability scanning framework.
- [OWASP Amass](https://github.com/owasp-amass/amass) — Attack-surface mapping and external asset discovery via active and passive techniques.

### Vulnerable Apps for Practice

- [OWASP Juice Shop](https://github.com/juice-shop/juice-shop) — Intentionally insecure modern web application written in Node.js, with built-in challenges.
- [OWASP WebGoat](https://github.com/WebGoat/WebGoat) — Deliberately insecure Java web application used to teach AppSec lessons.
- [OWASP crAPI](https://github.com/OWASP/crAPI) — Completely Ridiculous API: a vulnerable API for practicing the API Security Top 10.
- [OWASP Mutillidae II](https://github.com/webpwnized/mutillidae) — Free, open, deliberately vulnerable PHP web application.
- [OWASP Security Shepherd](https://github.com/OWASP/SecurityShepherd) — Web and mobile application security training platform with lessons and CTF mode.

### Dependency and Supply Chain

- [OWASP Dependency-Check](https://github.com/dependency-check/DependencyCheck) — SCA tool that identifies project dependencies and checks them against known vulnerability databases. (The former `jeremylong/DependencyCheck` repo was archived on 2025-09-27 and superseded by this org.)
- [OWASP Dependency-Track](https://github.com/DependencyTrack/dependency-track) — Continuous SBOM analysis platform for managing component risk across portfolios.
- [OWASP CycloneDX](https://cyclonedx.org) — Lightweight SBOM standard designed for application security and supply-chain risk.

### Threat Modeling

- [OWASP Threat Dragon](https://github.com/OWASP/threat-dragon) — Open-source threat modeling tool with web and desktop versions; supports STRIDE and LINDDUN.
- [OWASP pytm](https://github.com/OWASP/pytm) — Pythonic framework for threat modeling: define your system in code, generate diagrams and threat reports.

### WAF and Rule Sets

- [OWASP Core Rule Set (CRS)](https://github.com/coreruleset/coreruleset) — Set of generic attack-detection rules for ModSecurity-compatible WAFs.
- [OWASP Coraza](https://github.com/corazawaf/coraza) — Golang Enterprise-grade WAF library, compatible with ModSecurity SecLang rules and the OWASP CRS.

### Vulnerability Management and Orchestration

- [OWASP DefectDojo](https://github.com/DefectDojo/django-DefectDojo) — Open-source application vulnerability correlation and security orchestration platform.
- [OWASP SecureCodeBox](https://github.com/secureCodeBox/secureCodeBox) — Kubernetes-based orchestration platform for running and aggregating security scans at scale.

### Knowledge and Training

- [OWASP Security Knowledge Framework](https://owasp.org/www-project-security-knowledge-framework/) — Expert system that walks developers through secure coding requirements per technology and feature.
- [OWASP SamuraiWTF](https://github.com/SamuraiWTF/samuraiwtf) — Live linux environment pre-loaded with tools and vulnerable targets for web pen-testing practice.

## Companion Tools

Tools outside the OWASP umbrella that integrate cleanly with OWASP standards and are widely used in security testing.

### DAST

- [Burp Suite](https://portswigger.net/burp) — Industry-standard web vulnerability scanner and intercepting proxy by PortSwigger; Community Edition is free.
- [Nuclei](https://github.com/projectdiscovery/nuclei) — Fast, template-based vulnerability scanner driven by a large community template library.
- [Nikto](https://github.com/sullo/nikto) — Long-running open-source web server scanner that tests for outdated software and common misconfigurations.
- [sqlmap](https://github.com/sqlmapproject/sqlmap) — Automatic SQL injection detection and exploitation tool.
- [Wapiti](https://github.com/wapiti-scanner/wapiti) — Web application vulnerability scanner that fuzzes scripts and forms for common injection flaws.

### SAST

- [Semgrep](https://github.com/semgrep/semgrep) — Lightweight static analysis for many languages, driven by pattern rules; strong AppSec rule packs.
- [CodeQL](https://github.com/github/codeql) — Semantic code analysis engine from GitHub; treats code as data you can query.
- [Bandit](https://github.com/PyCQA/bandit) — Security linter for Python code.
- [Brakeman](https://github.com/presidentbeef/brakeman) — Static analysis security scanner for Ruby on Rails.
- [gosec](https://github.com/securego/gosec) — Inspects Go source code for security problems by AST analysis.
- [njsscan](https://github.com/ajinabraham/njsscan) — Static security scanner for Node.js applications powered by libsast and semgrep.

### SCA and SBOM

- [Trivy](https://github.com/aquasecurity/trivy) — All-in-one scanner for containers, file systems, git repos, IaC, and Kubernetes; SBOM-aware.
- [Grype](https://github.com/anchore/grype) — Vulnerability scanner for container images and filesystems.
- [Syft](https://github.com/anchore/syft) — SBOM generator for container images and filesystems; output to CycloneDX, SPDX, and others.
- [OSV-Scanner](https://github.com/google/osv-scanner) — Frontend to the OSV.dev database; scans lockfiles and SBOMs for known vulnerabilities.
- [Snyk Open Source CLI](https://github.com/snyk/cli) — Commercial SCA tool with a free tier; covers many ecosystems.

### Secret Scanning

- [Gitleaks](https://github.com/gitleaks/gitleaks) — SAST tool for detecting hardcoded secrets like passwords, API keys, and tokens in git repos.
- [TruffleHog](https://github.com/trufflesecurity/trufflehog) — Finds and verifies leaked credentials by scanning repos, S3, and other sources.
- [detect-secrets](https://github.com/Yelp/detect-secrets) — Pre-commit-friendly secrets scanner from Yelp with baseline-based suppression.

### Infrastructure as Code Scanning

- [Checkov](https://github.com/bridgecrewio/checkov) — Static analysis for Terraform, CloudFormation, Kubernetes, Helm, ARM, and more.
- [tfsec](https://github.com/aquasecurity/tfsec) — Security scanner for Terraform code (now part of the Trivy project).
- [KICS](https://github.com/Checkmarx/kics) — Find security vulnerabilities, compliance issues, and IaC misconfigurations across many IaC platforms.
- [Terrascan](https://github.com/tenable/terrascan) — IaC scanner that detects compliance and security violations.

### Container and Runtime

- [Falco](https://github.com/falcosecurity/falco) — Cloud-native runtime security tool that detects abnormal behavior using kernel events.
- [Clair](https://github.com/quay/clair) — Open-source project for static analysis of vulnerabilities in container images.
- [Dockle](https://github.com/goodwithtech/dockle) — Container image linter for security, helping build best-practice Docker images.
- [kube-bench](https://github.com/aquasecurity/kube-bench) — Checks whether Kubernetes is deployed securely per the CIS Kubernetes Benchmark.
- [kube-hunter](https://github.com/aquasecurity/kube-hunter) — Hunts for security weaknesses in Kubernetes clusters.

### API Security

- [Schemathesis](https://github.com/schemathesis/schemathesis) — Property-based testing for OpenAPI, GraphQL, and other API schemas; finds bugs the spec implies must not exist.
- [Postman / Newman](https://github.com/postmanlabs/newman) — Command-line collection runner for Postman; useful for embedding API security checks into CI.
- [Akto](https://github.com/akto-api-security/akto) — Open-source API security testing platform with traffic-aware test generation.
- [Insomnia](https://github.com/Kong/insomnia) — Open-source API client useful for manual API exploration alongside automated scans.

### Mobile Security

- [MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF) — Mobile Security Framework for automated, all-in-one mobile app pentesting (Android/iOS/Windows) — SAST, DAST, and API testing.
- [Frida](https://github.com/frida/frida) — Dynamic instrumentation toolkit for developers, reverse engineers, and security researchers.
- [Objection](https://github.com/sensepost/objection) — Runtime mobile exploration toolkit powered by Frida.
- [APKLeaks](https://github.com/dwisiswant0/apkleaks) — Scan APK files for URIs, endpoints, and secrets.

### Reconnaissance

- [Nmap](https://nmap.org) — De facto standard network scanner for host discovery and service/version detection.
- [Subfinder](https://github.com/projectdiscovery/subfinder) — Fast passive subdomain enumeration tool.
- [httpx](https://github.com/projectdiscovery/httpx) — Fast, multi-purpose HTTP toolkit that probes hosts and pulls metadata at scale.
- [Metasploit Framework](https://github.com/rapid7/metasploit-framework) — World's most-used penetration testing framework, with thousands of exploits and auxiliary modules.

## Standards and Frameworks (non-OWASP)

- [NIST SP 800-115](https://csrc.nist.gov/publications/detail/sp/800-115/final) — Technical Guide to Information Security Testing and Assessment.
- [PTES — Penetration Testing Execution Standard](http://www.pentest-standard.org) — Community-developed standard covering pentest methodology end-to-end.
- [MITRE ATT&CK](https://attack.mitre.org) — Globally accessible knowledge base of adversary tactics and techniques based on real-world observation.
- [CWE Top 25](https://cwe.mitre.org/top25/) — The most dangerous software weaknesses, maintained by MITRE.
- [CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks) — Consensus-developed secure-configuration guidelines for systems, cloud, and applications.

## Learning Platforms

- [PortSwigger Web Security Academy](https://portswigger.net/web-security) — Free, hands-on web security training from the makers of Burp Suite.
- [Hack The Box](https://www.hackthebox.com) — Penetration-testing labs and challenges, ranging from beginner to expert.
- [TryHackMe](https://tryhackme.com) — Guided learning paths and rooms for offensive and defensive security topics.
- [PentesterLab](https://pentesterlab.com) — Exercises focused on web application vulnerabilities and exploitation.
- [VulnHub](https://www.vulnhub.com) — Collection of downloadable vulnerable VM images for offline practice.
- [Pwning OWASP Juice Shop](https://pwning.owasp-juice.shop) — Companion book and walkthrough for the Juice Shop challenges.

## Books

- *The Web Application Hacker's Handbook* (2nd ed.) — Stuttard & Pinto, Wiley, 2011.
- *The Tangled Web* — Michal Zalewski, No Starch Press, 2011.
- *Real-World Bug Hunting* — Peter Yaworski, No Starch Press, 2019.
- *Hacking APIs* — Corey Ball, No Starch Press, 2022.
- *The Hacker Playbook 3* — Peter Kim, Secure Planet, 2018.
- *Black Hat Python* (2nd ed.) — Justin Seitz & Tim Arnold, No Starch Press, 2021.
- *Bug Bounty Bootcamp* — Vickie Li, No Starch Press, 2021.

## Communities and Events

- [OWASP Global AppSec](https://owasp.org/events/) — Flagship OWASP conferences held annually in multiple regions.
- [OWASP Chapters](https://owasp.org/chapters/) — Local meetups around the world; a good entry point for the community.
- [DEF CON](https://defcon.org) — One of the world's largest hacker conferences.
- [Black Hat](https://www.blackhat.com) — Information security event series with technical training and briefings.
- [BSides](http://www.securitybsides.com) — Community-driven framework for local security conferences.

## Related Awesome Lists

- [awesome-security](https://github.com/sbilly/awesome-security) — Broad security tools and resources list.
- [awesome-pentest](https://github.com/enaqx/awesome-pentest) — Penetration testing resources, tools, and references.
- [awesome-web-security](https://github.com/qazbnm456/awesome-web-security) — Web security materials and resources.
- [awesome-appsec](https://github.com/paragonie/awesome-appsec) — Application security learning resources.
- [awesome-api-security](https://github.com/arainho/awesome-api-security) — API security tools, talks, and references. *(Archived May 2026 — useful as a historical reference.)*
- [awesome-mobile-security](https://github.com/vaib25vicky/awesome-mobile-security) — Mobile security resources for Android and iOS.
- [awesome-fuzzing](https://github.com/cpuu/awesome-fuzzing) — Fuzzing tools, papers, and resources.

## Contributing

Contributions are welcome. Open a pull request that:

1. Adds a project only if it is **actively maintained** (commit or release within the last 12 months) or is a recognized historical reference.
2. Places the entry in the most specific existing section, alphabetized within that section.
3. Uses the format: `- [Project name](url) — Short, neutral description ending in a period.`
4. Avoids marketing language, superlatives, or unverified claims.
5. Prefers OSS projects; commercial tools are accepted only when they have no comparable OSS equivalent or are de-facto industry standards.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.
