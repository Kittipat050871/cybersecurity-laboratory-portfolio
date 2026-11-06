# Cybersecurity Laboratory Portfolio — OWASP ZAP / DVWA / bWAPP

**Academic web vulnerability assessment | Educational laboratory case study**

This repository documents a coursework-based security assessment of **DVWA (Damn Vulnerable Web Application)** and **bWAPP**, two deliberately vulnerable training applications, using **OWASP ZAP** and manual interpretation of request/response evidence. It is a **documentation portfolio**, not a scanner implementation or an assessment of real-world production systems.

## Scope and learning objectives

- Identify and analyze **SQL Injection** behavior in controlled training applications.
- Investigate **brute-force and weak login controls** by comparing authentication responses.
- Analyze **insecure login forms**, including credential exposure or client-side obfuscation in laboratory scenarios.
- Compare observations across the **Low / Medium / High** security settings documented in the coursework.
- Report technical evidence, limitations, and defensive recommendations clearly.

## Coursework results summary

| Lab application | Security topic | Low | Medium | High |
|---|---|---|---|---|
| DVWA | SQL Injection | Demonstrated | Demonstrated | Not reproduced by tested methods |
| DVWA | Brute Force | Demonstrated | Demonstrated | Demonstrated with a refreshed anti-CSRF token |
| bWAPP | SQL Injection (GET/Select) | Demonstrated | Demonstrated | Not reproduced by tested methods |
| bWAPP | Insecure Login Forms | Demonstrated | Demonstrated | Demonstrated in the recorded lab conditions |

**Interpretation:** These observations reflect particular lab configurations and testing methods. A test that does not reproduce a vulnerability is **not proof that all variants are prevented**. The original report attributes the more resistant SQLi cases to use of parameterized queries, based on observed behavior; this is not an independent source-code audit.

## Case study

[Web Vulnerability Assessment — Case Study (PDF)](docs/Web_Vulnerability_Assessment_Case_Study.pdf)

## Repository contents

```text
cybersecurity-laboratory-portfolio/
├── README.md
└── docs/
    └── Web_Vulnerability_Assessment_Case_Study.pdf
```

## Tools and environment

- **OWASP ZAP** — intercepting/testing HTTP requests and inspecting responses within the training environment.
- **DVWA** — intentionally vulnerable training web application.
- **bWAPP** — intentionally vulnerable training web application.

## Professional practices and limitations

- Testing described here was coursework on purpose-built vulnerable lab targets; **no unauthorized testing is endorsed**.
- This portfolio is derived from the existing academic report, not a claim of new testing or independent verification.
- It does not publish raw credentials, classmates' personal information, or original class assignment documents.
- The work may involve classmates or team contributions; this is a **portfolio summary, not a claim of sole authorship**.
- **No source code is included**: the deliverable is methodology, findings, and security reporting.
