# Cybersecurity Risk Assessment

## Objective

This project involved assessing the cybersecurity posture of a simulated client website. The objective was to identify vulnerabilities, evaluate risk levels, and provide actionable recommendations using industry-standard tools and frameworks. The focus was on aligning findings with best practices in Governance, Risk, and Compliance (GRC).

### Skills Learned
Over a two-week period, I conducted a hands-on risk assessment of a live cloud-based web application. Key activities included:
- Researching global and industry-specific cyber threats.
- Conducting automated and manual vulnerability scans.
- Mapping findings to the OWASP Top 10 framework.
- Creating a structured risk report with mitigation strategies.
- Delivering insights and recommendations in a formal presentation.

### Tools Used

- OWASP Zap – Vulnerability scanning
- Burp Suite – Manual web and API testing
- Wireshark – Packet analysis
- OWASP Top 10 – Risk classification framework
- Google Workspace / Docs – Report and presentation creation

### Skills Demonstrated

| Skill                              | Application Example                        |
| ---------------------------------- | ------------------------------------------ |
| Vulnerability Assessment           | Identified critical issues using OWASP Zap |
| Risk Prioritization & Reporting    | Structured risks by severity and impact    |
| OWASP Top 10 Analysis              | Mapped each vulnerability to known threats |
| GRC Understanding                  | Suggested policy and control improvements  |
| Communication of Security Findings | Presented detailed recommendations         |

### 🔎 Vulnerability Findings
The vulnerability assessment revealed multiple high- and critical-risk issues across key OWASP Top 10 categories. Below is a visual snapshot of our findings:

![Vulnerability Findings](./vulnerability-findings.png)

Key highlights include:

- 🔴 **Unauthenticated POST Request** (Critical): Exposes sensitive blog content and author emails without authentication.
- 🟠 **Post-authenticated User Enumeration** (High): Discloses full user directory including PII and privilege levels.
- 🟠 **Weak Password Policy** (High): Allows overly simple passwords, increasing the risk of brute-force and credential stuffing attacks.
- 🟡 **Permissive CORS Policy** (Medium): Allows cross-domain API calls, increasing the risk of unauthorized data access.
- 🟡 **Missing X-Frame-Options Header** (Medium): Enables clickjacking by allowing the site to be embedded in iframes.
- 🔴 **SQL Injection with Command Execution** (Critical): Allows arbitrary SQL and OS commands; full database compromise possible.

Each vulnerability was categorized according to the [OWASP Top 10](https://owasp.org/www-project-top-ten/) and evaluated based on its potential impact to the client's environment.
