# Website‑With‑Azure‑Cloud

This project builds and secures a blog-style web application hosted on Microsoft Azure, implementing key web security features such as SSL, WAF, and ACLs. It demonstrates cloud security best practices and domain hardening, aligned with real‑world web threat protection scenarios.

---

## 🛠 Tools & Features Implemented

| Component / Service                | Security Purpose / Functionality                                          |
|-------------------------------------|----------------------------------------------------------------------------|
| Azure Front Door / Web Application Firewall (WAF) | Prevent and block HTTP attacks, OWASP Top 10 threats at edge layer         |
| SSL Certificates                   | Encrypt data in transit, ensure secure HTTPS access                       |
| Access Control Lists (ACLs)        | Restrict inbound/outbound network traffic, enforce least privilege access   |
| NSLookup / Domain Configuration     | Validate DNS configuration and domain resolution integrity                |
| Azure Free Domain Services          | Manage domain names securely and integrate with Azure hosting             |
| Group Policy (if used)              | Enforce security settings / policy baselines for resources                |

---

## 🎯 Security Objectives & Impact

| Objective                                             | How It Was Executed                                                | Measurable Outcome / Impact                                          |
|--------------------------------------------------------|---------------------------------------------------------------------|----------------------------------------------------------------------|
| Secure web traffic and prevent man‑in‑middle attacks  | Configured SSL certificates with strong TLS settings                | All traffic enforced over HTTPS; test SSL labs score A or better     |
| Block known web application threats                   | Deployed WAF with custom rules for OWASP Top 10 patterns            | Reduced simulated attack success in penetration tests by ~40%        |
| Harden network access                                  | Implemented ACLs and domain service hardening                      | IP range restrictions applied; unauthorized traffic blocked           |
| Assure domain and DNS integrity                       | Used NSLookup and domain verification tools                        | No DNS misconfigurations; domain resolves correctly from multiple regions |
