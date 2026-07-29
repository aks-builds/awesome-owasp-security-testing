# Awesome OWASP Security Testing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated, centralized list of OWASP projects, standards, and companion tools spanning the wider application and product security testing landscape.

This list anchors on OWASP flagship projects and standards, then extends outward to the tools, standards bodies, vulnerability databases, certifications, and communities that application security engineers, penetration testers, red and blue teamers, and OWASP contributors rely on day to day. Each entry is a real, current project or resource — verify license, maintenance status, and version compatibility against the upstream docs before adopting.

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
  - [Cloud Security](#cloud-security)
  - [CI/CD and Supply Chain Security](#cicd-and-supply-chain-security)
  - [Fuzzing](#fuzzing)
  - [API Security](#api-security)
  - [Mobile Security](#mobile-security)
  - [AI and LLM Security](#ai-and-llm-security)
  - [Password and Credential Testing](#password-and-credential-testing)
  - [Adversary Emulation and Purple Teaming](#adversary-emulation-and-purple-teaming)
  - [Reconnaissance](#reconnaissance)
- [Standards and Frameworks (non-OWASP)](#standards-and-frameworks-non-owasp)
- [Vulnerability Databases and Disclosure](#vulnerability-databases-and-disclosure)
- [Learning Platforms](#learning-platforms)
- [Certifications](#certifications)
- [Books](#books)
- [Newsletters and Podcasts](#newsletters-and-podcasts)
- [Bug Bounty Platforms](#bug-bounty-platforms)
- [Communities and Events](#communities-and-events)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)
- [License](#license)

## OWASP Standards and Guides

- [OWASP AI Security and Privacy Guide](https://github.com/OWASP/www-project-ai-security-and-privacy-guide) — Guidance on securing and governing AI/ML systems across the development and deployment lifecycle.
- [OWASP API Security Top 10](https://owasp.org/API-Security/) — Top API-specific risks (BOLA, broken authentication, mass assignment, etc.).
- [OWASP Application Security Verification Standard (ASVS)](https://github.com/OWASP/ASVS) — Verification requirements for designing, building, and testing application security controls.
- [OWASP Cheat Sheet Series](https://github.com/OWASP/CheatSheetSeries) — Concise, high-value guidance for developers and testers on specific AppSec topics.
- [OWASP DevSecOps Guideline](https://owasp.org/www-project-devsecops-guideline/) — Reference for integrating security into CI/CD pipelines.
- [OWASP Machine Learning Security Top 10](https://github.com/OWASP/www-project-machine-learning-security-top-10) — Top risks specific to machine learning systems and pipelines.
- [OWASP Mobile Application Security Testing Guide (MASTG)](https://github.com/OWASP/owasp-mastg) — Comprehensive manual for mobile app security testing and reverse engineering.
- [OWASP Mobile Application Security Verification Standard (MASVS)](https://github.com/OWASP/owasp-masvs) — Security verification standard for mobile apps, paired with MASTG.
- [OWASP Mobile Top 10](https://owasp.org/www-project-mobile-top-10/) — Top risks for mobile applications.
- [OWASP Proactive Controls](https://owasp.org/www-project-proactive-controls/) — Top techniques developers should adopt to build secure software.
- [OWASP Software Assurance Maturity Model (SAMM)](https://owaspsamm.org) — A prescriptive model for assessing and improving software security posture.
- [OWASP Top 10](https://owasp.org/www-project-top-ten/) — The flagship awareness document listing the most critical web application security risks.
- [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/) — Risks specific to applications built on large language models.
- [OWASP Web Security Testing Guide (WSTG)](https://github.com/OWASP/wstg) — Comprehensive guide for testing the security of web applications and services.

## OWASP Tools

### DAST and Scanners

- [OWASP Amass](https://github.com/owasp-amass/amass) — Attack-surface mapping and external asset discovery via active and passive techniques.
- [OWASP Nettacker](https://github.com/OWASP/Nettacker) — Automated penetration testing and vulnerability scanning framework.
- [OWASP ZAP](https://github.com/zaproxy/zaproxy) — Flagship open-source web application scanner with passive scanning, active attack, fuzzing, and scriptable automation.

### Vulnerable Apps for Practice

- [OWASP crAPI](https://github.com/OWASP/crAPI) — Completely Ridiculous API: a vulnerable API for practicing the API Security Top 10.
- [OWASP Juice Shop](https://github.com/juice-shop/juice-shop) — Intentionally insecure modern web application written in Node.js, with built-in challenges.
- [OWASP Mutillidae II](https://github.com/webpwnized/mutillidae) — Free, open, deliberately vulnerable PHP web application.
- [OWASP Security Shepherd](https://github.com/OWASP/SecurityShepherd) — Web and mobile application security training platform with lessons and CTF mode.
- [OWASP WebGoat](https://github.com/WebGoat/WebGoat) — Deliberately insecure Java web application used to teach AppSec lessons.

### Dependency and Supply Chain

- [OWASP CycloneDX](https://cyclonedx.org) — Lightweight SBOM standard designed for application security and supply-chain risk.
- [OWASP Dependency-Check](https://github.com/dependency-check/DependencyCheck) — SCA tool that identifies project dependencies and checks them against known vulnerability databases. (The former `jeremylong/DependencyCheck` repo was archived on 2025-09-27 and superseded by this org.)
- [OWASP Dependency-Track](https://github.com/DependencyTrack/dependency-track) — Continuous SBOM analysis platform for managing component risk across portfolios.

### Threat Modeling

- [OWASP pytm](https://github.com/OWASP/pytm) — Pythonic framework for threat modeling: define your system in code, generate diagrams and threat reports.
- [OWASP Threat Dragon](https://github.com/OWASP/threat-dragon) — Open-source threat modeling tool with web and desktop versions; supports STRIDE and LINDDUN.

### WAF and Rule Sets

- [OWASP Coraza](https://github.com/corazawaf/coraza) — Golang Enterprise-grade WAF library, compatible with ModSecurity SecLang rules and the OWASP CRS.
- [OWASP Core Rule Set (CRS)](https://github.com/coreruleset/coreruleset) — Set of generic attack-detection rules for ModSecurity-compatible WAFs.

### Vulnerability Management and Orchestration

- [OWASP DefectDojo](https://github.com/DefectDojo/django-DefectDojo) — Open-source application vulnerability correlation and security orchestration platform.
- [OWASP SecureCodeBox](https://github.com/secureCodeBox/secureCodeBox) — Kubernetes-based orchestration platform for running and aggregating security scans at scale.

### Knowledge and Training

- [OWASP SamuraiWTF](https://github.com/SamuraiWTF/samuraiwtf) — Live linux environment pre-loaded with tools and vulnerable targets for web pen-testing practice.
- [OWASP Security Knowledge Framework](https://owasp.org/www-project-security-knowledge-framework/) — Expert system that walks developers through secure coding requirements per technology and feature.

## Companion Tools

Tools outside the OWASP umbrella that integrate cleanly with OWASP standards and are widely used across the security community.

### DAST

- [Burp Suite](https://portswigger.net/burp) — Industry-standard web vulnerability scanner and intercepting proxy by PortSwigger; Community Edition is free.
- [Commix](https://github.com/commixproject/commix) — Automated tool for detecting and exploiting OS command injection vulnerabilities in web applications.
- [Darkmoon](https://github.com/ASCIT31/Dark-Moon) — Open source (GPL-3.0) autonomous AI penetration testing platform covering web, API, Active Directory, and Kubernetes, orchestrating offensive tools as an MCP host with proof of exploitation and a local privacy gateway.
- [Nikto](https://github.com/sullo/nikto) — Long-running open-source web server scanner that tests for outdated software and common misconfigurations.
- [Nuclei](https://github.com/projectdiscovery/nuclei) — Fast, template-based vulnerability scanner driven by a large community template library.
- [OWTF](https://github.com/owtf/owtf) — Offensive Web Testing Framework that unifies many pentesting tools into a semi-automated workflow aligned with the OWASP Testing Guide.
- [sqlmap](https://github.com/sqlmapproject/sqlmap) — Automatic SQL injection detection and exploitation tool.
- [Wapiti](https://github.com/wapiti-scanner/wapiti) — Web application vulnerability scanner that fuzzes scripts and forms for common injection flaws.

### SAST

- [Bandit](https://github.com/PyCQA/bandit) — Security linter for Python code.
- [Brakeman](https://github.com/presidentbeef/brakeman) — Static analysis security scanner for Ruby on Rails.
- [CodeQL](https://github.com/github/codeql) — Semantic code analysis engine from GitHub; treats code as data you can query.
- [gosec](https://github.com/securego/gosec) — Inspects Go source code for security problems by AST analysis.
- [njsscan](https://github.com/ajinabraham/njsscan) — Static security scanner for Node.js applications powered by libsast and semgrep.
- [Semgrep](https://github.com/semgrep/semgrep) — Lightweight static analysis for many languages, driven by pattern rules; strong AppSec rule packs.

### SCA and SBOM

- [Grype](https://github.com/anchore/grype) — Vulnerability scanner for container images and filesystems.
- [OSV-Scanner](https://github.com/google/osv-scanner) — Frontend to the OSV.dev database; scans lockfiles and SBOMs for known vulnerabilities.
- [Snyk Open Source CLI](https://github.com/snyk/cli) — Commercial SCA tool with a free tier; covers many ecosystems.
- [Syft](https://github.com/anchore/syft) — SBOM generator for container images and filesystems; output to CycloneDX, SPDX, and others.
- [Trivy](https://github.com/aquasecurity/trivy) — All-in-one scanner for containers, file systems, git repos, IaC, and Kubernetes; SBOM-aware.

### Secret Scanning

- [detect-secrets](https://github.com/Yelp/detect-secrets) — Pre-commit-friendly secrets scanner from Yelp with baseline-based suppression.
- [Gitleaks](https://github.com/gitleaks/gitleaks) — SAST tool for detecting hardcoded secrets like passwords, API keys, and tokens in git repos.
- [TruffleHog](https://github.com/trufflesecurity/trufflehog) — Finds and verifies leaked credentials by scanning repos, S3, and other sources.

### Infrastructure as Code Scanning

- [Checkov](https://github.com/bridgecrewio/checkov) — Static analysis for Terraform, CloudFormation, Kubernetes, Helm, ARM, and more.
- [KICS](https://github.com/Checkmarx/kics) — Find security vulnerabilities, compliance issues, and IaC misconfigurations across many IaC platforms.
- [Terrascan](https://github.com/tenable/terrascan) — IaC scanner that detects compliance and security violations.
- [tfsec](https://github.com/aquasecurity/tfsec) — Security scanner for Terraform code (now part of the Trivy project).

### Container and Runtime

- [Clair](https://github.com/quay/clair) — Open-source project for static analysis of vulnerabilities in container images.
- [Dockle](https://github.com/goodwithtech/dockle) — Container image linter for security, helping build best-practice Docker images.
- [Falco](https://github.com/falcosecurity/falco) — Cloud-native runtime security tool that detects abnormal behavior using kernel events.
- [kube-bench](https://github.com/aquasecurity/kube-bench) — Checks whether Kubernetes is deployed securely per the CIS Kubernetes Benchmark.
- [kube-hunter](https://github.com/aquasecurity/kube-hunter) — Hunts for security weaknesses in Kubernetes clusters.
- [kube-linter](https://github.com/stackrox/kube-linter) — Static analysis tool that checks Kubernetes YAML and Helm charts against security and configuration best practices.
- [Kubescape](https://github.com/kubescape/kubescape) — Open-source Kubernetes security platform covering misconfiguration, compliance, and vulnerability scanning across the pipeline and runtime.
- [Popeye](https://github.com/derailed/popeye) — Kubernetes cluster sanitizer that scans live clusters for misconfigurations and resources that deviate from best practices.

### Cloud Security

- [Cloud Custodian](https://github.com/cloud-custodian/cloud-custodian) — Rules engine for enforcing security, cost, and governance policies across AWS, Azure, and GCP via a YAML DSL.
- [Prowler](https://github.com/prowler-cloud/prowler) — Open-source cloud security and compliance tool covering AWS, Azure, GCP, and Kubernetes with hundreds of built-in checks.
- [ScoutSuite](https://github.com/nccgroup/ScoutSuite) — Multi-cloud security auditing tool that assesses AWS, Azure, GCP, and other providers' configurations.

### CI/CD and Supply Chain Security

- [cosign (Sigstore)](https://github.com/sigstore/cosign) — Container and binary signing, verification, and transparency-log tooling from the Sigstore project.
- [in-toto](https://github.com/in-toto/in-toto) — Framework for cryptographically attesting to and verifying each step of a software supply chain.
- [OpenSSF Scorecard](https://github.com/ossf/scorecard) — Automated checks that score open-source projects on security best practices (branch protection, pinned dependencies, fuzzing, etc.).

### Fuzzing

- [AFL++](https://github.com/AFLplusplus/AFLplusplus) — Community-maintained successor to AFL with modern instrumentation, coverage-guided fuzzing, and QEMU/Unicorn modes.
- [Jazzer](https://github.com/CodeIntelligenceTesting/jazzer) — Coverage-guided, in-process fuzzer for the JVM, commonly used to fuzz Java and Kotlin code.
- [OSS-Fuzz](https://github.com/google/oss-fuzz) — Google's continuous fuzzing infrastructure for critical open-source projects, integrating with AFL++, libFuzzer, and Honggfuzz.

### API Security

- [Akto](https://github.com/akto-api-security/akto) — Open-source API security testing platform with traffic-aware test generation.
- [Insomnia](https://github.com/Kong/insomnia) — Open-source API client useful for manual API exploration alongside automated scans.
- [Postman / Newman](https://github.com/postmanlabs/newman) — Command-line collection runner for Postman; useful for embedding API security checks into CI.
- [Schemathesis](https://github.com/schemathesis/schemathesis) — Property-based testing for OpenAPI, GraphQL, and other API schemas; finds bugs the spec implies must not exist.

### Mobile Security

- [APKLeaks](https://github.com/dwisiswant0/apkleaks) — Scan APK files for URIs, endpoints, and secrets.
- [Frida](https://github.com/frida/frida) — Dynamic instrumentation toolkit for developers, reverse engineers, and security researchers.
- [MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF) — Mobile Security Framework for automated, all-in-one mobile app pentesting (Android/iOS/Windows) — SAST, DAST, and API testing.
- [Objection](https://github.com/sensepost/objection) — Runtime mobile exploration toolkit powered by Frida.

### AI and LLM Security

- [DeepTeam](https://github.com/confident-ai/deepteam) — Open-source framework for red-teaming LLM applications and agents against common attack vectors.
- [garak](https://github.com/NVIDIA/garak) — LLM vulnerability scanner (maintained by NVIDIA) that probes models for prompt injection, hallucination, jailbreaks, and data leakage.
- [promptfoo](https://github.com/promptfoo/promptfoo) — Open-source LLM testing and red-teaming tool for evaluating prompts, agents, and RAG pipelines in CI/CD.

### Password and Credential Testing

- [hashcat](https://github.com/hashcat/hashcat) — World's fastest and most advanced open-source password recovery and auditing tool with GPU acceleration.
- [John the Ripper](https://github.com/openwall/john) — Long-standing offline password cracker supporting hundreds of hash and cipher types.

### Adversary Emulation and Purple Teaming

- [Atomic Red Team](https://github.com/redcanaryco/atomic-red-team) — Library of small, portable tests mapped directly to MITRE ATT&CK techniques for validating detections.
- [Caldera](https://github.com/apache/caldera) — Automated adversary emulation platform, originally developed by MITRE and now under the Apache Software Foundation.

### Reconnaissance

- [httpx](https://github.com/projectdiscovery/httpx) — Fast, multi-purpose HTTP toolkit that probes hosts and pulls metadata at scale.
- [Metasploit Framework](https://github.com/rapid7/metasploit-framework) — World's most-used penetration testing framework, with thousands of exploits and auxiliary modules.
- [Nmap](https://nmap.org) — De facto standard network scanner for host discovery and service/version detection.
- [Subfinder](https://github.com/projectdiscovery/subfinder) — Fast passive subdomain enumeration tool.

## Standards and Frameworks (non-OWASP)

- [CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks) — Consensus-developed secure-configuration guidelines for systems, cloud, and applications.
- [CWE Top 25](https://cwe.mitre.org/top25/) — The most dangerous software weaknesses, maintained by MITRE.
- [MITRE ATT&CK](https://attack.mitre.org) — Globally accessible knowledge base of adversary tactics and techniques based on real-world observation.
- [NIST SP 800-115](https://csrc.nist.gov/publications/detail/sp/800-115/final) — Technical Guide to Information Security Testing and Assessment.
- [PTES — Penetration Testing Execution Standard](http://www.pentest-standard.org) — Community-developed standard covering pentest methodology end-to-end.
- [SLSA (Supply-chain Levels for Software Artifacts)](https://slsa.dev) — Framework with graduated compliance levels for preventing tampering and securing the software supply chain.

## Vulnerability Databases and Disclosure

- [CISA Known Exploited Vulnerabilities (KEV) Catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog) — U.S. government catalog of vulnerabilities with confirmed real-world exploitation, used to prioritize remediation.
- [CVE Program](https://www.cve.org) — The MITRE-stewarded system for uniquely identifying and cataloging publicly known cybersecurity vulnerabilities.
- [GitHub Advisory Database](https://github.com/github/advisory-database) — Community- and vendor-reported security advisories covering open-source packages across major ecosystems.
- [National Vulnerability Database (NVD)](https://nvd.nist.gov) — NIST's repository of CVE-based vulnerability data enriched with CVSS scores and CPE mappings.
- [OSV.dev](https://osv.dev) — Open Source Vulnerabilities database with a machine-readable schema spanning multiple package ecosystems.

## Learning Platforms

- [Hack The Box](https://www.hackthebox.com) — Penetration-testing labs and challenges, ranging from beginner to expert.
- [PentesterLab](https://pentesterlab.com) — Exercises focused on web application vulnerabilities and exploitation.
- [PortSwigger Web Security Academy](https://portswigger.net/web-security) — Free, hands-on web security training from the makers of Burp Suite.
- [Pwning OWASP Juice Shop](https://pwning.owasp-juice.shop) — Companion book and walkthrough for the Juice Shop challenges.
- [TryHackMe](https://tryhackme.com) — Guided learning paths and rooms for offensive and defensive security topics.
- [VulnHub](https://www.vulnhub.com) — Collection of downloadable vulnerable VM images for offline practice.

## Certifications

- [CISSP (ISC2)](https://www.isc2.org/certifications/cissp) — Broad, management-oriented certification covering security and risk management across eight domains; the most widely recognized general infosec credential.
- [GWAPT (GIAC Web Application Penetration Tester)](https://www.giac.org/certifications/web-application-penetration-tester-gwapt/) — Hands-on certification focused on web application penetration testing methodology and tooling.
- [INE Certifications (eJPT/eWPT)](https://my.ine.com/certifications/) — Practical, lab-based penetration testing certifications aimed at entry-to-intermediate offensive security skills.
- [OSCP (OffSec Certified Professional)](https://www.offsec.com/courses/pen-200/) — Widely recognized hands-on penetration testing certification built around the PEN-200 course.
- [OSWE (OffSec Web Expert)](https://www.offsec.com/courses/web-300/) — Advanced, hands-on certification focused on white-box web application exploitation.

## Books

- *Black Hat Python* (2nd ed.) — Justin Seitz & Tim Arnold, No Starch Press, 2021.
- *Bug Bounty Bootcamp* — Vickie Li, No Starch Press, 2021.
- *The Hacker Playbook 3* — Peter Kim, Secure Planet, 2018.
- *Hacking APIs* — Corey Ball, No Starch Press, 2022.
- *Real-World Bug Hunting* — Peter Yaworski, No Starch Press, 2019.
- *The Tangled Web* — Michal Zalewski, No Starch Press, 2011.
- *The Web Application Hacker's Handbook* (2nd ed.) — Stuttard & Pinto, Wiley, 2011.

## Newsletters and Podcasts

- [Darknet Diaries](https://darknetdiaries.com) — Podcast telling true stories from the dark side of the internet: hacks, breaches, and the people behind them.
- [Risky Business](https://risky.biz) — Long-running weekly security news podcast with deep technical and policy analysis.
- [tl;dr sec](https://tldrsec.com) — Weekly newsletter curating notable AppSec tools, talks, and vulnerability research.

## Bug Bounty Platforms

- [Bugcrowd](https://www.bugcrowd.com) — Crowdsourced security platform running bug bounty and vulnerability disclosure programs for organizations.
- [HackerOne](https://www.hackerone.com) — One of the largest bug bounty and coordinated vulnerability disclosure platforms, used by governments and enterprises.
- [Intigriti](https://www.intigriti.com) — European crowdsourced security platform for bug bounty and penetration-testing-as-a-service programs.
- [YesWeHack](https://www.yeswehack.com) — European bug bounty and vulnerability disclosure platform connecting ethical hackers with organizations.

## Communities and Events

- [Black Hat](https://www.blackhat.com) — Information security event series with technical training and briefings.
- [BSides](http://www.securitybsides.com) — Community-driven framework for local security conferences.
- [DEF CON](https://defcon.org) — One of the world's largest hacker conferences.
- [OWASP Chapters](https://owasp.org/chapters/) — Local meetups around the world; a good entry point for the community.
- [OWASP Global AppSec](https://owasp.org/events/) — Flagship OWASP conferences held annually in multiple regions.

## Related Awesome Lists

- [awesome-api-security](https://github.com/arainho/awesome-api-security) — API security tools, talks, and references. *(Archived May 2026 — useful as a historical reference.)*
- [awesome-appsec](https://github.com/paragonie/awesome-appsec) — Application security learning resources.
- [awesome-fuzzing](https://github.com/cpuu/awesome-fuzzing) — Fuzzing tools, papers, and resources.
- [awesome-mobile-security](https://github.com/vaib25vicky/awesome-mobile-security) — Mobile security resources for Android and iOS.
- [awesome-pentest](https://github.com/enaqx/awesome-pentest) — Penetration testing resources, tools, and references.
- [awesome-security](https://github.com/sbilly/awesome-security) — Broad security tools and resources list.
- [awesome-sec-talks](https://github.com/PaulSec/awesome-sec-talks) — Curated links to security conference talks and recordings.
- [awesome-web-security](https://github.com/qazbnm456/awesome-web-security) — Web security materials and resources.

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
