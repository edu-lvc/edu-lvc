# Eduardo Jurado

**.NET Software Developer · Application Security · Open Source Contributor**

I fix bugs and security issues in production open source projects (Elsa Workflows, ASP.NET Core, GLPI), and I back every fix with regression tests.

<p align="left">
  <a href="https://github.com/edu-lvc"><img src="https://img.shields.io/badge/GitHub-edu--lvc-181717?style=for-the-badge&logo=github" /></a>
  <a href="https://www.linkedin.com/in/eduardo-felipe-jurado-ramos-a3b143251/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin" /></a>
  <a href="mailto:eduardoj2056@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

<p align="left">
  <img src="https://skillicons.dev/icons?i=cs,dotnet,azure,docker,linux,git,github" />
</p>

📍 Panama · 🗣️ Spanish (native) · English (technical)

---

## About

Software developer with 3+ years of experience building enterprise applications, automating business processes and operating the infrastructure behind them. My core stack is **C#, .NET / ASP.NET Core and SQL Server**, with a growing focus on **security**: secure software development, access control, system hardening and log analysis.

I am in the final year of a Bachelor's degree in Cybersecurity (Universidad Tecnológica de Panamá). I contribute to international open source projects, where I reproduce issues, find root causes, write tests and work through maintainer code reviews.

---

## Open Source Contributions

**Elsa Workflows:** 6 merged pull requests in November 2026, 2 more open.

### Elsa Workflows · Elsa Core

**Security and identity**

[![PR 9204](https://img.shields.io/badge/PR_%239204-Merged-8957e5?style=flat-square&logo=github)](https://github.com/elsa-workflows/elsa-core/pull/9204)
The modular server now validates the Identity token signing key at startup, so Production no longer boots with an insecure placeholder key. Includes smoke tests for Production, Demo and Identity-disabled scenarios.

[![PR 9209](https://img.shields.io/badge/PR_%239209-Open-2da44e?style=flat-square&logo=github)](https://github.com/elsa-workflows/elsa-core/pull/9209)
Identity login now returns HTTP 401 for invalid credentials instead of 200, and Studio's anonymous login calls no longer trigger token refresh. Scheduled for the 3.11 release branch.

**Multi-tenancy**

[![PR 9210](https://img.shields.io/badge/PR_%239210-Merged-8957e5?style=flat-square&logo=github)](https://github.com/elsa-workflows/elsa-core/pull/9210)
EF Core now validates explicit tenant IDs, matching the existing Dapper behavior: it stamps the ambient tenant on entities without one and rejects conflicting tenant IDs.

[![PR 9205](https://img.shields.io/badge/PR_%239205-Merged-8957e5?style=flat-square&logo=github)](https://github.com/elsa-workflows/elsa-core/pull/9205)
Normalized tenant ID handling across the MassTransit, Hangfire and Quartz integrations, keeping backward compatibility with previously scheduled jobs. 254 tests passing.

[![PR 9239](https://img.shields.io/badge/PR_%239239-Open-2da44e?style=flat-square&logo=github)](https://github.com/elsa-workflows/elsa-core/pull/9239)
Architecture Decision Record defining how tenant-agnostic workflow definitions handle triggers, instance ownership, timers, cron and recovery.

**Data and runtime fixes**

[![PR 9177](https://img.shields.io/badge/PR_%239177-Merged-8957e5?style=flat-square&logo=github)](https://github.com/elsa-workflows/elsa-core/pull/9177)
Fixed MySQL migrations (Labels and Secrets): removed unsupported `SIGNAL` pre-checks and made migrations retry-safe, with integration tests.

[![PR 9157](https://img.shields.io/badge/PR_%239157-Merged-8957e5?style=flat-square&logo=github)](https://github.com/elsa-workflows/elsa-core/pull/9157)
Fixed handling of nested generic activity type names, with regression tests.

**CI**

[![PR 9248](https://img.shields.io/badge/PR_%239248-Merged-8957e5?style=flat-square&logo=github)](https://github.com/elsa-workflows/elsa-core/pull/9248)
Reordered the npm publish workflow so the Studio WASM package is published and verified before the React package, with gate validation to enforce the order.

### Microsoft .NET · ASP.NET Core

[![PR 70109](https://img.shields.io/badge/PR_%2370109-In_Review-orange?style=flat-square&logo=github)](https://github.com/dotnet/aspnetcore/pull/70109)
Security fix: restricted file permissions on the `user-jwts` signing key on Unix, with regression and cross-platform tests.

### GLPI Project · GLPI

[![PR 26151](https://img.shields.io/badge/PR_%2326151-In_Review-orange?style=flat-square&logo=github)](https://github.com/glpi-project/glpi/pull/26151)
Security fix: corrected personal token handling in planning iCal export links.

**How I work on a contribution:** reproduce the issue, find the root cause, implement the fix following the project's conventions, add tests, and iterate on review feedback with the maintainers.

---

## Technical Skills

| Area | Technologies |
|---|---|
| **Languages & frameworks** | C#, .NET, ASP.NET Core, VB.NET, .NET MAUI, Java / Spring, Python, JavaScript, SQL |
| **Databases** | SQL Server, PostgreSQL, MariaDB / MySQL, SQL optimization, data integration |
| **Cloud & DevOps** | Microsoft Azure, Azure DevOps, Docker, Git / GitHub, CI/CD |
| **Security** | Secure software development, Linux hardening, access control, auditd and log analysis, Wazuh, Fortinet, Wireshark |
| **Infrastructure** | Windows Server, Linux (Debian, Rocky), Active Directory, DNS, DHCP, VMware, pfSense, GLPI, Zabbix |
| **Automation & BI** | Power Automate, Power Apps, AppSheet, n8n, Power BI, Microsoft Fabric |

---

## Featured Work

### Panama Fuel Prices API *(in development)*
Open source API that centralizes Panama's official fuel prices: collects data from government publications, automates extraction and updates, and exposes it in a structured, public format.

### Enterprise Software & Automation
Business applications and internal tools in C# / .NET with SQL Server, plus process automation and reporting with Power Platform, n8n, Power BI and Microsoft Fabric.

### Infrastructure & Security Lab
Environment with Windows Server and Active Directory, Debian and Rocky Linux, pfSense, Wazuh monitoring, auditd-based Linux auditing and Docker deployments.

---

## Education & Certifications

**Education**
- Bachelor's Degree in Cybersecurity, Universidad Tecnológica de Panamá (final year)
- Back End Development (Java / Spring), Oracle Next Education
- Google IT Support Professional Certificate, Coursera

**Certifications**
- Fortinet NSE 3 and NSE 2 Certified in Cybersecurity, Fortinet
- Fortinet Certified Fundamentals in Cybersecurity, Fortinet
- SOC Analyst Level 1 Bootcamp (v6), ComunidadDOJO
- Oracle Cloud Infrastructure 2025 Certified Foundations Associate, Oracle
- Ethical Hacker and Junior Cybersecurity Analyst Career Path, Cisco
- LFD121: Developing Secure Software, The Linux Foundation

---

## Focus Areas

Backend engineering · .NET ecosystem · Application security · Secure software development · Multi-tenant systems · Cloud infrastructure · Database engineering · Process automation

---

## Contact

[GitHub](https://github.com/edu-lvc) · [LinkedIn](https://www.linkedin.com/in/eduardo-felipe-jurado-ramos-a3b143251/) · [eduardoj2056@gmail.com](mailto:eduardoj2056@gmail.com)
