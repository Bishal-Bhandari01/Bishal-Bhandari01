<div align="center">

<img src="header.svg" alt="Bishal Bhandari" width="860" />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=15&pause=1200&color=00FF41&center=true&vCenter=true&width=640&lines=Tracking+threats+so+you+don%27t+have+to.;SOC+Analyst+%40+Monal+Tech+%7C+Kathmandu%2C+Nepal;OSINT+%7C+Threat+Intelligence+%7C+VAPT;Building+tools+that+make+security+less+painful.;If+it+has+a+CVE%2C+I%27ve+probably+read+it.)](https://git.io/typing-svg)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/bishalbhandari-infosec)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:bishalbhandari390@gmail.com)
[![Stack Overflow](https://img.shields.io/badge/Stack_Overflow-F58025?style=for-the-badge&logo=stackoverflow&logoColor=white)](https://stackoverflow.com/users/18072647)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/Y8GfEcb)

![Profile Views](https://komarev.com/ghpvc/?username=Bishal-Bhandari01&style=flat-square&color=00ff41&label=Profile+Views)

</div>

---

## Hey there 👋

I'm Bishal — a security researcher and SOC analyst based in Kathmandu, Nepal. I've spent the last 2+ years at Monal Tech hunting threats, digging through SIEM alerts, and building tools that automate the boring parts of security work so analysts can focus on what actually matters.

My day-to-day lives somewhere between threat intelligence, OSINT investigations, and vulnerability assessments. I'm equally comfortable writing a Python automation script, tracing a blockchain wallet linked to suspicious activity, or documenting a pen test finding with proper CVSS scoring. I also genuinely enjoy building — not just breaking things.

When I'm not in a SIEM dashboard, I'm probably working on one of my open-source projects or reading about something that probably has a CVE.

---

## What I work with

<table>
<tr>
<td valign="top" width="50%">

**🔍 Intelligence & Investigations**
- OSINT methodology and tooling
- Person-of-interest investigations (digital context)
- Threat actor attribution and profiling
- Blockchain transaction tracing (Chainalysis)
- Social media and deep/dark web reconnaissance
- Structured intelligence reporting (BLUF)

</td>
<td valign="top" width="50%">

**🛡️ Security Operations**
- SIEM monitoring and alert triage (LogPoint, Splunk)
- Vulnerability assessment — Nmap, Burp Suite, OWASP ZAP
- MITRE ATT&CK mapping
- Network and digital forensics
- Incident documentation and response
- Security automation with Python and n8n

</td>
</tr>
</table>

---

## Things I've built

### 🖥️ SysCommand — Linux Server Management Panel
> *Self-hosted. Security-first. Actually usable.*

I built SysCommand because I wanted a server management panel that didn't cut corners on security. It's a full Flask application with real-time system monitoring, Docker container orchestration, and an integrated vulnerability scanner — all gated behind proper RBAC with granular permissions like `docker:start` and `image:scan`.

A few things I'm particularly proud of: the Docker socket is never mounted directly into the app — it goes through a `docker-socket-proxy` (CIS Docker Benchmark compliant). MFA is TOTP-based with backup codes. Every privileged action lands in a structured JSON audit log with CSV/PDF export. The test suite covers unit, integration (Testcontainers), E2E (Playwright), property-based (Hypothesis), contract (Schemathesis), and load testing (Locust).

[![Repo](https://img.shields.io/badge/View_on_GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Bishal-Bhandari01/SysCommand)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

<details>
<summary>More details</summary>
<br>

- Multi-user RBAC with drag-and-drop role editor and toggle-chip permission UI
- TOTP-based MFA with one-time backup codes, optional enforcement at login
- Real-time CPU (per-core), RAM, disk, temperature, and uptime via psutil
- Docker: start/stop/restart/remove, SSE log streaming, image pull with live progress, automated tag-switch lifecycle
- Vulnerability scanning via Grype — CVE dashboard with severity badges, JSON export
- Production hardened: CSP + HSTS + X-Frame-Options (Flask-Talisman), bcrypt cost-12, rate-limited login (5/min), session fixation prevention, CSRF protection

</details>

---

### 🔬 MakeMyScan — Network Vulnerability Scanner
> *Automating the recon work that takes too long by hand.*

An ongoing project — a Python/Django-based network vulnerability scanner with REST APIs for scan management, CVE lookup integration, and an OWASP-aligned web application scanner prototype. Built for extensibility from the ground up.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)

---

### 🧠 Fragment LLM — Lightweight Language Model
> *A GPT-style LLM with security compliance baked in, not bolted on.*

38M parameter language model built with PyTorch, designed for low-resource hardware. The security angle was the whole point — OWASP ASVS 4.0, CWE Top 25, and CIS controls enforced throughout. Replaced `pickle` serialization with JSON checkpoints to eliminate the RCE risk that most ML projects ignore. FP16 training and gradient accumulation cut memory usage by 50%.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)

---

## Certifications

- ✅ **PCI Compliance** — Qualys (2024)
- ✅ **OPSWAT File Security Associate (OFSA)** — 2024
- ✅ **Ethical Hacking Essentials** — 2024

---

## Tech I reach for

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)

**Security Tooling**

![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white)
![OWASP ZAP](https://img.shields.io/badge/OWASP_ZAP-00549E?style=flat-square&logo=owasp&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-0E83CD?style=flat-square&logo=nmap&logoColor=white)
![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)

**Frameworks & Infrastructure**

![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)

**Automation**

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white)

---

## GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Bishal-Bhandari01&show_icons=true&theme=chartreuse-dark&hide_border=true&include_all_commits=true&count_private=true&bg_color=0d1117&title_color=00ff41&icon_color=00ff41&text_color=c9d1d9" height="170" />
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Bishal-Bhandari01&theme=chartreuse-dark&hide_border=true&layout=compact&bg_color=0d1117&title_color=00ff41&text_color=c9d1d9" height="170" />

<br/><br/>

<img src="https://streak-stats.demolab.com?user=Bishal-Bhandari01&theme=chartreuse-dark&hide_border=true&background=0d1117&ring=00ff41&fire=ff6b35&currStreakLabel=00ff41" />

<br/><br/>

<!-- <img src="https://github-profile-trophy.vercel.app/?username=Bishal-Bhandari01&theme=matrix&no-frame=true&no-bg=true&margin-w=6&column=6" /> -->

[![trophy](https://github-profile-trophy.vercel.app/?username=Bishal-Bhandari01&theme=onedark)](https://github.com/Bishal-Bhandari01/github-profile-trophy)

</div>

---

<div align="center">

*"Security is not a product, but a process."* — Bruce Schneier

<br/>

[![BuyMeACoffee](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/WraSinMeliodas)

</div>
